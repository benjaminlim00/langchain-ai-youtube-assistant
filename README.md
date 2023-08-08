# LangChain YouTube Assistant

The LangChain YouTube Assistant is a Python script that utilizes various language processing and AI techniques to extract information and answer questions based on the transcript of a YouTube video. This script integrates with the LangChain library to handle document loading, text processing, embeddings, vector stores, chat models, and more.

## Installation

1. Clone the repository to your local machine.
2. Install the required dependencies by running:

```bash
pip install -r requirements.txt
```

## Usage

1. Ensure you have a valid YouTube video URL that you want to analyze.
2. Run the script:
   `python youtube_llm.py`

3. Follow the prompts to provide the YouTube video URL and your question.

## Features

The LangChain YouTube Assistant script demonstrates the following key features:

### 1. Document Loading

The script uses the `YoutubeLoader` class from the LangChain library to load the transcript of the provided YouTube video URL.

### 2. Text Splitting

The transcript is split into smaller chunks using the `RecursiveCharacterTextSplitter` to facilitate processing and analysis.

### 3. Embeddings

The script leverages OpenAI's embeddings to create embeddings for the text chunks obtained from the transcript.

### 4. Vector Store

The FAISS vector store is used to efficiently index and search through the embeddings of text chunks.

### 5. Chat Models

The LangChain `ChatOpenAI` model is utilized for generating responses based on user queries.

### 6. Language Model Chaining

The `LLMChain` class enables the chaining of language models and prompts for a coherent conversational flow.

### 7. User Interaction

The script interacts with the user by prompting for the YouTube video URL and the user's question. It then provides a detailed response based on the transcript.

## Example

Here's an example of how to use the LangChain YouTube Assistant script:

1. Run the script as mentioned above.
2. Provide the URL of the YouTube video you want to analyze.
3. Enter your question related to the video.
4. The script will process the transcript, generate a response, and display it to you.

## Notes

- Ensure you have the necessary API keys or environment variables set up as required by the LangChain library.
- The script currently uses the `gpt-3.5-turbo` model for generating responses. You can modify the model name as needed.

## License

This project is licensed under the [MIT License](LICENSE).
