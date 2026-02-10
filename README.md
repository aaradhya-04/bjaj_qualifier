# 🚀 Bajaj Finserv Qualifier — REST API (POST /bfhl & GET /health)

This repository contains a **production-ready REST API** built for the **Bajaj Finserv Qualifier Round (Chitkara University 2026)**. The project implements all required endpoints, follows strict response structures, includes validation, error handling, and integrates with **Google Gemini AI** for intelligent responses.

---

## 🎯 **Project Objective**

Develop and deploy two public REST APIs:

| Endpoint  | Method | Description                                                    |
| --------- | ------ | -------------------------------------------------------------- |
| `/health` | GET    | Checks if the server is running                                |
| `/bfhl`   | POST   | Performs computations or AI-based answering based on input key |

The API is **hosted live on Vercel** and publicly accessible.

---

## 🌍 **Live API Endpoints**

### ✅ Health Check

```
GET https://bjaj-qualifier.vercel.app/health
```

**Sample Response**

```json
{
  "is_success": true,
  "official_email": "aaradhya1503.be23@chitkara.edu.in"
}
```

---

### ✅ Core API

```
POST https://bjaj-qualifier.vercel.app/bfhl
```

#### Supported Keys (send only ONE at a time)

| Key         | Input           | Output                               |
| ----------- | --------------- | ------------------------------------ |
| `fibonacci` | Integer         | Fibonacci series                     |
| `prime`     | Integer array   | List of prime numbers                |
| `lcm`       | Integer array   | LCM value                            |
| `hcf`       | Integer array   | HCF value                            |
| `AI`        | Question string | Single-word AI response (via Gemini) |

---

## 📌 **Example Requests**

### Fibonacci

```json
{
  "fibonacci": 7
}
```

### Prime Numbers

```json
{
  "prime": [2,4,7,9,11]
}
```

### LCM

```json
{
  "lcm": [12,18,24]
}
```

### HCF

```json
{
  "hcf": [24,36,60]
}
```

### AI Question

```json
{
  "AI": "What is the capital of Maharashtra?"
}
```

---

## 🛠️ **Tech Stack**

* **Backend:** Node.js + Express
* **AI Integration:** Google Gemini API
* **Hosting:** Vercel
* **Version Control:** GitHub

---

## 📁 **Project Structure**

```
bajaj-qualifier/
│── server.js
│── package.json
│── package-lock.json
│── .gitignore
└── README.md
```

---

## 🚀 **How to Run Locally**

1. Clone the repo:

```bash
git clone https://github.com/aaradhya-04/bjaj_qualifier.git
```

2. Install dependencies:

```bash
npm install
```

3. Run the server:

```bash
node server.js
```

4. Test in browser:

```
http://localhost:3000/health
```

---

## 🔐 **Security Note**

* API keys should ideally be stored as environment variables in Vercel.
* Do **not** expose keys in public repositories.

---

## 👩‍💻 **Created By**

**Aaradhya**
B.Tech | Chitkara University

📧 [aaradhya1503.be23@chitkara.edu.in](mailto:aaradhya1503.be23@chitkara.edu.in)

---

If you want, I can also:

* format this in **Markdown styling**,
* add **badges**, or
* tailor it to look like a **professional portfolio project**.
