# Fake News Detection Flask App

This repository contains a Flask-based web application for detecting fake news using machine learning and natural language processing (NLP). The application is designed to analyze a text input and classify it as real or fake news.

---

## Features

- **User-Friendly Interface**: A clean and interactive web interface built with Flask.
- **Natural Language Processing (NLP)**: Utilizes NLTK for text preprocessing and lemmatization.
- **Machine Learning Model**: Predicts whether the input text is real or fake news.
- **REST API**: Exposes endpoints for making predictions programmatically.

---

## Technologies Used

- Python 3.x
- Flask
- NLTK (Natural Language Toolkit)
- scikit-learn
- HTML, CSS

---

## Prerequisites

Make sure you have the following installed:

- Python 3.11.4
- pip (Python package manager)

---

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/fake-news-detection.git
   cd fake-news-detection
   ```

2. Create and activate a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate   # For Linux/macOS
   venv\Scripts\activate     # For Windows
   ```

3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Download the NLTK resource (`wordnet`):
   ```python
   import nltk
   nltk.download('wordnet')
   ```

---

## Usage

1. Run the Flask app:
   ```bash
   python app.py
   ```

2. Open your browser and go to:
   ```
   http://127.0.0.1:5000
   ```

3. Input text into the provided field and click "Predict" to classify the text as real or fake news.

---

## API Endpoints

### 1. `/predict` (POST)
**Description**: Takes a JSON payload with a text input and returns the prediction.

**Request Format**:
```json
{
  "text": "Sample news text here."
}
```

**Response Format**:
```json
{
  "prediction": "Fake"
}
```

---

## Project Structure

```
.
├── app.py                  # Main Flask application
├── templates/              # HTML templates
│   └── index.html          # Main UI template
├── static/                 # Static files (CSS, images, etc.)
│   └── hero_img.svg
├── requirements.txt        # Project dependencies
└── README.md               # Project documentation
```

---

## Notes

- Ensure `wordnet` and other NLTK resources are downloaded before running the app.
- This app is for educational purposes and may require further enhancements for production use.

---

## Contribution

Feel free to fork the repository and submit pull requests for improvements.

---

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.
