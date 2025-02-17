# YouTube and Website Content Summarizer

A Streamlit application that uses LangChain and Hugging Face to automatically summarize content from YouTube videos (using transcripts) and websites.

## 🌟 Features

- Summarize content from YouTube videos using video transcripts
- Summarize content from any website
- Uses Hugging Face's Mistral-7B-Instruct-v0.3 model for summarization
- Clean and user-friendly Streamlit interface
- Automatic text chunking for processing long content
- Support for custom API keys

## 🛠️ Technologies Used

- Python 3.12
- Streamlit
- LangChain
- Hugging Face
- YouTube Transcript API
- RecursiveCharacterTextSplitter for text processing

## 📋 Prerequisites

Before running this application, make sure you have:

1. Python 3.12 or later installed
2. A Hugging Face API key
3. pip (Python package manager)

## 🔧 Installation

1. Clone this repository:
```bash
git clone https://github.com/yourusername/content-summarizer.git
cd content-summarizer
```

2. Install the required dependencies:
```bash
pip install -r requirements.txt
```

3. Create a `requirements.txt` file with the following dependencies:
```
streamlit
langchain
langchain-groq
langchain-core
langchain-community
langchain-huggingface
youtube-transcript-api
```

## 🚀 Usage

1. Start the Streamlit application:
```bash
streamlit run app.py
```

2. Open your web browser and navigate to the provided local URL (typically `http://localhost:8501`)

3. In the sidebar, enter your Hugging Face API key

4. Choose the source type (YouTube or Website)

5. Enter the URL of the content you want to summarize

6. Click the "Summarize" button and wait for the results

## 📝 Features Explanation

### YouTube Summarization
- Automatically extracts video ID from YouTube URLs
- Retrieves video transcripts using the YouTube Transcript API
- Supports both youtube.com and youtu.be URL formats

### Website Summarization
- Uses WebBaseLoader to extract content from websites
- Processes HTML content automatically

### Text Processing
- Splits long texts into manageable chunks
- Maintains context with chunk overlap
- Handles large documents efficiently

## ⚠️ Limitations

- YouTube videos must have English subtitles/transcripts available
- The summarization quality depends on the Hugging Face model used
- API rate limits may apply based on your Hugging Face account type

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Hugging Face for providing the language model
- Streamlit for the amazing web framework
- LangChain for the document processing capabilities
- YouTube Transcript API developers

## 📧 Contact

Your Name - [your.email@example.com](mailto:your.email@example.com)

Project Link: [https://github.com/yourusername/content-summarizer](https://github.com/yourusername/content-summarizer)
