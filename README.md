# Let's load the notebook file to understand its structure and contents.
import nbformat

# Load the notebook content
notebook_path = '/mnt/data/TesisHV.ipynb'
with open(notebook_path, 'r', encoding='utf-8') as file:
    notebook_content = nbformat.read(file, as_version=4)

# Extract key information from cells (especially markdown and code cells) for README preparation
notebook_summary = {
    "markdown_cells": [],
    "code_cells": []
}

for cell in notebook_content['cells']:
    if cell.cell_type == 'markdown':
        notebook_summary['markdown_cells'].append(cell.source)
    elif cell.cell_type == 'code':
        notebook_summary['code_cells'].append(cell.source[:200])  # Sample first 200 characters of code for summary

notebook_summary
