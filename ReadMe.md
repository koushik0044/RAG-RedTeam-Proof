# RAG-RedTeam-Proof

This repository implements a Retrieval-Augmented Generation (RAG) architecture designed for red teaming purposes. The system classifies user queries into relevant and irrelevant categories and processes them accordingly using a Groq LLaMA3-70B language model.

## Architecture

The architecture consists of the following components:

1. **User Query**: The input provided by the user.
2. **Classification Chain**: Determines whether the query is relevant or irrelevant.
3. **Prompt Template for Classification**: A template used to format the classification prompt.
4. **LLM Groq LLaMA3-70B**: The language model used for classification and generation tasks.
5. **StrOutputParser**: Parses the output from the language model.
6. **Business Chain**: Handles relevant queries by interfacing with a retriever.
7. **Retriever (Pinecone)**: Retrieves relevant documents from the database.
8. **Prompt Template for Business**: A template used to format the business-specific prompt.
9. **Out of Context Response**: Generates a response for irrelevant queries.
10. **Output Answer**: The final answer outputted to the user.
11. **Handle Query Function**: Handles the entire query processing flow.

## Notebook

The implementation details and code are provided in the `RAG-Business.ipynb` notebook.

## Flowchart

![RAG Architecture]([path/to/your/image/RAG-Architecture.png](https://github.com/koushik0044/RAG-RedTeam-Proof/blob/692d352188a31cbc09baa5c3b5d16704cfb2fa5d/RAG-Architecture.png))

## Getting Started

### Prerequisites

- Python 3.x
- Jupyter Notebook
- Pinecone (for document retrieval)
- Groq LLaMA3-70B model

### Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/koushik0044/RAG-RedTeam-Proof.git
    cd RAG-RedTeam-Proof
    ```

2. Run the Jupyter Notebook:
    ```bash
    jupyter notebook RAG-Business.ipynb
    ```

## Usage

1. Open the Jupyter Notebook `RAG-Business.ipynb`.
2. Follow the instructions in the notebook to load the model and run the classification and retrieval process.
3. Input your query and observe the system classify and process it.

## Contributing

Contributions are welcome! Please fork this repository and submit a pull request for any features, bug fixes, or enhancements.

## License

This project is licensed under the MIT License. See the `LICENSE` file for more details.

