# 🤖 BotTrainer – LLM-Based NLU Testing & Evaluation Platform

An interactive **Natural Language Understanding (NLU) testing platform** built using **Streamlit** that allows users to analyze chatbot intents, extract entities, and evaluate model performance using a **local LLM (Gemma-3) powered by Ollama**.

---

## 👨‍💻 Author
**Kowshika Suresh**

---

## 🧠 Project Overview

BotTrainer simulates a **chatbot Natural Language Understanding (NLU) system** where user messages are analyzed to determine the **intent** and **entities** in real time.

### Example Input
```
I need to book rooms in Delhi tomorrow
```

### Example Output
```json
{
  "intent": "book_hotel",
  "entities": {
    "location": "Delhi",
    "date": "tomorrow"
  },
  "confidence": 0.94
}
```

The platform helps developers **test chatbot understanding capabilities** and **evaluate intent classification accuracy**.

---

## 🚀 Key Features

- 🎯 Real-time **Intent Classification**
- 🧩 **Entity Extraction** from user messages
- 🖥 Interactive **NLU Testing Interface**
- 📊 **Model Evaluation Dashboard**
- 🔀 **Confusion Matrix Visualization**
- 📋 Detailed **Prediction Analysis Table**
- 📁 **Dataset Insights and Overview**
- ⚡ Local LLM inference using **Ollama + Gemma-3**

---

## 🏗️ System Architecture

```
User Message
     ↓
Streamlit Interface
     ↓
Gemma-3 Model (Local via Ollama)
     ↓
Intent Classification
     ↓
Entity Extraction
     ↓
Prediction Result
     ↓
Evaluation Metrics & Visualization
```

---

## ScreenShots:


## 🖥️ Application Interface

### 🧪 NLU Tester

Users can input any message to test **intent detection and entity extraction** in real time.

**Example Input**

```
I need to book rooms in Delhi tomorrow
```

**Output**

Intent → `book_hotel`

Entities:

- location → Delhi  
- date → tomorrow  

---

### 📊 Model Evaluation

The evaluation module measures the model's performance using standard machine learning metrics.

**Metrics Included**

- Accuracy
- Precision
- Recall
- F1 Score

**Example Result**

```
Accuracy  : 100%
Precision : 100%
Recall    : 100%
F1 Score  : 100%
```

The system also displays a **Confusion Matrix** to visualize predicted vs actual intents.

---

### 📋 Detailed Predictions

Displays dataset predictions including:

- Input text
- True intent
- Predicted intent
- Prediction correctness

**Example Dataset**

| Text | True Intent | Predicted Intent |
|-----|-----|-----|
| Available balance | bank_balance | bank_balance |
| Get me breakfast | order_food | order_food |
| Book airfare to Hyderabad | book_flight | book_flight |
| Weather report for Kochi | check_weather | check_weather |

---

## 📦 Tech Stack

| Component | Technology |
|---|---|
| Programming Language | Python |
| UI Framework | Streamlit |
| LLM Model | Gemma-3 |
| Inference Engine | Ollama |
| Data Processing | Pandas |
| Model Evaluation | Scikit-learn |
| Visualization | Plotly / Matplotlib |

---

## 🗂️ Project Structure

```
BotTrainer/
              
├── Milestone.ipynb      # Development notebook
├── requirements.txt     # Project dependencies
└── README.md
```

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/yourusername/bottrainer.git
cd bottrainer
```

### 2️⃣ Create Virtual Environment

```bash
python -m venv venv
```

Activate environment:

**Windows**

```bash
venv\Scripts\activate
```

**Mac/Linux**

```bash
source venv/bin/activate
```

---

### 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

---

### 4️⃣ Install Ollama

Download Ollama from:

https://ollama.com

Pull the **Gemma-3 model**

```bash
ollama pull gemma:3
```

---

### 5️⃣ Run the Application

```bash
streamlit run app.py
```

Open in browser:

```
http://localhost:8501
```

---

## 📊 Supported Intents

| Intent | Example |
|---|---|
| bank_balance | "Check my account balance" |
| book_flight | "Book flight to Hyderabad" |
| book_hotel | "Reserve a hotel in Delhi" |
| check_weather | "Will it rain in Mumbai?" |
| order_food | "Order pizza" |
| track_order | "Where is my order?" |

---

## 🎓 Learning Outcomes

Through this project you will learn:

- Building **NLU systems for chatbots**
- Implementing **Intent Classification**
- Performing **Entity Extraction**
- Running **LLMs locally with Ollama**
- Creating **interactive ML dashboards**
- Evaluating models using **confusion matrices**

---

## ❤️ Acknowledgement

Built with ❤️ using:

- **Python**
- **Streamlit**
- **Ollama**
- **Gemma-3**
