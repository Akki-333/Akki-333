<!--
🌈 Welcome Banner
-->

<h1 align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=28&pause=1200&color=FF6F61&center=true&vCenter=true&width=1200&height=70&lines=Hi%2C+I+am+Akshay!!!;Software+Developer+%7C+Web+Development+%7C+Aspiring+Data+Analyst" alt="Typing SVG" />
</h1>

<p align="center">
  <img src="https://img.shields.io/badge/Software%20Development-2E8B57?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Artificial%20Intelligence-8A2BE2?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Full--Stack%20Development-61DAFB?style=for-the-badge&logo=react&logoColor=black" />
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/LLM%20%7C%20RAG-FF6F61?style=for-the-badge" />
  <img src="https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white" />
  <img src="https://img.shields.io/badge/Gamer-1e2a78?style=for-the-badge&logo=steam&logoColor=white" />
</p>
<p align="center">
  <a href="https://portfolio-by-akshay.vercel.app/" target="_blank">
    <img src="https://img.shields.io/badge/Portfolio-Visit%20My%20Portfolio-2E8B57?style=for-the-badge&logo=vercel&logoColor=white" />
  </a>

  <a href="https://www.linkedin.com/in/ak445/" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" />
  </a>

  <a href="mailto:akkies445@gmail.com">
    <img src="https://img.shields.io/badge/Email-Contact%20Me-FF6F61?style=for-the-badge&logo=gmail&logoColor=white" />
  </a>
</p>
---

## 🚀 About Me

👋 **Hi, I'm Akshay — a Computer Science Engineer and Software Developer who enjoys building practical software and AI systems.**

💻 Currently working as a **Software Developer at BDSR Solutions LLP**, contributing to production applications across backend development, full-stack development, automation, APIs, debugging, performance optimization, and deployment.

🧠 My current focus is at the intersection of **Software Engineering and Artificial Intelligence** — building applications around **LLMs, RAG, GraphRAG, document intelligence, semantic search, and intelligent automation**.

⚙️ I enjoy taking problems from **idea → architecture → implementation → debugging → deployment**, rather than only working on isolated pieces of a system.

🌐 My experience also includes **React, Flask, FastAPI, SQL, web scraping, REST APIs, Git, Linux, remote deployments, testing, and application security**.

🎯 I am particularly interested in opportunities involving **AI Engineering, Backend Engineering, Full-Stack Development, and Data Engineering**.

🎮 Outside technology, I enjoy **video games, cricket, and movies**.

---

## 💼 What I Do

### 🔹 Software Engineering
- Build and maintain production-oriented web applications.
- Develop backend services, REST APIs, frontend components, and database workflows.
- Debug complex application issues and improve system performance.
- Work with Git-based development, code reviews, testing, and remote deployments.

### 🔹 AI Engineering
- Build LLM-powered applications and retrieval systems.
- Work with **RAG, GraphRAG, vector databases, knowledge graphs, embeddings, and prompt engineering**.
- Explore practical applications of NLP, document intelligence, OCR, and intelligent automation.

### 🔹 Data & Automation
- Build Python-based automation and web scraping workflows.
- Work with structured and unstructured data.
- Develop document ingestion and processing pipelines.
- Use SQL, Pandas, Power BI, and Python for analysis and visualization.

---

## 🏢 Professional Experience

### Software Developer — BDSR Solutions LLP
**Mar 2026 – Present**

- Contribute to **Quantis**, an enterprise performance management platform, working across React-based frontend development, Python/Flask backend services, REST APIs, debugging, testing, and production support.
- Build and enhance application features, dashboards, menus, API integrations, and performance-related functionality.
- Develop and maintain **Python-based web scraping and automation workflows**, including URL extraction, HTML processing, dynamic website handling, and data processing.
- Worked across the web scraping lifecycle from **URL discovery → HTML parsing → backend processing → remote deployment and monitoring**.
- Optimized Python backend logic to process multiple companies through a shared API connection, reducing connection overhead and improving execution efficiency.
- Deploy and troubleshoot applications on remote environments using **SSH, PuTTY, and WinSCP**.
- Collaborate with developers and team leads using **Git, code reviews, task prioritization, and structured debugging workflows**.
- Gain hands-on experience working with production systems where reliability, maintainability, and performance matter.

---

## 🧠 Featured Projects

### 🧠 ArchiveMind AI — Hybrid GraphRAG Knowledge System

> **An AI-powered document intelligence platform designed to make complex government policy documents searchable, understandable, and context-aware.**

🔗 **Repository:**  
https://github.com/Akki-333/ArchiveMind-AI

**What I built:**
- Designed a hybrid **GraphRAG architecture** combining **Pinecone vector retrieval + Neo4j knowledge graphs**.
- Integrated **Groq Llama 3.3 70B** through LangChain for document understanding, entity extraction, recommendations, and conversational responses.
- Built a multi-format document ingestion pipeline supporting **PDF, DOCX, PPTX, TXT, CSV, and Markdown**.
- Implemented document chunking, embeddings, metadata filtering, semantic retrieval, and document-scoped querying.
- Built **JWT authentication, bcrypt password hashing, and role-based access control** for Admin and User workflows.
- Developed multi-session conversations with persisted chat history and an 8-message contextual window.
- Built an interactive **knowledge graph / mind-map explorer using React Flow and Dagre**.
- Added document profiles, AI recommendations, graph exploration, and query-specific entity extraction.

### ⚡ Engineering Decisions

One of the most important improvements was redesigning the graph extraction pipeline.

The initial architecture performed LLM-based entity extraction across every document chunk during ingestion, resulting in **40+ LLM calls for a typical document**, causing rate-limit problems and slow uploads.

I redesigned the system around **lazy graph extraction**:

`Document → Vector Retrieval → Relevant Chunks → Query-Time Entity Extraction → Knowledge Graph`

This reduced upload-time LLM calls from approximately **40 to 1** while making the generated graph more relevant to the user's actual question.

Other engineering decisions include:

- Deterministic chat auto-titling instead of spending an LLM call.
- Similarity-score filtering before sending retrieved chunks to the LLM.
- Document-scoped vector retrieval.
- Cascading cleanup across Pinecone and Neo4j during document deletion.
- Persistent graph-based storage for users, sessions, messages, documents, and entities.

**Tech Stack:**  
`Python` `FastAPI` `LangChain` `Groq` `Llama 3.3 70B` `Pinecone` `Neo4j` `HuggingFace` `React` `Vite` `TailwindCSS` `React Flow` `Dagre` `JWT` `bcrypt`

---

### 🍽️ Stay & Dine — Reserve & Dine Experience

> **A full-stack restaurant reservation platform that combines table booking with pre-arrival meal ordering.**

🔗 **Repository:**  
https://github.com/Akki-333/Stay_and_Dine

🌐 **Live Application:**  
https://hotel-reservation-system-two.vercel.app/

**Highlights:**
- Built a complete **React + Node.js + Express + MySQL** full-stack application.
- Designed a custom **2D interactive restaurant floor plan** supporting multiple table geometries and real-time availability states.
- Implemented **JWT authentication** and role-based access control for Admin and User workflows.
- Added Axios interceptors for automatic Bearer-token handling.
- Implemented secure image uploads using Multer with file-type validation.
- Built real-time booking and cancellation notifications using **WebSockets**.
- Added live restaurant occupancy tracking for administrators.
- Developed menu browsing and **pre-ordering** as part of the reservation workflow.
- Added nutritional information including calories, protein, and fiber.
- Implemented targeted coupons based on user booking activity.
- Built protected routes, administrative management workflows, booking history, and responsive UI components.

**Tech Stack:**  
`React 18` `Vite` `React Router` `Node.js` `Express.js` `MySQL` `JWT` `bcrypt` `Axios` `WebSockets` `Vanilla CSS` `React Bootstrap`

---

### 📚 Bibliography Extraction & Document Intelligence

> **A document-processing application that extracts structured bibliographic information from unstructured documents and scanned images.**

🔗 **Repository:**  
https://github.com/Akki-333/Bibliography_extraction

🌐 **Live Application:**  
https://bibliography-extraction.vercel.app/

**Highlights:**
- Built a **Streamlit-based document intelligence application**.
- Supports PDF, image, DOCX, and PPTX inputs.
- Used **PyMuPDF** for PDF processing and **Tesseract OCR** for scanned images.
- Applied **spaCy NLP** and entity recognition to extract structured information.
- Used Pandas for data processing and export.
- Designed the workflow to convert messy document content into structured bibliographic fields.

**Tech Stack:**  
`Python` `Streamlit` `PyMuPDF` `Tesseract OCR` `spaCy` `Pandas` `NumPy` `python-docx` `python-pptx` `Pillow`

---

## 🛠️ Technical Skills

### 👨‍💻 Languages
`Python` `JavaScript` `SQL` `C` `HTML5` `CSS3`

### ⚛️ Frontend
`React` `React Router` `Vite` `Tailwind CSS` `Axios` `React Flow`

### 🔧 Backend
`FastAPI` `Flask` `Node.js` `Express.js` `REST APIs`

### 🤖 AI / Machine Learning
`Generative AI` `LLMs` `RAG` `GraphRAG` `Prompt Engineering` `LangChain` `NLP` `Document Intelligence` `Semantic Search` `Knowledge Graphs` `Vector Embeddings` `OCR` `OpenCV`

### 🗄️ Databases
`MySQL` `PostgreSQL` `SQLite` `Neo4j` `Pinecone`

### 📊 Data & Analytics
`Power BI` `Power Query` `DAX` `Excel` `Pandas` `NumPy` `Tableau`

### 🌐 Automation & Data Extraction
`Web Scraping` `Python Automation` `Playwright` `HTML Parsing` `XPath` `CSS Selectors` `Chrome DevTools`

### 🧪 Testing & Security
`Pytest` `Playwright` `API Testing` `UI Testing` `OWASP ZAP` `DAST` `Functional Testing` `CORS` `CSP` `JWT` `RBAC`

### ☁️ Development & Deployment
`Git` `GitHub` `Docker` `Linux` `SSH` `PuTTY` `WinSCP`

---

## 📊 My Engineering Focus

```text
AI Engineering       ████████████████████  Building
Backend Engineering  ███████████████████░  Strong
Full-Stack           ██████████████████░░  Strong
Data Engineering     ████████████████░░░░  Growing
Data Analytics       ███████████████░░░░░  Experienced
DevOps               ████████████░░░░░░░░  Growing
Application Security ████████████░░░░░░░░  Hands-on
