# T5 Text Summarizer

## Overview

T5 Text Summarizer is a web-based application that generates concise summaries from lengthy text and dialogues using a fine-tuned T5-small transformer model. The model is trained on the SAMSum dataset to summarize conversational text.

The application uses FastAPI for the backend and HTML, CSS, and JavaScript for the user interface.

## Technologies Used

* Python
* PyTorch
* Hugging Face Transformers
* T5-small
* FastAPI
* HTML, CSS, and JavaScript
* SAMSum Dataset

## Features

* Automatic text summarization
* Dialogue summarization
* Simple and user-friendly interface
* FastAPI-based backend
* Local model inference

## Project Structure

```text
t5-text-summarizer/
├── app.py
├── index.html
├── saved_summary_model/
├── .gitignore
└── README.md
```

## Installation and Setup

**1. Clone the repository**

```bash
git clone https://github.com/saurabhdhule2005/t5-text-summarizer.git
cd t5-text-summarizer
```

**2. Install the required dependencies**

```bash
pip install fastapi uvicorn transformers torch sentencepiece jinja2
```

**3. Set up the trained model**

Place the trained model files in the `saved_summary_model/` directory. The application requires these files to run locally.

**4. Start the application**

```bash
python -m uvicorn app:app --reload
```

**5. Open the application**

Open the following URL in your browser:

http://127.0.0.1:8000

## How It Works

1. The user enters text or a dialogue.
2. The input is sent to the FastAPI backend.
3. The text is processed by the fine-tuned T5-small model.
4. The application generates and displays a concise summary.

## Model and Dataset

* **Model:** T5-small
* **Dataset:** SAMSum
* **Task:** Abstractive text summarization

## Future Scope

* Deploy the application online.
* Improve summarization quality through further training.
* Support longer documents.
* Enhance the user interface.

## Author

Saurabh Dhule

GitHub: https://github.com/saurabhdhule2005

