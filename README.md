# NLP-Based-Disaster-Info-Extraction-Summarization
NLP-based system for extracting disaster-related information and generating automated summaries from multi-source text data like social media and news. 
🌍 DisasterNLP: Intelligent Disaster Information Extraction & Summarization
🚀 Project Overview
This project implements a Natural Language Processing (NLP)-based intelligent system that extracts critical disaster-related information and generates automated summaries from multi-source text data such as Reddit and news feeds.

The system helps transform unstructured disaster data into actionable insights, enabling faster and more effective decision-making during emergencies.

🧩 Complete System Pipeline
The project follows a 6-step NLP pipeline:

🔹 Step 1: Data Collection (Multisource)
Data is collected from:

Reddit (citizen reports)

News RSS feeds

🔍 Keywords Used:
flood, earthquake, cyclone, landslide, fire, collapse, rescue, trapped
📌 Extracted Signals:
Disaster type

Location mentions

Casualties

Urgent needs

🔹 Step 2: Text Preprocessing
Performed using NLTK, SpaCy, Regex

✔ Lowercasing
✔ URL removal
✔ Hashtag removal
✔ Emoji removal
✔ Stopword removal
✔ Tokenization

➡️ Output: Cleaned and structured text dataset

🔹 Step 3: Information Extraction (NER)
Using SpaCy Pretrained Model

Extracted Entities:

📍 Location

🌪 Disaster Type

👥 Casualties

🏗 Infrastructure Damage

Example:
Location: Chennai
Disaster: Flood
Casualties: 5 injured
Damage: Bridge collapsed
🔹 Step 4: Message Classification
Messages are classified into:

🚨 Emergency Request

🏚 Damage Report

ℹ General Information

🤝 Relief Update

Approach:
Rule-based keyword classification (current)

Extendable to BERT-based classifier (future)

🔥 Priority Levels:
High

Medium

Low

🔹 Step 5: Text Summarization
Using Transformer Models (BART / T5)

Summarizes high-priority messages

Reduces information overload

Example Output:
Severe flooding in Chennai has trapped residents and caused infrastructure damage. Immediate rescue operations required.

🔹 Step 6: Output Dashboard
Built using Streamlit

📊 Dashboard Displays:
Extracted Entities

Message Category

Priority Level

Generated Summary

🧠 Tech Stack
Python

NLTK

SpaCy

Scikit-learn

Hugging Face Transformers (BART/T5)

Pandas

Streamlit

📂 Project Structure
DisasterNLP/
│── data/
│── preprocessing/
│── ner/
│── classification/
│── summarization/
│── dashboard/
│── app.py
│── requirements.txt
│── README.md
💡 Key Features
Multi-source disaster data collection

Real-time-like processing pipeline

Entity extraction (NER)

Disaster classification with priority tagging

Transformer-based summarization

Interactive dashboard

⚠️ Limitations
Limited real-time streaming

Rule-based classification (initial version)

Depends on data quality

English-only processing

🚀 Future Improvements
Real-time Twitter integration (when API available)

Fine-tuned BERT classification

Multilingual support

GIS-based visualization

Abstractive summarization improvements

🏁 Conclusion
This project demonstrates how NLP can be used to:

Extract critical disaster insights

Reduce information overload

Support emergency response systems

It provides a scalable foundation for intelligent disaster management systems.

👩‍💻 Authors
Sabana Asmi G

Yuvashree M
