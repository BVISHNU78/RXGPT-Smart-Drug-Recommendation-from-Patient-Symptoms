# RXGPT-Smart-Drug-Recommendation-from-Patient-Symptoms

RxGPT is an **LLM-powered clinical decision support system** that analyzes **free-text patient symptom descriptions** and generates **context-aware, confidence-based drug recommendations**.  
The system is built using the **BLOOM Large Language Model**, enabling deep semantic understanding of clinical language and symptom patterns.

> ⚠️ **Important Notice:**  
> RxGPT is an assistive AI system and **does not replace licensed medical professionals**.  
> All outputs are intended for preliminary decision support and educational purposes only.

---

## 📌 Table of Contents

- Project Overview  
- Problem Statement  
- Solution Overview  
- Key Features  
- System Architecture  
- Technology Stack  
- Why BLOOM LLM  
- Installation & Setup  
- Usage  
- Model & Inference Pipeline  
- Explainability & Safety  
- Use Cases  
- Limitations  
- Future Enhancements  
- Ethical Considerations  
- Author  

---

## 📖 Project Overview

Healthcare data is predominantly unstructured, with patient symptoms often expressed in natural language.  
RxGPT leverages the **BLOOM Large Language Model** to interpret these descriptions and provide **structured, ranked drug recommendations** with associated confidence scores.

The project is designed as a **production-ready, modular clinical decision support system**, focusing on safety, explainability, and scalability.

---

## ❓ Problem Statement

- Patient symptoms are expressed in diverse natural language forms
- Traditional rule-based systems struggle with semantic variability
- Clinicians require assistive tools that provide confidence-aware insights
- Explainability and transparency are critical in healthcare AI systems

---

## 💡 Solution Overview

RxGPT addresses these challenges by:

- Using **BLOOM LLM** for contextual understanding of symptoms
- Mapping symptom embeddings to disease probabilities
- Recommending drugs associated with predicted conditions
- Providing structured outputs for human-in-the-loop validation

---

## 🚀 Key Features

- Natural language symptom analysis using BLOOM LLM  
- Disease prediction with probability estimation  
- Intelligent drug recommendation mapping  
- Explainable and interpretable outputs  
- Modular and scalable system design  
- Assistive clinical decision support focus  

---

## 🧠 System Architecture

Patient Symptoms (Text Input)
↓
Text Preprocessing & Tokenization
↓
BLOOM Large Language Model
↓
Disease Probability Estimation
↓
Drug Recommendation Engine
↓
Structured Clinical Output

yaml
Copy code

---

## 🛠️ Technology Stack

| Layer | Technology |
|------|-----------|
| Language Model | BLOOM Large Language Model |
| Backend | Python |
| ML Framework | PyTorch, Hugging Face Transformers |
| Data Processing | Pandas, NumPy |
| Deployment Ready | API / Service Integration |


## 🌸 Why BLOOM LLM?

BLOOM was selected for this project due to:

- **Strong multilingual and semantic understanding**
- **Open-source and transparent model architecture**
- **Ability to handle long-form clinical text**
- **Scalability for research and enterprise environments**
- **Alignment with responsible AI principles**

BLOOM’s architecture enables RxGPT to interpret complex symptom descriptions beyond keyword matching.

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/your-username/RxGPT.git
cd RxGPT

python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate

pip install -r requirements.txt

from rxgpt import diagnose

results = diagnose("fever, cough, body pain")
print(results)
