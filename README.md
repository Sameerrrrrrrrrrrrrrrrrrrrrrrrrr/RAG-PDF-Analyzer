# RAG-PDF-Analyzer
Author Sameer Mankar

RAG-PDF-Analyzer is a simple resume analysis tool that extracts, analyzes, and evaluates resumes using Retrieval-Augmented Generation (RAG) and Large Language Models (LLMs). It provides HR-friendly assessments and allows users to ask questions about a candidate's resume interactively.

## Features
- Extracts text from PDF resumes.
- Uses RAG (Retrieval-Augmented Generation) for resume analysis.
- Categorizes skills into predefined groups such as programming, machine learning, and data visualization.
- Calculates years of experience from job history.
- Provides an AI-generated HR assessment.
- Streamlit-based web UI for easy resume uploads and analysis.
- Interactive Q&A about resumes.

## Installation
### Prerequisites
- Python 3.8+
- Pip
- Virtual environment (recommended)

### Setup
1. Clone the repository:
   ```sh
   git clone https://github.com/your-repo-name/ai-resume-analyzer.git
   cd ai-resume-analyzer
   ```
2. Create a virtual environment (optional but recommended):
   ```sh
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```
3. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```

## Usage
### Command Line Mode
Run the resume analyzer directly from the terminal:
```sh
python AN.py
```
Follow the prompts to provide the resume file path and interact with the system.

### Web App Mode
To launch the Streamlit-based web interface:
```sh
streamlit run app.py
```
Upload a PDF resume and receive an AI-generated assessment.

## Environment Variables
This project requires an API key for Groq’s LLM services. Set up the environment variable:
```sh
export GROQ_API_KEY="your_api_key_here"
```
On Windows:
```sh
set GROQ_API_KEY="your_api_key_here"
```

## File Structure
```
.
├── AN.py               # Backend resume analysis logic
├── app.py              # Streamlit-based frontend UI
├── requirements.txt    # Required dependencies
├── README.md           # Project documentation
```

## Dependencies
- `streamlit` for the UI
- `PyMuPDF` for PDF text extraction
- `langchain` and `FAISS` for RAG-based resume processing
- `sentence-transformers` for embeddings

## Contribution
Feel free to submit issues or pull requests! Contributions are always welcome.

## License
This project is licensed under the MIT License.

