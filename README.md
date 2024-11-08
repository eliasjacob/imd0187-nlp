# IMD0187 / PPGTIXXXX - Natural Language Processing

## [Dr. Elias Jacob de Menezes Neto](https://docente.ufrn.br/elias.jacob)

This repository contains the code and resources for the course. The course covers a broad spectrum of topics in Natural Language Processing (NLP) and Generative Models, including foundational concepts, advanced architectures, and practical applications.

## Course Topics

### Natural Language Processing (NLP) Basics
- **Bag-of-Words**: Understand this simple yet powerful representation of text where each word is represented by its count or frequency in a document.
- **TF-IDF (Term Frequency-Inverse Document Frequency)**: Learn how to weigh words based on their frequency in a document relative to their frequency across all documents, enhancing the representation by highlighting important words while downplaying common ones.
- **Word Embeddings**: Explore vector representations of words that capture semantic relationships, enabling more nuanced text processing and analysis.

### Transformer Architecture
- **Self-Attention Mechanisms**: Dive into how transformers utilize self-attention to weigh the significance of different words in a sentence, allowing for more context-aware representations.
- **Encoder-Decoder Structure**: Understand the role of the encoder in processing input data and the decoder in generating output, fundamental to many NLP tasks.
- **Impact of Models like BERT (Bidirectional Encoder Representations from Transformers)**: Study how BERT and similar models have revolutionized NLP by leveraging bi-directional context.

### Embeddings
- **Concept of Embeddings**: Learn about embeddings beyond text, including their application in representing images and other data types within generative models.
- **Role in Generative Models**: Understand how embeddings facilitate the representation and generation of diverse data types.

### Large Language Models (LLMs)
- **Foundation Models**: Explore the architecture and training of large pre-trained models that serve as the basis for various NLP applications.
- **Fine-Tuning Techniques**: Learn methods for adapting pre-trained models to specific tasks, enhancing their performance and applicability.
- **Prompt Engineering**: Study the art of designing prompts to coax desired responses from generative models, crucial for applications like chatbots and content generation.

### Retrieval Augmented Generation (RAG)
- **Retrieval-Based Methods**: Understand how integrating retrieval mechanisms can augment generative models, improving their performance by incorporating relevant external information.

## Prerequisites

To get started with the course, ensure you have the following:

- **Access to a Machine with a GPU**: Recommended for running computationally intensive tasks, or alternatively use Google Colab.
- **Installation of Conda**: For managing Python environments. Follow the installation guide [here](https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html).
- **Weights & Biases Account**: For experiment tracking and visualization. Sign up [here](https://wandb.ai/).

## Installation

Follow these steps to set up the environment and dependencies:

1. **Download the Repository**:
    ```shell
    git clone https://github.com/eliasjacob/imd0187-nlp.git
    cd imd0187-nlp
    ```

2. **Install Dependencies**:
 - For GPU support:
    ```shell
    poetry install --sync -E cuda --with cuda
    poetry shell
    ```
- For CPU-only support:
    ```shell
    poetry install --sync -E cpu
    poetry shell
    ```

3. **Run the Download Script**:
    ```shell
    bash download_datasets_and_binaries.sh
    ```

4. **Install Ollama**:
   Download and install Ollama from [here](https://ollama.com/download).

5. **Download LLama 3.1**:
    ```bash
    ollama pull llama3.1
    ```

6. **Authenticate Weights & Biases**:
    ```bash
    wandb login
    ```

## Using VS Code Dev Containers

This repository is configured to work with Visual Studio Code Dev Containers, providing a consistent and isolated development environment. To use this feature:

1. Install [Visual Studio Code](https://code.visualstudio.com/) and the [Remote - Containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers) extension.

2. Clone this repository to your local machine (if you haven't already):

3. Open the cloned repository in VS Code.

4. When prompted, click "Reopen in Container" or use the command palette (F1) and select "Remote-Containers: Reopen in Container".

5. VS Code will build the Docker container and set up the development environment. This may take a few minutes the first time.

6. Once the container is built, you'll have a fully configured environment with all the necessary dependencies installed.

Using Dev Containers ensures that all course participants have the same development environment, regardless of their local setup. It also makes it easier to manage dependencies and avoid conflicts with other projects.

## Getting Started

Once the environment is set up, you can start exploring the course materials, running code examples, and working on the practical exercises.

### Notes

- Some parts of the code may require a GPU for efficient execution. If you don't have access to a GPU, consider using Google Colab.

## Teaching Approach

The course will use a **top-down** teaching method, which is different from the traditional **bottom-up** approach. 

- **Top-Down Method**: We'll start with a high-level overview and practical application, then delve into the underlying details as needed. This approach helps maintain motivation and provides a clearer picture of how different components fit together.
- **Bottom-Up Method**: Typically involves learning individual components in isolation before combining them into more complex structures, which can sometimes lead to a fragmented understanding.

### Example: Learning Baseball
Harvard Professor David Perkins, in his book [Making Learning Whole](https://www.amazon.com/Making-Learning-Whole-Principles-Transform/dp/0470633719), compares learning to playing baseball. Kids don't start by memorizing all the rules and technical details; they begin by playing the game and gradually learn the intricacies. Similarly, in this course, you'll start with practical applications and slowly uncover the theoretical aspects.

> **Important**: Don't worry if you don't understand everything initially. Focus on what things do, not what they are. 

### Learning Methods
1. **Doing**: Engage in coding and building projects.
2. **Explaining**: Write about what you've learned or help others in the course.

You'll be encouraged to follow along with coding exercises and explain your learning to others. Summarizing key points as the course progresses will also be part of the learning process.

## Final Grade

Your final project will be evaluated based on several criteria:

- **Technical Quality**: How well you implement the project.
- **Creativity**: The originality of your approach.
- **Usefulness**: The practical value of your project for the court.
- **Presentation**: How effectively you present your project.
- **Report**: The clarity and thoroughness of your report.

### Project Guidelines
- **Individual Work**: The project must be done individually.
- **Submission**: Submit a link to a GitHub repo/shared folder with your code, data, and report. Use virtual environments or `requirements.txt` to facilitate running your code.
- **Confidential Data**: Be mindful of any confidential data used in your project.
- **Deadline**: The project will be due 15 days after the end of the course.
- **Submission Platform**: Submit your project using SIGAA.

## Contributing

Contributions to the course repository are welcome! Follow these steps to contribute:

1. Fork the repository.
2. Create a new branch:

    ```shell
    git checkout -b feature/YourFeature
    ```

3. Make your changes.
4. Commit your changes:

    ```shell
    git commit -m 'Add some feature'
    ```

5. Push to the branch:

    ```shell
    git push origin feature/YourFeature
    ```

6. Create a Pull Request.

## Contact

For any questions or feedback regarding the course materials or repository, you can [contact me](mailto:elias.jacob@ufrn.br).