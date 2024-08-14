## Overview

This project is designed to extract structured data from complex, unstructured PDFs using a multi-stage processing pipeline. The solution integrates **Azure Document Intelligence**, [**Unstructured.io**](http://unstructured.io/), and **GPT-4** to achieve high accuracy in data extraction, particularly from documents with complex tables and layouts.

## Features

- **Multi-Stage Processing Pipeline**: The pipeline breaks down the task into multiple stages, each optimized for handling different aspects of unstructured data.
- **Integration with Azure Document Intelligence**: Leverages Azure's powerful document processing capabilities to extract structured information from PDFs.
- **Use of GPT-4**: Utilizes GPT-4 for natural language understanding and to fill gaps where traditional methods may fall short.
- [**Unstructured.io](http://unstructured.io/) Integration**: Employs [Unstructured.io](http://unstructured.io/)'s API for enhanced data extraction from difficult or non-standard layouts.
- **High Accuracy**: Achieves 97% accuracy in data extraction, especially from highly unstructured and complex PDFs.

## Installation

### Prerequisites

- Python 3.8+
- Azure Subscription with access to Document Intelligence API
- [Unstructured.io](http://unstructured.io/) API key
- OpenAI API key (for GPT-4)
- Other dependencies as listed in `requirements.txt`

### Steps

1. **Clone the Repository**:
    
    ```bash
    git clone <https://github.com/yourusername/Unstructured-Azure-LLM.git>
    cd Unstructured-Azure-LLM
    
    ```
    
2. **Install Dependencies**:
    
    ```bash
    pip install -r requirements.txt
    
    ```
    
3. **Set Up Environment Variables**:
    - `AZURE_API_KEY`: Your Azure Document Intelligence API key.
    - `UNSTRUCTURED_IO_KEY`: Your [Unstructured.io](http://unstructured.io/) API key.
    - `OPENAI_API_KEY`: Your OpenAI GPT-4 API key.
    - You can set these in a `.env` file or export them directly in your shell.
4. **Run the Jupyter Notebook**:
    - Start Jupyter Notebook:
        
        ```bash
        jupyter notebook
        
        ```
        
    - Open `Unstructured+Azure+LLM.ipynb` and run the cells to process your PDFs.

## Usage

1. **Upload Your PDFs**: Place the PDFs you want to process in the specified directory.
2. **Run the Pipeline**: Execute the notebook cells to process the PDFs through the multi-stage pipeline.
3. **View Results**: The processed results will be stored in the output directory in a structured format (e.g., CSV, JSON).

## Configuration

- **Pipeline Stages**: You can modify the individual stages of the pipeline by editing the corresponding sections in the notebook.
- **API Keys**: Ensure that your API keys are correctly configured in the environment to avoid any issues during execution.

## Contact

For any questions or issues, please reach out to **Aryan Gandhi** at [aryangan@usc.edu](mailto:aryangan@usc.edu).
