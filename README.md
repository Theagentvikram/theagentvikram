# Hey, I'm Cherupally 👋

<div align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=22&duration=3000&pause=1000&color=36BCF7&center=true&vCenter=true&multiline=true&width=720&height=90&lines=Generative+AI+Engineer+%7C+RAG+%26+Document+AI;I+build+AI+that+works+on+real%2C+messy+documents" alt="Typing SVG" />
</div>

I build AI systems that hold up on real business data, not just in demos. Most of my work is document AI and RAG: reading long, messy PDFs, scans and XML, pulling out what matters, and checking it against rules people can trust.

My rule of thumb: use AI where it earns its place, and plain code everywhere else. It keeps things fast, cheap and easy to debug.

- 💼 **Recently:** spent a year as a freelance ML engineer for **Syncd Analytics (US)**, rebuilding an AI platform that reviews property appraisal reports. Rated **5.0/5** on Upwork.
- 🔨 **Building:** JobPilot, Nexus and JobEasy (below)
- 🏠 **Weekends:** a home lab with a Raspberry Pi, a Linux server and a NAS, running my own agents and side projects
- 🏏 **Off screen:** cricket and chess

---

## 💼 Experience

**AI/ML Engineer (Freelance) · Syncd Analytics, US** · *Aug 2025 – Jul 2026*
- Took over an AI quality-control platform for appraisal reports and rebuilt it into something the review team could rely on
- Multimodal RAG pipeline with Vision-Language Models that reads text, tables, scans and photos in each report
- Hybrid review engine: rules handle the clear-cut checks, the LLM only handles judgement calls, which cut API cost and processing time
- Multi-tenant Django REST + Celery backend so big batches run in parallel, with a Next.js front end and live updates over WebSockets
- Deployed on AWS, with models compared across Bedrock, Azure OpenAI and local LLMs on accuracy, speed and cost

**Machine Learning Intern · Intel Unnati Programme** · *May 2023 – Jul 2023*
- Built a fake news detector end to end: data cleaning, NLP pipeline, model comparison (LR, Naive Bayes, SVM) and a live Streamlit app
- Led a small team through planning, code review and delivery

---

## 🎯 Projects

### 🤖 JobPilot: a data pipeline and browser agent that runs itself every night
Goes from raw web data to finished action with nobody watching. I built it for job applications, but every layer is separate, so new sources and tasks plug straight in.
- **Collects** about 40,000 postings a day from Greenhouse, Lever, Ashby and Workable with a Scrapy crawler on Zyte, then removes duplicates and ranks them
- **Organises** results with ~10 scheduled pipelines that update a Google Sheets tracker, file documents in Drive and send one daily email
- **Acts** through a Playwright browser agent that fills multi-step forms. It tries saved answers first and only asks the LLM when it has to
- **Survives failure:** catches up after outages, never runs twice at once, and always waits for a human before anything is submitted

`Python` `Scrapy` `Playwright` `Node.js` `LLMs` `cron` `systemd`

### 🧠 Nexus: a second brain you can talk to
All my notes, PDFs and saved articles in one place, answered in plain English.
- Every answer shows the exact sources it used, and if the answer isn't in my documents, it says so instead of guessing
- Handles scanned PDFs with OCR and splits documents by their real structure, so answers keep their context
- Mixes keyword and semantic search with re-ranking, so it finds the right passage whether I remember the words or just the idea
- I test retrieval on my own question set after every change, so quality never quietly slips

`Python` `LangChain` `ChromaDB` `pgvector` `FastAPI` `Next.js` `Docker`

### 💼 [JobEasy: beat the ATS, land the interview](https://jobeasy.app)
A live SaaS I designed, built and shipped on my own.
- Resume scanner on fine-tuned sentence transformers that shows how well a CV matches a job before you apply
- An AI assistant on a locally hosted open-source model, so users' data never leaves the platform
- Browser automation that cuts a typical application from 15 minutes to under 2
- Kanban tracker, email reminders and version history for resumes and cover letters

`Next.js` `React` `FastAPI` `Django` `PostgreSQL` `Cloudflare` `Sentence Transformers`

### 🛒 Retail Vision: real-time shoplifting detection
Spots and follows people across store camera footage and alerts staff to suspicious behaviour. I led the team and published a paper on it.
- YOLOv8 detection with DeepSORT tracking that keeps hold of people through crowds, blur and partial blocking
- Flags loitering, back-and-forth pacing and long dwell times
- FastAPI backend with a React dashboard showing live boxes and time-stamped alerts

`YOLOv8` `DeepSORT` `OpenCV` `FastAPI` `React`

---

## 🏠 Weekend Builds
- **Kite**: an AI learning app that keeps kids asking questions instead of just watching
- **Rehearse**: a mock interview tool that listens and talks back in real time
- **My agents**: I talk to them with Wispr instead of typing, watch them on my own dashboards, and they share work across two machines
- **A model gateway**: free models (DeepSeek, Kimi, GLM) do the bulk work and Claude makes the real decisions, with personal data masked before anything leaves the house

---

## 🛠️ Tech Stack

**AI & LLMs**
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white)
![Claude](https://img.shields.io/badge/Claude-D97757?style=for-the-badge&logo=anthropic&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white)
![Hugging Face](https://img.shields.io/badge/Hugging%20Face-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black)
![Ollama](https://img.shields.io/badge/Ollama-000000?style=for-the-badge&logo=ollama&logoColor=white)
![MCP](https://img.shields.io/badge/MCP-000000?style=for-the-badge&logo=anthropic&logoColor=white)
![ChromaDB](https://img.shields.io/badge/ChromaDB-FF6F61?style=for-the-badge)

**ML & Data**
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Scrapy](https://img.shields.io/badge/Scrapy-60A839?style=for-the-badge&logo=scrapy&logoColor=white)

**Back End & Front End**
![Python](https://img.shields.io/badge/Python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Django](https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=white)
![Celery](https://img.shields.io/badge/Celery-37814A?style=for-the-badge&logo=celery&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-005571?style=for-the-badge&logo=fastapi)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=next.js&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DD0031?style=for-the-badge&logo=redis&logoColor=white)

**Cloud & DevOps**
![AWS](https://img.shields.io/badge/AWS-FF9900?style=for-the-badge&logo=amazonwebservices&logoColor=white)
![Azure](https://img.shields.io/badge/Azure-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white)
![GCP](https://img.shields.io/badge/GCP-4285F4?style=for-the-badge&logo=googlecloud&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-0db7ed?style=for-the-badge&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2671E5?style=for-the-badge&logo=githubactions&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Raspberry Pi](https://img.shields.io/badge/Raspberry_Pi-A22846?style=for-the-badge&logo=raspberrypi&logoColor=white)

---

## 🏆 Certifications & Highlights
- ☁️ AWS Certified AI Practitioner (Sep 2026) · AWS Certified Cloud Practitioner (Oct 2026)
- 🧠 Oracle Generative AI Professional · Oracle Data Science Professional · Oracle AI Foundations Associate
- ⭐ Upwork **Rising Talent**, 5.0/5 client rating
- 📈 GATE All India Rank **4,800** (2025) and **6,000** (2024)
- 🎓 Bachelor's in AI & ML, Sreenidhi Institute of Science and Technology (SNIST), top 5% of the department

---

## 📊 GitHub Stats

<div align="center">
  <img height="170" src="https://github-readme-stats.vercel.app/api?username=Theagentvikram&show_icons=true&theme=tokyonight&include_all_commits=true&count_private=true&hide_border=true" />
  <img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Theagentvikram&layout=compact&langs_count=8&theme=tokyonight&hide_border=true" />
</div>

<div align="center">
  <img src="https://streak-stats.demolab.com/?user=Theagentvikram&theme=tokyonight&hide_border=true" alt="GitHub Streak" />
</div>

---

## 🌐 Say Hi

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/AbhiCherupally)
[![Upwork](https://img.shields.io/badge/Upwork-6FDA44?style=for-the-badge&logo=upwork&logoColor=white)](https://www.upwork.com/freelancers/~01677b33e344495620)
[![JobEasy](https://img.shields.io/badge/JobEasy-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://jobeasy.app)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:cherupallyabhi@gmail.com)

<br/>
<img src="https://komarev.com/ghpvc/?username=Theagentvikram&label=Profile%20views&color=0e75b6&style=flat" alt="Profile views" />

</div>
