# GitHub Documentation Ingestion Pipeline

A lightweight Python pipeline that downloads GitHub repositories, extracts documentation files, parses frontmatter metadata, and prepares structured data for Retrieval-Augmented Generation (RAG), semantic search, and AI agent applications.

## Features

* Download GitHub repositories directly as ZIP archives
* Process repositories entirely in memory
* Extract Markdown (`.md`) and MDX (`.mdx`) files
* Parse YAML frontmatter metadata
* Generate structured document records
* Compatible with RAG and vector database pipelines

## Tech Stack

* Python
* Requests
* python-frontmatter
* zipfile
* Jupyter Notebook

## Example

```python
from repo_ingestion import read_repo_data

faq_docs = read_repo_data(
    "DataTalksClub",
    "faq"
)

print(len(faq_docs))
print(faq_docs[0])
```

## Example Repositories

* DataTalksClub FAQ
* Evidently AI Documentation

## Use Cases

* AI Agents
* Retrieval-Augmented Generation (RAG)
* Documentation Search
* Knowledge Base Construction
* LLM Evaluation Pipelines

## Future Improvements

* Document chunking
* Embedding generation
* Vector database integration
* Semantic search
* Agentic retrieval workflows
