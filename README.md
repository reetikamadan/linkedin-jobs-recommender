# LinkedIn Job Recommender Engine

A real-time job recommendation system that matches users to relevant job opportunities based on their current skills and identifies personalized upskilling paths. It uses NLP, vector embeddings, and streaming data pipelines to generate career-aware suggestions and highlight aspirational roles.

## 🔑 Features

- 🔍 Personalized job recommendations based on skill and profile similarity
- ⚙️ Real-time job data ingestion using Kafka producer–consumer pipeline
- 🧠 NLP-powered skill extraction and cosine similarity scoring
- 🚀 LLaMA-based skill gap analysis to surface aspirational roles
- 📊 Dynamic recommendations updated with live job market data

## 🧠 How It Works

1. **Data Ingestion**: Real-time job postings are fetched from the LinkedIn API via a Kafka producer.
2. **Stream Processing**: A Kafka consumer stores and processes the incoming job data.
3. **Embedding & Matching**: User profiles and job descriptions are encoded using sentence-transformers, and cosine similarity identifies best-fit jobs.
4. **Aspirational Role Discovery**: LLaMA identifies additional skills that can unlock higher-paying or senior roles.
5. **Output**: The system displays jobs the user is qualified for now, and recommends upskilling to qualify for better roles.

## ⚙️ Data Sources

- [LinkedIn Job Postings (Kaggle)](https://www.kaggle.com/datasets/arshkon/linkedin-job-postings)
- [LinkedIn API via RapidAPI](https://rapidapi.com/rockapis-rockapis-default/api/linkedin-data-api/)
- [LinkedIn User Dataset (GitHub)](https://github.com/navid-aub/LinkedIn-Dataset)


## 🧰 Tech Stack

- Python
- SentenceTransformers (for embedding)
- LLaMA via Hugging Face
- Confluent Cloud (Apache Kafka backend- Producer and Consumer)
- Google Colab / Jupyter Notebooks

---

