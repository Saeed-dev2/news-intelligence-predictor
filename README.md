# 🧠 News Intelligence Predictor

**News Intelligence Predictor** is a web-based machine learning application built with **FastAPI** that classifies the genre or category of news based on the headline and article content. It uses Natural Language Processing (NLP) and a trained ML model to identify patterns and make predictions in real-time.
---

## 🚀 Features

- 📰 Input: News headline + article text
- 📊 Output: Predicted genre/category
- 🤖 ML model trained using scikit-learn and vectorized text
- ⚡ FastAPI backend with Jinja2 templating
- 🌐 Web UI for interactive input
- 🧰 Model and vectorizer serialized with `joblib`

---

## 📁 Project Structure

```
.
├── main.py                # FastAPI backend
├── model.pkl              # Trained ML model (binary)
├── vectorizer.pkl         # Fitted vectorizer (binary)
├── templates/
│   └── index.html         # Web interface
├── static/                # Static CSS/JS assets (optional)
└── train_model.py         # Script to train and save model/vectorizer
```
---

## ⚙️ Installation

1. **Clone the repository**:

```bash
git clone https://github.com/your-username/news-intelligence-predictor.git
cd news-intelligence-predictor
```

2. **Create a virtual environment**:

```bash
python -m venv venv
source venv/bin/activate  # or venv\Scripts\activate on Windows
```

3. **Install dependencies**:

```bash
pip install -r requirements.txt
```


4. **Train the model** (if `model.pkl` or `vectorizer.pkl` is missing):

```bash
python train_model.py
```

5. **Run the FastAPI app**:

```bash
uvicorn main:app --reload
```

6. **Visit the app** at:

```
http://127.0.0.1:8000/
```

---

## 🖼️ Web Interface

Submit a headline and an article through the input form to receive an instant genre prediction.

---

## 🧪 Example

Input:
- **Headline**: "Government unveils new economic reforms"
- **Article**: "The finance ministry has announced a new set of policies..."

Output:
- **Prediction**: `Politics` *(for example)*

---

## 📝 License

This project is licensed under the [MIT License](LICENSE.md).

---

## 🤝 Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

---

## 👨‍💻 Author

**Muhammad Saeed**  
AI & Data Science Enthusiast  
