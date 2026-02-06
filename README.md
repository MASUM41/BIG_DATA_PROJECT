# 📚 Intelligent Book Recommendation System
### A Hybrid Search Engine using Big Data Engineering & AI

##  Project Overview
This project is an end-to-end **Big Data & AI application** that helps users find books not just by keywords, but by *meaning*. It combines traditional **SQL Search** (for exact matches) with **Semantic Vector Search** (AI) to understand user intent (e.g., searching for *"sad story about space"* finds *"Cosmos"* or Sci-Fi novels).

##  Architecture (Three-Phase Pipeline)

### **Phase 1: Data Engineering (ETL)**
* **Data Source:** Raw CSV logs (Library dataset).
* **Processing:** Cleaning, normalization, and handling missing values using **Pandas**.
* **Storage:** Structured data stored in **SQLite** for fast retrieval.

### **Phase 2: AI & Backend (The "Brain")**
* **Embeddings:** Converted 30,000+ book descriptions into 384-dimensional vectors using **Sentence Transformers (`all-MiniLM-L6-v2`)**.
* **Similarity Engine:** Uses **Cosine Similarity** to rank books based on "vibes" and concepts.
* **API:** Built with **FastAPI** to serve both SQL and AI results via REST endpoints (`/search` and `/recommend`).

### **Phase 3: User Interface**
* **Frontend:** Interactive **Streamlit** dashboard.
* **Features:** Toggle between "Keyword Search" (Database) and "AI Recommendation" (Semantic).

---

## 🛠️ Tech Stack
* **Language:** Python 3.11+
* **API Framework:** FastAPI
* **AI Model:** Sentence-Transformers (Hugging Face)
* **Frontend:** Streamlit
* **Database:** SQLite
* **Data Processing:** Pandas, NumPy

---

##  How to Run Locally

### 1. Clone the Repository
```bash
git clone [https://github.com/MASUM41/BIG_DATA_PROJECT.git](https://github.com/MASUM41/BIG_DATA_PROJECT.git)
cd BIG_DATA_PROJECT
