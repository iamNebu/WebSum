<div align="center">

# 📄 WebSum
### *RAG Intelligent Web Page Summarizer*

<p>
An intelligent web summarization application that extracts textual content from web pages and generates comprehensive, structured summaries using <b>Meta Llama 3 Instruct</b> running locally with <b>Ollama</b>.
</p>

![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-Web_App-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-AI_Framework-121212?style=for-the-badge)
![Ollama](https://img.shields.io/badge/Ollama-Llama3-blue?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-success?style=for-the-badge)

---

*A Sixth Semester Mini Project*

</div>

---

# 📖 Overview

**WebSum** is an RAG powered web content summarization tool that automatically extracts readable text from websites and converts lengthy articles into detailed, structured summaries.

Instead of manually reading long webpages, users simply enter a URL. The application downloads the webpage, removes HTML elements, processes the extracted text through **Meta's Llama 3 Instruct** model via **Ollama**, and generates a coherent summary that can also be exported as a PDF.

---

# ✨ Features

- 🌐 Automatic webpage content extraction
- 🤖 AI-powered summarization using Llama 3 Instruct
- 📑 Structured summaries with headings and subheadings
- ⚡ Local inference using Ollama
- 📄 Export summaries as PDF
- 🎨 Interactive Streamlit interface
- 🔍 HTML content cleaning using BeautifulSoup
- 📚 Chunk-based processing for lengthy webpages

---

# 🏗 System Architecture

```text
                 User
                   │
                   ▼
          Enter Website URL
                   │
                   ▼
         Fetch Webpage Content
             (Requests)
                   │
                   ▼
         HTML Content Cleaning
          (BeautifulSoup)
                   │
                   ▼
         Text Chunk Generation
                   │
                   ▼
      LangChain Prompt Template
                   │
                   ▼
      Meta Llama 3 Instruct
        (via Ollama)
                   │
                   ▼
       Intelligent Summary
                   │
         ┌─────────┴─────────┐
         ▼                   ▼
 Display in Streamlit    Export to PDF
```

---

# 🛠 Technologies Used

| Technology | Purpose |
|------------|----------|
| Python | Core Programming Language |
| Streamlit | Interactive Web Interface |
| LangChain | Prompt orchestration |
| Ollama | Local LLM Runtime |
| Meta Llama 3 Instruct | AI Summarization Model |
| BeautifulSoup | HTML Parsing |
| Requests | Webpage Retrieval |
| FPDF | PDF Generation |

---

# ⚙ Workflow

```text
User enters URL
       │
       ▼
Download webpage
       │
       ▼
Remove HTML tags
       │
       ▼
Extract readable text
       │
       ▼
Split into chunks
       │
       ▼
Generate summaries
       │
       ▼
Merge summaries
       │
       ▼
Display results
       │
       ▼
Download PDF
```

---

# 🖥 User Interface

The application is developed using **Streamlit**, providing a simple and intuitive interface.

## 📍 URL Input

Users provide the webpage URL to summarize.

---

## 🚀 Summarize Button

Initiates the complete summarization pipeline.

---

## ⏳ Processing Indicators

Displays progress while

- Fetching webpage
- Cleaning HTML
- Generating summaries

---

## 📄 Summary Viewer

Displays the generated structured summary.

Features include

- Headings
- Subheadings
- Paragraph formatting

---

## 📥 PDF Export

Allows users to download the generated summary as a PDF document.

---

# 🧠 AI Pipeline

```text
Web URL
   │
   ▼
HTML Extraction
   │
   ▼
Content Cleaning
   │
   ▼
Chunk Creation
   │
   ▼
Prompt Engineering
   │
   ▼
Llama 3 Instruct
   │
   ▼
Generated Summary
```

---

# 📂 Project Structure

```text
WebSum/
│
├── mini_project_s6_.py          # Main Streamlit application
├── requirements.txt             # Project dependencies
├── LICENSE
│
├── Model_details/
│   ├── Data_flow_diagram.png
│   ├── System_architecture_imgae.png
│   └── README.md
│
├── output_images/
│   ├── output_1.png
│   ├── Output_2.png
│   ├── out_put_3.png
│   └── output_4.png
│
├── Report_of_the_project/
│   ├── Websum_by_Nebu.pdf
│   └── README.md
│
└── README.md
```

---

# 📷 Application Preview

## Main Interface

> Add screenshots from the `output_images` folder here.

```text
📌 Homepage
📌 Generated Summary
📌 PDF Export
📌 AI Processing
```

---

# 🚀 Installation

Clone the repository

```bash
git clone https://github.com/iamNebu/WebSum.git
```

Navigate to the project

```bash
cd WebSum
```

Install dependencies

```bash
pip install -r requirements.txt
```

---

# 📦 Install Ollama

Download and install Ollama from

https://ollama.com

Pull the Llama 3 model

```powershell
ollama pull llama3:instruct
```

Start the Ollama server

```powershell
ollama serve
```

---

# ▶ Run the Application

```powershell
streamlit run mini_project_s6_.py
```

---

# 📚 How It Works

1. User enters a webpage URL.
2. Requests downloads the webpage.
3. BeautifulSoup extracts readable content.
4. Long text is divided into smaller chunks.
5. LangChain constructs prompts.
6. Llama 3 generates summaries for each chunk.
7. Summaries are merged into one final document.
8. The summary is displayed and can be downloaded as a PDF.

---

# 🌍 Applications

- Research Paper Summarization
- News Article Summaries
- Blog Summaries
- Educational Content
- Documentation Review
- Technical Articles
- Web Content Analysis

---

# 🔮 Future Improvements

- Multi-language summarization
- URL history
- AI-generated keywords
- Mind map generation
- Voice summaries
- Dark mode
- Browser extension
- Batch URL summarization
- Citation generation
- RAG-based knowledge enhancement

---

# 📊 Model Details

**Model**

- Meta Llama 3 Instruct

**Framework**

- LangChain

**Inference**

- Ollama (Local)

**Prompt Strategy**

- Structured summarization
- Heading generation
- Subheading generation
- Context preservation

---

# 📄 Output

The application generates

- Clean Summary
- Structured Sections
- Headings
- Subheadings
- Downloadable PDF

---

# 🤝 Contributing

Contributions are welcome.

1. Fork the repository
2. Create a new feature branch
3. Commit your changes
4. Push the branch
5. Open a Pull Request

---

# 👨‍💻 Author

**Nebu**

Sixth Semester Mini Project

---

# 📜 License

This project is licensed under the MIT License.

---

# 🙏 Acknowledgements

Special thanks to the open-source community behind

- Python
- Streamlit
- LangChain
- Ollama
- Meta AI
- BeautifulSoup
- Requests
- FPDF

for providing the tools that made this project possible.

---

<div align="center">

### ⭐ If you found this project useful, please consider giving it a Star!

</div>

