# IMD0187 - Natural Language Processing

## [Dr. Elias Jacob de Menezes Neto](https://docente.ufrn.br/elias.jacob)

This repository contains the code and resources for the course. The course covers a wide range of topics in Natural Language Processing (NLP) and Generative Models, including the basics of NLP, transformer architecture, embeddings, large language models (LLMs), and retrieval augmented generation (RAG).

- **Natural Language Processing (NLP) basics**: Explore techniques like bag-of-words, TF-IDF, and word embeddings for processing and understanding text data.
- **Transformer Architecture**: Learn about the revolutionary transformer architecture, including self-attention mechanisms and the encoder-decoder structure. Understand the impact of models like BERT.
- **Embeddings**: Dive into the concept of embeddings and their role in representing text, images, and other data types in generative models.
- **Large Language Models (LLMs)**: Explore the world of foundation models, fine-tuning techniques, and prompt engineering for generating human-like text.
- **Retrieval Augmented Generation (RAG)**: Understand how retrieval-based methods can enhance the performance and capabilities of generative models.

Throughout the course, you will have the opportunity to work on practical exercises and projects to solidify your understanding of the concepts. I will provide code examples and resources to support your learning journey.

## Prerequisites

To get started with the course, ensure that you have the following prerequisites:

- Access to a machine with a GPU (recommended) or Google Colab for running computationally intensive tasks.
- Installation of [Conda](https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html) for managing Python environments.
- An account with [Weights & Biases](https://wandb.ai/) for experiment tracking and visualization.

## Installation

Follow these steps to set up the environment and dependencies:

1. **Download this Repository:**

   Clone this repository to your local machine using:

   ```shell
    git clone https://github.com/eliasjacob/imd0187-residencia_dpe.git
    cd imd0187-residencia_dpe
    ```

2. **Run the Download Script:**

   Run the following script to download the required resources:

   ```shell
   bash download_datasets_and_binaries.sh
   ```

3. **Install Ollama:**

   Download and install Ollama from [here](https://ollama.com/download).

4. **Download LLama 3.1:**

   After installing Ollama, run the following command to download LLama 3.1:

   ```bash
   ollama pull llama3.1
   ```

5. **Set up Conda Environment:**

   Create and activate the Conda environment using the provided `environment.yml` file. For better performance, I suggest you use [Mamba](https://mamba.readthedocs.io/en/latest/installation/mamba-installation.html) instead of Conda. It looks like Conda, but it is faster. Just replace `conda` with `mamba` in the commands below:

   ```bash
   conda env create -f environment.yml
   conda activate imd0187
   ```

6. **Authenticate Weights & Biases:**

   Create a Weights & Biases account if you haven't already. Then, authenticate by running:

   ```bash
   wandb login
   ```

## Getting Started

Once you have the environment set up, you can start exploring the course materials, running the code examples, and working on the practical exercises.

### Notes

- Certain parts of the code may require a GPU for efficient execution. If you don't have access to a GPU, you can use Google Colab for running the code.

## Contributing

Contributions to the course repository are welcome! If you have any improvements, bug fixes, or additional resources to share, please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/YourFeature`).
3. Make your changes.
4. Commit your changes (`git commit -m 'Add some feature'`).
5. Push to the branch (`git push origin feature/YourFeature`).
6. Create a Pull Request.

## Contact

You can [contact me](elias.jacob@ufrn.br) for any questions or feedback regarding the course materials or repository.