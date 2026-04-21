# Open PDF Parser
Self-hostable PDF parsing engine for structured text and table extraction. Works locally or via Docker.

## Features
- Extract text from PDFs
- Extract tables
- Supports password-protected PDFs (user should know the password)
- Runs locally or via Docker

## Quick Start

### Docker
docker build -t open-pdf-parser .
docker run -p 8000:8000 open-pdf-parser

### Local
pip install -r requirements.txt
uvicorn app.main:app --reload
