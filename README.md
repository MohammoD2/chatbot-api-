# 🤖 Bulipe Tech Chatbot (FastAPI + FAISS)

  

A lightweight, production-ready chatbot backend that answers company service-related queries using a question-answer dataset (`data.xlsx`).

Built with **FastAPI**, **FAISS** for scalable search, and **sentence-transformers**.

  

---

  

## 📁 Project Structure
bulipe\_chatbot/

├── chatbot.py # Core logic: embedding, search, FAISS

├── main.py # FastAPI app and API endpoint

├── data.xlsx # Chat dataset (Input & Response)

├── test\_chatbot.py # Optional pytest unit test

├── requirements.txt # Python dependencies

└── README.md # Project documentation

## 🚀 Running Locally

  

### ✅ Step 1: Clone and enter the project

  

```

git clone https://your-repo-url.git

````

```

cd bulipe_chatbot

````
  

### ✅ Step 2: Create a virtual environment

  

```bash

python3  -m  venv  venv

source  venv/bin/activate

```

  

### ✅ Step 3: Install dependencies

  

```bash

pip  install  --upgrade  pip

pip  install  -r  requirements.txt

```

  

### ✅ Step 4: Start the FastAPI server

  

```bash

uvicorn  main:app  --reload

```

  

---

  

## 📍 API Docs

  

Visit the Swagger UI:

  

👉 [http://127.0.0.1:8000/docs](http://127.0.0.1:8000/docs)

  

---

  

## 📡 API Endpoint

  

### `POST /chat/`

  

#### ➤ Request

  

```json

{

"message": "What services do you offer?"

}

```

  

#### ➤ Response

  

```json

{

"response": "We offer web development, SEO, and AI automation services."

}

```

  

---

  

## 🧪 Run Unit Tests (Optional)

  

```bash

pytest  test_chatbot.py

```

  

---

  

## 🛠 Deployment Notes

  

* Can be hosted using **Uvicorn + Gunicorn** or **Docker**

* Optional: Set up **Nginx** + **Let's Encrypt** SSL

* FAISS supports efficient search on large datasets

* Dataset is stored in `data.xlsx` — update to improve responses

  

---

  

## 🔐 Production Security Checklist

  

* ✅ Input validation included

* 🔒 Add rate limiting (e.g., `slowapi`)

* 🔒 Add authentication if exposed publicly

* 🔒 Serve over HTTPS (SSL)

  

---

  

## 👨‍💻 Maintainers

  

*  **Initial Developer**: \[Your Name]

*  **Deployment**: Hand over to Backend/DevOps for API deployment and website integration

  

---

✅ Let me know if you want this:

- Converted into an actual file (`README.md`)

- Automatically zipped with your code folder

- Published to GitHub with an example repo

