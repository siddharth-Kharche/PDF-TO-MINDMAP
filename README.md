Here is a sample `README.md` for your project:

---

# SID.AI PDF to Interactive Mindmap Converter

This is a Streamlit-based application that allows users to upload a PDF file, extract its text content, and generate a hierarchical mindmap in Markdown format. The app uses Google Gemini AI (Generative AI) to analyze the content and create an organized mindmap that visually represents the main topics, subtopics, and details from the document.

## Features

- **PDF Upload**: Upload your PDF file to extract its text content.
- **Text Extraction**: The app extracts readable text from the uploaded PDF file.
- **Mindmap Generation**: Uses Google Gemini AI to create a hierarchical mindmap in Markdown format.
- **Interactive Mindmap**: Visualizes the mindmap in an interactive format using the Markmap library.
- **Markdown Export**: Allows users to download the generated mindmap in Markdown format.

## Installation

To run the app locally, follow the instructions below:

### Prerequisites

- Python 3.7+
- Streamlit
- PyPDF2
- Google Generative AI (Gemini)

### Step 1: Clone this repository

```bash
git clone https://github.com/yourusername/sid-ai-pdf-mindmap.git
cd sid-ai-pdf-mindmap
```

### Step 2: Install required libraries

```bash
pip install -r requirements.txt
```

### Step 3: Set up Google API Key

You need to provide your own Google API key to interact with Google Gemini AI (Generative AI). Replace the placeholder API key in the code with your valid API key:

```python
API_KEY = "YOUR_GOOGLE_API_KEY"
```

### Step 4: Run the app

```bash
streamlit run app.py
```

The app will open in your default browser at `http://localhost:8501`.

## How It Works

1. **Configure Google Gemini AI**: The app configures Gemini AI using the provided API key to interact with the Generative model for text analysis.
2. **Text Extraction**: The PDF text is extracted using the `PyPDF2` library. The app reads each page and collects the text.
3. **Mindmap Generation**: Using the extracted text, the app generates a hierarchical markdown mindmap. The mindmap organizes the content into main topics, subtopics, and details, making it easy to understand the structure of the document.
4. **Interactive Visualization**: The generated markdown mindmap is rendered using Markmap, an interactive mindmap visualization tool.
5. **Markdown Export**: Users can download the mindmap as a `.md` file for further use or reference.

## Usage

1. **Upload PDF**: Click on the "Choose a PDF file" button to upload your PDF file.
2. **Processing**: The app will extract text from the PDF and generate the mindmap.
3. **View Mindmap**: The mindmap will be displayed in an interactive format, and you can explore its structure.
4. **View Markdown**: You can also view the generated Markdown code and download it for later use.

## File Structure

```
sid-ai-pdf-mindmap/
│
├── app.py                  # Main Streamlit app file
├── requirements.txt        # List of dependencies
├── README.md               # Project documentation
└── assets/                 # (Optional) Folder for assets, images, etc.
```

## Technologies Used

- **Streamlit**: Framework for creating interactive web apps.
- **Google Gemini AI**: Generative AI model for text analysis and mindmap creation.
- **PyPDF2**: Library for extracting text from PDF files.
- **Markmap**: Library for visualizing mindmaps in the browser using D3.js.
- **Python**: Programming language used to build the app.

## License

This project is licensed under the MIT License.

---

Make sure to replace `"YOUR_GOOGLE_API_KEY"` with your actual Google API key to enable the app functionality.
