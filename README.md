# Mental Health Chatbot 🤖

## Overview
This project is a compassionate mental health chatbot designed to assist users with general mental well-being support. It leverages advanced language models to provide thoughtful responses and creates a vector database for efficient document retrieval. The chatbot is accessible through an interactive web interface built using [Gradio](https://gradio.app/).

---

## Features
- **Language Model**: Utilizes the `ChatGroq` LLM for generating thoughtful responses.
- **Document Retrieval**: Loads PDF documents, splits text into manageable chunks, and creates a vector database for retrieval using Chroma.
- **Compassionate Chatbot**: Tailored to respond with empathy and understanding, focused on mental well-being.
- **Web Interface**: Built using Gradio for easy interaction.
- **Persistent Database**: Saves and reuses vector embeddings for efficient querying.

---

## Tech Stack
- **Programming Language**: Python
- **Frameworks and Libraries**:
  - [LangChain](https://langchain.com/): For LLM operations, prompt templates, and QA chain setup.
  - [Gradio](https://gradio.app/): For creating the chatbot interface.
  - [HuggingFace Transformers](https://huggingface.co/): For embeddings.
  - [Chroma](https://www.trychroma.com/): For vector database.
  - [PyPDF](https://pypi.org/project/pypdf/): For PDF document processing.

---

## Setup Instructions

### Prerequisites
- Python 3.9 or later
- Google Colab or a local Python environment

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/mental-health-chatbot.git
   cd mental-health-chatbot
   ```

2. Install dependencies:
   ```bash
   pip install langchain_groq langchain_core langchain_community sentence_transformers chromadb pypdf gradio
   ```

### Running the Chatbot
1. Ensure your PDF documents are placed in the `/content/data` directory.
2. Run the script:
   ```bash
   python chatbot.py
   ```
3. Access the Gradio interface at the URL displayed in the terminal.

### Google Colab
Alternatively, you can run this project directly on Google Colab:
- Upload the project files.
- Execute the script cells sequentially.

---

## Project Structure
```
mental-health-chatbot/
├── chatbot.py                # Main script for chatbot setup
├── README.md                 # Project documentation
├── requirements.txt          # List of dependencies
├── /content/sample_data/data # Directory for PDF files
└── chroma_db/                # Persistent Chroma vector database
```

---

## Example Interaction
```
Human: What should I do if I feel overwhelmed?
Chatbot: It's okay to feel overwhelmed sometimes. Consider taking a deep breath, reaching out to someone you trust, or practicing mindfulness. Remember, you're not alone.
```

---

## Notes
- **Important**: This chatbot is for general mental health support and should not replace professional help. For serious concerns, please consult a licensed professional.
- To reset the database, delete the `/content/chroma_db` directory and rerun the script.

---

## Future Enhancements
- Add support for multi-lingual responses.
- Include more advanced analytics for chatbot interaction.
- Enhance the visual design of the Gradio interface.

---

## License
This project is licensed under the [MIT License](LICENSE).

---

## Acknowledgements
- [LangChain](https://langchain.com/)
- [HuggingFace](https://huggingface.co/)
- [Chroma](https://www.trychroma.com/)
- [Gradio](https://gradio.app/)
