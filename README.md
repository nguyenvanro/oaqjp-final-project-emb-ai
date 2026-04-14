# Final Project: AI-Based Emotion Detection Web Application

## Project Overview

This repository contains the **Final Project** for the Coursera course **"AI-Based Natural Language Processing (NLP) with Embedded AI"**. The project demonstrates the development of an Emotion Detection application using IBM Watson NLP libraries and a Flask-based web server.

## Project Name

**Final Project** — NLP Emotion Detection using Embedded AI

## Description

The Emotion Detection application analyzes text input provided by the user and identifies the dominant emotions expressed in the text. It leverages IBM Watson's Embedded AI (NLP) library to perform emotion analysis and returns scores for the following emotions:

- **Anger**
- **Disgust**
- **Fear**
- **Joy**
- **Sadness**

The application also identifies and returns the **dominant emotion** — the one with the highest score.

## Project Structure

```
oaqjp-final-project-emb-ai/
├── README.md                    # Project documentation
├── LICENSE                      # License file
├── server.py                    # Flask web server
├── EmotionDetection/
│   ├── __init__.py              # Package initializer
│   └── emotion_detection.py     # Core emotion detection logic
├── static/
│   └── mywebscript.js           # Frontend JavaScript for AJAX calls
├── templates/
│   └── index.html               # Main web UI template
└── test_emotion_detection.py    # Unit tests for emotion detection
```

## Features

- Accepts user text input via a web interface
- Calls IBM Watson NLP Embedded AI API for emotion analysis
- Displays emotion scores and the dominant emotion in the browser
- Handles blank/invalid input with appropriate error messages
- Fully unit-tested emotion detection logic
- PEP8-compliant Python code (score 10/10 via PyLint)

## Technologies Used

- **Python 3** — Backend logic
- **Flask** — Web framework for the server
- **IBM Watson NLP (Embedded AI)** — Emotion analysis API
- **HTML5 / Bootstrap 4** — Frontend UI
- **JavaScript (XMLHttpRequest)** — Asynchronous frontend requests

## How to Run

1. **Clone the repository:**
   ```bash
   git clone https://github.com/<your-username>/oaqjp-final-project-emb-ai.git
   cd oaqjp-final-project-emb-ai
   ```

2. **Install dependencies:**
   ```bash
   pip install flask requests
   ```

3. **Start the Flask server:**
   ```bash
   python server.py
   ```

4. **Open your browser and navigate to:**
   ```
   http://localhost:5000
   ```

## Usage

1. Enter the text you want to analyze in the input field.
2. Click the **"Run Sentiment Analysis"** button.
3. View the emotion scores and the dominant emotion in the **Result of Emotion Detection** section.

## Sample Output

For input text *"I am so happy I am doing this"*, the application returns:

```
For the given statement, the system response is
'anger': 0.006, 'disgust': 0.002, 'fear': 0.009, 'joy': 0.986, 'sadness': 0.016.
The dominant emotion is joy.
```

## Error Handling

If the text field is left blank, the application displays:
```
Invalid text! Please try again!
```

## Course Information

- **Course:** Developing AI Applications with Python and Flask (IBM / Coursera)
- **Assignment:** Final Project — Emotion Detection Web App using Embedded AI

## License

This project is licensed under the terms of the [LICENSE](LICENSE) file included in this repository.
