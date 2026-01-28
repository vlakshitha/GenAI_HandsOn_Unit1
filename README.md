# Unit 1: Generative AI & NLP Fundamentals

## 🎯 Overview
Interactive hands-on notebook (PES2UG23CS665.ipynb) covering Transformer architectures, Hugging Face pipelines, and NLP tasks. Follows the 4-phase structure: Theory → Practice → Assessment → Application.

**Course Context:** PES University GenAI Hands-on Unit 1. Builds foundational skills for LLMs, tokenization, and domain-specific models like FinBERT.

## 📋 Phases Completed

### Phase 1: Theory
- Definitions: AI/ML/DL, LLM history (GPT-1 to GPT-4)
- Transformers: Encoder/decoder, attention mechanism

### Phase 2: Hands-On Practice
Hands-on with pipelines:
- Text Generation: distilgpt2 (fast) vs gpt2 (smart)
- Tokenization, POS tagging (NLTK), NER (`dbmdz/bert-large-cased-finetuned-conll03-english`)
- Summarization: distilbart vs bart-large-cnn

**Key Output Example:**
```
Generative AI is a revolutionary technology that allows users to build AI...
```
(gpt2 stays on-topic; distilgpt2 drifts)

### Phase 3: Assessment
Architecture benchmark table (update in `Unit1Benchmark.ipynb`):

| Task      | BERT | RoBERTa | BART   | Reason              |
|-----------|------|---------|--------|---------------------|
| Text Gen | FAIL | FAIL   | SUCCESS| Decoder required   |
| Fill-Mask| ✓    | ✓      | ~      | MLM vs denoising   |
| QA       | ~    | ~      | ~      | Needs fine-tuning  | 

### Phase 4: Mini-Project
**Financial Sentiment Analyzer** (FinBERT on Indian/US market headlines):
```
Fed rate hike 50bps: neutral (80.7%)
Nifty hits 25k ATH: positive (61.9%)
```
