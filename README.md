# Hey, I'm Krish 👋
I build LLM and ML systems that solve real business problems. Wrapping up a 26-day Prompt
Engineering Sprint (Groq API, structured outputs, evaluation harnesses) after completing a
full transformer fine-tuning sprint — next up: production RAG pipelines and AI support tools
for SaaS companies.

Currently open to AI/ML internships to build experience and hands-on production reps.

---

## What I've built

| Project | What it does | Key result |
|---|---|---|
| [code-doc-generator](https://github.com/codewith-krishh/code-doc-generator) · [demo](https://code-doc-generator-26.streamlit.app/) | Two-stage LLM pipeline via Groq: function calling extracts code structure, then generates structured docstrings/comments from raw source; Pydantic schema validation with retry logic on malformed outputs | Turns an unreliable single-shot LLM call into a repeatable, schema-validated documentation tool — the core pattern behind the client-facing automation tools I'm building toward |
| [email-tone-rewriter](https://github.com/codewith-krishh/email-tone-rewriter) · [demo](https://email-tone-rewriter-2026.streamlit.app/) | Groq-powered tool that rewrites email drafts to a target tone using few-shot prompting; Pydantic retry logic catches and re-requests malformed model outputs | Proof-of-concept for reliable structured output from an LLM — no silent failures, no unvalidated JSON reaching the user |
| [email-intent-parser](https://github.com/codewith-krishh/email-intent-parser) · [demo](https://email-intent-parser-2026.streamlit.app/) | Groq-powered classifier that parses raw email text into a strict JSON schema (intent, urgency, key entities) via Pydantic-validated structured output | Early proof of the "unstructured text → reliable structured data" pattern — the same building block a support-ticket router or CRM auto-tagger would need |
| [qa-summarizer-app](https://github.com/codewith-krishh/qa-summarizer-app) · [demo](https://nlp-demo-app-distilbart.streamlit.app/) | Two-tab Streamlit app: document summarizer (BART-large-CNN) + extractive QA (RoBERTa-base-SQuAD2); both loaded via HuggingFace `pipeline()` with `@st.cache_resource`; QA tab handles unanswerable questions correctly — returns empty span with low confidence rather than hallucinating | Chose extractive over generative QA for zero hallucination risk; proof-of-concept for the Employee Handbook Chatbot inference layer before adding a vector DB |
| [bert-sentiment-app](https://github.com/codewith-krishh/bert-sentiment-app) · [demo](https://bert-sentiment-app-011.streamlit.app/) | Fine-tuned bert-base-uncased on 25k IMDb reviews using HuggingFace Trainer API (TrainingArguments, DataCollatorWithPadding, compute_metrics); checkpoint scoped for 4GB VRAM | Production-ready binary sentiment classifier — exposed a WordPiece tokenization failure on SaaS domain text that a generic model misses entirely |
| [ResNet-18-image-classifier](https://github.com/codewith-krishh/ResNet-18-image-classifier) · [demo](https://resnet-18-image-classifier-2026.streamlit.app/) | Transfer learning pipeline fine-tuned on cats vs. dogs using PyTorch + ResNet-18; Streamlit UI for live predictions with confidence scores | 98.14% validation accuracy in 5 epochs |
| [SMS-Spam-Classifier](https://github.com/codewith-krishh/SMS-Spam-Classifier) | PyTorch feedforward classifier benchmarked against a TF-IDF + Multinomial Naive Bayes baseline (98.48% accuracy, 0.94 F1 on spam class) | Diagnosed a recall collapse in the neural net caused by class imbalance and identified the fix (class-weighted loss) — documented as a portfolio case study |
| [Customer-Churn-prediction](https://github.com/codewith-krishh/Customer-Churn-prediction) | End-to-end churn model on Telco dataset using sklearn Pipelines, class-weight balancing, and GridSearchCV | 78% recall on churners — optimised to catch at-risk customers, not just overall accuracy |

---

## Current stack

**LLM Engineering** — Groq API (Llama models) · Prompt Engineering · Prompt Chaining · Few-shot Prompting · Structured Outputs (Pydantic) · Function Calling · LLM-as-Judge Evaluation

**LLMs / Transformers** — BERT fine-tuning · BART (abstractive summarization) · RoBERTa (extractive QA) · T5 architecture · GPT-2 architecture · HuggingFace Transformers · Trainer API · AutoModel · AutoTokenizer · `pipeline()` · BPE / WordPiece tokenization

**ML / DL** — PyTorch · CNNs · ResNet-18 · Transfer Learning · Neural Networks · scikit-learn · Logistic Regression · Pipelines · GridSearchCV

**NLP** — extractive QA · abstractive summarization · TF-IDF · Multinomial Naive Bayes · text preprocessing · Word2Vec (concepts)

**Data** — pandas · NumPy · Matplotlib · Seaborn

**Deploy** — Streamlit · Streamlit Cloud · Google Colab (T4 GPU) · CUDA · Git · GitHub

---

## What I'm working toward
Weeks 23–26 Prompt Engineering Sprint wrapping up — shipped Groq-powered tools with
structured outputs, retry logic, and an LLM-as-Judge evaluation harness for automated
output scoring.

Next: production RAG pipelines, vector databases, and client-ready AI support chatbots
for SaaS companies.

---

## Let's connect
[LinkedIn](https://linkedin.com/in/krish-manji011) · [X / Twitter](https://x.com/Born_TechK)
