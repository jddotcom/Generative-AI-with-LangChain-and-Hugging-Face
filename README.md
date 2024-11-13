# Generative AI with LangChain and Hugging Face

![Project Banner](https://path-to-image.com/banner.png)

Welcome to the **Generative AI with LangChain and Hugging Face** project! This repository provides tutorials and resources to guide you through using **LangChain** and **Hugging Face** for building generative AI models. LangChain facilitates working with language models in a streamlined way, while Hugging Face provides access to an extensive hub of open-source models.

## Table of Contents
- [Introduction](#introduction)
- [Project Overview](#project-overview)
- [Installation](#installation)
- [Repository Structure](#repository-structure)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [Examples](#examples)
- [Contributing](#contributing)
- [License](#license)

## Introduction

Generative AI models, especially language models, have revolutionized natural language processing by enabling tasks such as text generation, summarization, translation, and more. This repository is designed to show how to use **LangChain** and **Hugging Face Transformers** to easily create, deploy, and interact with generative AI models.

## Project Overview

This repository provides a collection of Jupyter notebooks that walk through:

1. **Building Language Models**: Using LangChain to structure language models.
2. **Using Hugging Face Transformers**: Accessing pretrained models on the Hugging Face Hub.
3. **Creating and Using Pipelines**: For common NLP tasks (e.g., text generation, summarization, Q&A).
4. **Fine-Tuning Language Models**: Training models on specific datasets.

### Key Features
- **LangChain Integration**: An intuitive way to manage and chain language models.
- **Hugging Face Model Hub Access**: Direct integration with popular transformers for fast experimentation.
- **Pipeline Customization**: Modify and build NLP pipelines to suit project needs.
- **Detailed Notebooks**: Step-by-step instructions and examples for building generative AI projects.

## Installation

### Prerequisites

- Python 3.7 or higher
- Jupyter Notebook
- Necessary libraries listed in `requirements.txt`

### Step-by-Step Installation

1. **Clone the Repository**

    ```bash
    git clone https://github.com/krishnaik06/Gen-AI-With-Hugging-Face.git
    cd Gen-AI-With-Hugging-Face
    ```

2. **Create a Virtual Environment**

    ```bash
    python -m venv gen-ai-env
    source gen-ai-env/bin/activate  # On Windows, use `gen-ai-env\Scripts\activate`
    ```

3. **Install Dependencies**

    ```bash
    pip install -r requirements.txt
    ```

4. **Launch Jupyter Notebook**

    ```bash
    jupyter notebook
    ```

5. Open `1_Langchain_And_Huggingface.ipynb` in Jupyter Notebook and follow along with the tutorial.

## Repository Structure

```plaintext
Gen-AI-With-Hugging-Face/
│
├── notebooks/
│   └── 1_Langchain_And_Huggingface.ipynb       # Tutorial notebook for using LangChain and Hugging Face
│
├── requirements.txt                            # List of dependencies
├── README.md                                   # Project documentation (you are here)
├── LICENSE                                     # Project license
└── assets/                                     # Directory for images and other assets
```

## Getting Started

To get started with generative AI using LangChain and Hugging Face, open the `1_Langchain_And_Huggingface.ipynb` notebook in Jupyter. This notebook covers the following:

- **Loading and Inspecting Pretrained Models**: How to fetch and use models from Hugging Face's model hub.
- **Setting Up LangChain**: Create chains of language models to manage tasks like text generation or summarization.
- **Customizing Pipelines**: Use specific parameters to fine-tune language model performance.

### Prerequisites

Before using the notebook, ensure you have an API key from Hugging Face (required for accessing some models) and basic knowledge of Python and Jupyter.

## Usage

1. **Load Models**: Use Hugging Face Transformers to load pre-trained models directly.
2. **Create Language Chains**: Use LangChain to create and test different chains of models.
3. **Experiment with Tasks**: Test the models on NLP tasks like summarization, translation, or text generation.
4. **Fine-Tune Models**: Customize models on your own dataset if desired.

## Examples

### Text Generation with GPT-2

In the `1_Langchain_And_Huggingface.ipynb` notebook, you can follow an example to perform text generation:

```python
from transformers import pipeline

generator = pipeline('text-generation', model='gpt2')
result = generator("Once upon a time,")
print(result[0]['generated_text'])
```

### Using LangChain with Hugging Face Models

LangChain allows chaining together multiple language models. See the notebook for a more detailed example of chaining models together.

## Contributing

We welcome contributions! To contribute:

1. Fork the repository.
2. Create a new branch with your feature or bugfix.
3. Commit and push your changes.
4. Open a Pull Request for review.

## License

This project is licensed under the MIT License.
