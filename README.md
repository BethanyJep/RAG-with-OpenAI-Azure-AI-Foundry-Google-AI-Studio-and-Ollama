# RAG with Multiple AI Platforms

This repository demonstrates a Retrieval-Augmented Generation (RAG) implementation across multiple AI platforms, designed specifically for querying an employee handbook. The project showcases RAG implementations using:
- OpenAI
- Azure OpenAI
- Google AI Studio (Gemini)
- Ollama (local models, featuring gemma3n:latest)

## Overview

The project includes a comprehensive Jupyter notebook (`rag_implementation.ipynb`) that demonstrates:
1. Processing an employee handbook PDF (with fallback to sample data)
2. Creating and managing vector embeddings for document sections
3. Implementing RAG using multiple AI platforms
4. Comparing results and performance across platforms
5. Best practices for each platform's implementation

## Features

- **PDF Processing**: Automatic extraction and sectioning of employee handbook content
- **Vector Store**: ChromaDB implementation for efficient similarity search
- **Multiple Platform Support**: 
  - OpenAI (using latest SDK)
  - Azure OpenAI Service
  - Google AI Studio (using Gemini model)
  - Ollama (with gemma3n:latest model)
- **RAG Components**:
  - Document chunking and embedding
  - Similarity search
  - Context-aware prompt engineering
  - Response generation
- **Performance Comparison**: Tools for comparing responses across platforms
- **Error Handling**: Robust error handling and fallback mechanisms

## Setup Instructions

### Prerequisites
- Python 3.8+
- API keys for cloud services:
  - OpenAI API key
  - Azure OpenAI Service key and endpoint
  - Google AI Studio API key
- Ollama installation (optional, for local model usage)
- VS Code or Jupyter Notebook environment

### Installation

1. Clone this repository:
   ```bash
   git clone [repository-url]
   cd RAG-with-OpenAI-Azure-AI-Foundry-Google-AI-Studio-and-Ollama
   ```

3. Create a `.env` file with your API keys:
   ```
   OPENAI_API_KEY=your_openai_api_key
   AZURE_OPENAI_API_KEY=your_azure_openai_key
   AZURE_OPENAI_ENDPOINT=your_azure_endpoint
   AZURE_OPENAI_API_VERSION=your_azure_openai_api_version
   GOOGLE_API_KEY=your_google_api_key
   ```

4. (Optional) Install Ollama for local model support:
   ```bash
   # Follow Ollama installation instructions from: https://ollama.ai
   ollama pull gemma3n:latest
   ```

### Running the Notebook

1. Open `rag_implementation.ipynb` in Jupyter or VS Code
2. Run each cell in sequence
3. The notebook includes:
   - Setup and configuration
   - PDF processing and chunking
   - Vector store initialization
   - Platform-specific RAG implementations
   - Comparison tools and examples

## Usage Examples

The notebook includes sample queries specifically designed for HR/employee handbook scenarios:
- Policy lookups
- Benefits information
- Procedure clarifications
- Company guidelines

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License.

