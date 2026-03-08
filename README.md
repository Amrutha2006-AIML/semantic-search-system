Below is a **clean, improved README for your repository**. It keeps the **same structure as your friend’s** (so it matches the assignment style) but is **slightly more professional and clearer**.

You can **copy and paste this into your `README.md`**.

---

# Trademarkia – AI/ML Engineer Task

# Semantic Search System

This project implements a **semantic search system** that retrieves documents based on their **meaning rather than exact keyword matches**.

The system processes natural language queries using **text embeddings**, performs **fast similarity search using FAISS**, organizes queries using **clustering**, and improves efficiency using a **semantic caching mechanism**.

The API is built using **FastAPI**, allowing users to interact with the system through REST endpoints.

---

# Features

* Semantic search using **sentence embeddings**
* Fast vector similarity search using **FAISS**
* Intelligent **semantic cache** to avoid repeated computation
* **Query clustering** for improved search organization
* Cache performance tracking
* RESTful API built with **FastAPI**

---

# Project Structure

```
semantic-search-system/

api/ → FastAPI endpoints

cache/ → Semantic caching logic

clustering/ → Fuzzy clustering implementation

embeddings/ → Text embedding generation

vector_store/ → FAISS vector search system

utils/ → Text preprocessing utilities

data_loader.py → Dataset loading and preparation

requirements.txt → Project dependencies

README.md → Project documentation
```

---

# Installation

Clone the repository

```
git clone https://github.com/Amrutha2006-AIML/semantic-search-system.git
```

Navigate to the project folder

```
cd semantic-search-system
```

Install the required dependencies

```
pip install -r requirements.txt
```

---

# How to Run the Project

Follow the steps below to run the application locally.

### 1. Create a virtual environment

```
python -m venv venv
```

### 2. Activate the virtual environment

On Windows

```
venv\Scripts\activate
```

On Mac / Linux

```
source venv/bin/activate
```

### 3. Install dependencies

```
pip install -r requirements.txt
```

### 4. Start the FastAPI server

```
uvicorn api.main:app --reload
```

After running this command, the server will start and display the **local server address**.

---

# Open API Documentation

Open the following link in your browser:

```
http://127.0.0.1:8000/docs
```

This will open the **interactive FastAPI documentation**, where you can test all endpoints.

---

# API Endpoints

### Search Query

```
POST /query
```

Used to submit a semantic search query and retrieve relevant results.

---

### Cache Statistics

```
GET /cache/stats
```

Returns statistics about cache usage including hits and misses.

---

### Clear Cache

```
DELETE /cache
```

Clears all cached queries and resets statistics.

---

# Example Cache Statistics Output

```
{
 "total_entries": 0,
 "hit_count": 0,
 "miss_count": 0,
 "hit_rate": 0
}
```

---

# Technologies Used

* Python
* FastAPI
* Sentence Transformers
* FAISS
* NumPy
* Scikit-learn

---

# Author

D. Amrutha
AI/ML Engineer Task Submission – Trademarkia

---
