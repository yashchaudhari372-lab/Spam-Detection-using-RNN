# Spam Detection Using RNN | Deep Learning & NLP

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![TensorFlow](https://img.shields.io/badge/TensorFlow-Keras-orange?logo=tensorflow)
![NLP](https://img.shields.io/badge/NLP-Text%20Classification-purple)
![Status](https://img.shields.io/badge/Project-Live-brightgreen)

An end-to-end **spam message classification** project using **Natural Language Processing (NLP)** and a **Recurrent Neural Network (RNN)**. The application accepts a text message and predicts whether it is **Spam** or **Not Spam (Ham)** using a trained Keras model.

**[🚀 Try the Live Demo](https://spam-not-spam-detection-by-rnn-g96x9yxtjkuhxtdabkgvyc.streamlit.app/)** · **[💻 View Repository](https://github.com/yashchaudhari372-lab/Spam-Detection-using-RNN)**

## Project Overview

Unwanted promotional messages, phishing attempts, and unsolicited communication can make messaging platforms difficult to use. This project demonstrates how deep learning can assist with automated spam filtering by learning patterns from labeled text messages.

The saved model and preprocessing artifacts are packaged with an application so users can test new messages through a web interface.

## Key Features

- Classifies user-entered messages as **Spam** or **Not Spam**.
- Uses an **RNN-based Keras model** for sequence classification.
- Reuses the saved tokenizer and label encoder for inference.
- Provides an interactive web application.
- Includes trained-model artifacts in the repository.

## Tech Stack

| Area | Technology |
| --- | --- |
| Programming | Python |
| Deep learning | TensorFlow / Keras |
| NLP | Tokenization and text-to-sequence conversion |
| Model | Recurrent Neural Network (RNN) |
| Saved artifacts | `.keras` and `.pkl` files |
| Application | Python web interface (`app.py`) |
| Deployment | Streamlit Community Cloud (live demo URL) |

## How It Works

```text
Input Message
     ↓
Text Preprocessing / Tokenization
     ↓
Sequence Conversion and Padding
     ↓
Trained RNN Model
     ↓
Prediction / Label Decoding
     ↓
Spam or Not Spam
```

The inference application loads the trained model and the saved preprocessing artifacts to keep incoming text compatible with the model's expected input.

## Repository Structure

```text
Spam-Detection-using-RNN/
├── app.py                # Web application and inference logic
├── spam_rnn.keras        # Trained RNN model
├── tokenizer.pkl         # Saved text tokenizer
├── label_encoder.pkl     # Saved target-label encoder
├── model_config.pkl      # Saved model configuration
├── requirements.txt      # Python dependencies
└── README.md             # Project documentation
```

## Run Locally

**1. Clone the repository**

```bash
git clone https://github.com/yashchaudhari372-lab/Spam-Detection-using-RNN.git
cd Spam-Detection-using-RNN
```

**2. Create and activate a virtual environment (recommended)**

```bash
python -m venv .venv
```

Windows:

```bash
.venv\Scripts\activate
```

macOS / Linux:

```bash
source .venv/bin/activate
```

**3. Install dependencies**

```bash
pip install -r requirements.txt
```

**4. Start the application**

```bash
streamlit run app.py
```

> The hosted demo uses a Streamlit URL. If your current `app.py` uses another web framework, start it with that framework's command instead (for example, `python app.py` for a Flask entry point).

## Example Usage

Enter a message such as:

> Congratulations! You have won a free prize. Claim it now!

The application processes the text and returns a predicted class. Predictions are model-generated and may be incorrect, especially for unfamiliar messages.

## Model Evaluation

The repository includes a saved trained model, but **verified evaluation metrics are not documented here**. To make the project more compelling, add results from your held-out test set:

| Metric | Result |
| --- | --- |
| Accuracy | Add verified result |
| Precision | Add verified result |
| Recall | Add verified result |
| F1-score | Add verified result |

Consider adding a confusion matrix and classification report screenshot to an `assets/` folder and linking them here.

## Applications

- SMS and email spam filtering
- Automated message moderation
- Suspicious-message triage
- NLP and deep learning demonstrations

## Limitations and Future Improvements

- Model predictions do not guarantee that a message is safe or malicious.
- Test robustness against misspellings, multilingual messages, and adversarial wording.
- Compare RNN performance with LSTM, GRU, and transformer baselines.
- Add reproducible training notebooks, dataset attribution, and test-set metrics.
- Add unit tests and deployment health checks.

## Author

**Yash Chaudhari**  
Aspiring Data Scientist & Data Analyst

- [GitHub](https://github.com/yashchaudhari372-lab)
- [LinkedIn](https://www.linkedin.com/in/yashchaudhari08/)

---

If this project helped you, consider giving the repository a ⭐.
