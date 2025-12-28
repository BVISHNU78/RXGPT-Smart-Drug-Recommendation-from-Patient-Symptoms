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
## 🌸 BLOOM Large Language Model Details

RxGPT is built using the **BLOOM (BigScience Large Open-science Open-access Multilingual) Large Language Model**, an open-source transformer-based model designed for large-scale natural language understanding.

### 🔹 Model Overview
- **Model Family:** BLOOM
- **Architecture:** Decoder-only Transformer
- **Training Organization:** BigScience Workshop
- **Open-Source:** Yes
- **Multilingual Support:** Yes
- **Domain Flexibility:** General-purpose with strong semantic understanding

### 🔹 Why BLOOM for RxGPT?
BLOOM was selected for the following reasons:

- Strong ability to understand **long-form and unstructured clinical text**
- Open-source and transparent, suitable for research and enterprise use
- Capable of capturing **contextual relationships between symptoms**
- Scalable architecture for backend and service-level integration
- Aligns with **responsible AI and ethical deployment** standards

### 🔹 Role of BLOOM in RxGPT
In RxGPT, BLOOM is used to:
- Encode patient symptom descriptions into semantic representations
- Capture contextual meaning beyond keyword matching
- Support disease likelihood estimation
- Enable intelligent drug recommendation mapping

BLOOM serves as the **core reasoning engine** of the system, enabling natural language understanding in the medical symptom domain.

### 🔹 Deployment Considerations
- BLOOM models are resource-intensive
- CPU inference is supported but slow
- GPU with sufficient VRAM is recommended for production usage
- Model size can be adjusted based on hardware availability

---

Official Model Pages

Hugging Face – BLOOM Model Page (main repository with weights & docs)
👉 https://huggingface.co/bigscience/bloom
 
Hugging Face

Hugging Face – Smaller version (560M) (good for local testing/dev)
👉 https://huggingface.co/bigscience/bloom-560m
 
Hugging Face

📚 Documentation Links

Transformers Library Documentation (BLOOM section)
👉 https://huggingface.co/docs/transformers/en/model_doc/bloom
 
Hugging Face

BigScience Project Homepage (BLOOM research initiative)
👉 https://bigscience.huggingface.co/blog/bloom


## 📌 Upcoming Actions

The following enhancements are planned to evolve RxGPT into a more robust and production-ready clinical decision support system:

### 🔹 Model & AI Improvements
- Fine-tune BLOOM on domain-specific clinical and symptom datasets
- Improve disease probability calibration and confidence estimation
- Introduce prompt optimization and structured inference strategies
- Evaluate lightweight BLOOM variants for faster inference

### 🔹 Data & Knowledge Expansion
- Expand disease–drug mapping coverage
- Add support for multi-symptom and comorbidity scenarios
- Incorporate structured medical knowledge bases
- Improve handling of ambiguous or incomplete symptom descriptions

### 🔹 System & Engineering Enhancements
- Expose the inference pipeline via a secure REST API
- Add logging and monitoring for model inference
- Optimize memory usage and inference latency
- Implement batch inference support

### 🔹 Safety, Validation & Compliance
- Add drug–drug interaction and contraindication checks
- Introduce confidence thresholds and uncertainty handling
- Validate outputs with clinical guidelines
- Prepare for regulatory and compliance considerations

### 🔹 Deployment & Scalability
- Containerize the system for reproducible deployment
- Support GPU and CPU inference configurations
- Enable horizontal scaling for high-throughput use cases
- Prepare cloud deployment pipelines

