# Hey, I'm Krish 👋
I build LLM and ML systems that solve real business problems — transformer sprint complete
(fine-tuning, QA, summarization) and now heading into prompt engineering, RAG pipelines,
and AI support tools for SaaS companies.

---

## What I've built

| Project | What it does | Key result |
|---|---|---|
| [qa-summarizer-app](https://github.com/codewith-krishh/qa-summarizer-app) | Two-tab Streamlit app: document summarizer (BART-large-CNN) + extractive QA (RoBERTa-base-SQuAD2); both loaded via HuggingFace `pipeline()` with `@st.cache_resource`; QA tab handles unanswerable questions correctly — returns empty span with low confidence rather than hallucinating | Chose extractive over generative QA for zero hallucination risk; proof-of-concept for the Employee Handbook Chatbot inference layer before adding a vector DB |
| [bert-sentiment-app](https://github.com/codewith-krishh/bert-sentiment-app) | Fine-tuned bert-base-uncased on 25k IMDb reviews using HuggingFace Trainer API (TrainingArguments, DataCollatorWithPadding, compute_metrics); checkpoint scoped for 4GB VRAM | Production-ready binary sentiment classifier — exposed a WordPiece tokenization failure on SaaS domain text that a generic model misses entirely |
| [ResNet-18-image-classifier](https://github.com/codewith-krishh/ResNet-18-image-classifier) | Transfer learning pipeline fine-tuned on cats vs. dogs using PyTorch + ResNet-18; Streamlit UI for live predictions with confidence scores | 98.14% validation accuracy in 5 epochs |
| [pytorch-text-classifier](https://github.com/codewith-krishh/pytorch-text-classifier) | Neural text classifier (nn.Embedding → mean pooling → BCEWithLogitsLoss) benchmarked head-to-head against the TF-IDF baseline on the same dataset | Diagnosed 87% class imbalance as root cause of recall collapse — a stronger portfolio signal than a clean result |
| [Customer-Churn-prediction](https://github.com/codewith-krishh/Customer-Churn-prediction) | End-to-end churn model on Telco dataset using sklearn Pipelines, class-weight balancing, and GridSearchCV | 78% recall on churners — optimised to catch at-risk customers, not just overall accuracy |

---

## Current stack

**LLMs / Transformers** — BERT fine-tuning · BART (abstractive summarization) · RoBERTa (extractive QA) · T5 architecture · GPT-2 architecture · HuggingFace Transformers · Trainer API · AutoModel · AutoTokenizer · `pipeline()` · BPE / WordPiece tokenization  
**ML / DL** — PyTorch · CNNs · ResNet-18 · Transfer Learning · Neural Networks · scikit-learn · Logistic Regression · Pipelines · GridSearchCV  
**NLP** — extractive QA · abstractive summarization · TF-IDF · Multinomial Naive Bayes · text preprocessing · Word2Vec (concepts)  
**Data** — pandas · NumPy · Matplotlib · Seaborn  
**Deploy** — Streamlit · Streamlit Cloud · Google Colab (T4 GPU) · CUDA · Git · GitHub  

---

## What I'm working toward

Weeks 20–22 transformer sprint complete — built attention from scratch, fine-tuned BERT,
deployed a two-pipeline QA + summarization app.

Next: Weeks 23–26 — prompt engineering. OpenAI + Claude API, chain-of-thought prompting,
system prompt design, and the first deployed LLM tools with real business logic.

After that: production RAG pipelines, vector databases, and client-ready AI support
chatbots for SaaS companies. First client-ready demo targeted for Month 9.

---

## Let's connect

[LinkedIn](https://linkedin.com/in/krish-manji011) · [X / Twitter](https://x.com/Born_TechK)
