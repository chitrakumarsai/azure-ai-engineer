# Azure AI Engineer Project

This repository contains AI and machine learning projects built using Azure AI services and Prompt Flow.

## Project Structure

```
.
├── ai/
│   ├── language_translation.ipynb    # Notebook for language translation tasks
│   ├── test_translations.ipynb      # Test cases for translation functionality
│   └── promptflows/
│       └── new-chat-flow-created-at-2025-5-31/  # Chat flow implementation
├── main.py
└── requirements.txt
```

## Features

- **Chat Flow Implementation**: An interactive chat system using Azure OpenAI GPT models
- **Language Translation**: Jupyter notebooks for language translation tasks
- **Prompt Flow Integration**: Structured prompt engineering using Azure's Prompt Flow

## Prerequisites

- Python 3.11+
- Azure OpenAI Service subscription
- Prompt Flow CLI
- Required Python packages (specified in requirements.txt)

## Setup

1. Clone the repository
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Configure Azure OpenAI connection:
   ```bash
   pf connection create --file azure_openai.yaml
   ```

## Usage

### Running the Chat Flow

```bash
cd ai/promptflows/new-chat-flow-created-at-2025-5-31
pf flow test --flow . --interactive
```

### Running Translations

Open and run the Jupyter notebooks in the `ai/` directory:
- `language_translation.ipynb` for translation tasks
- `test_translations.ipynb` for testing the translations

## Configuration

The project uses YAML files for configuration:
- `azure_openai.yaml`: Azure OpenAI service configuration
- `flow.dag.yaml`: Prompt Flow DAG configuration
