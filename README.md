# n8n_RAG_chatbot_web
📘 Project Title

AI-Powered School Information & Admission Assistant (RAG-based)

🧩 Problem Statement

Schools receive many repetitive questions from parents about admissions, fees, timings, policies, and facilities.
These questions are usually answered manually by school staff, which:

- Takes time

- Delays responses

- Is not available 24/7

Parents also need a simple way to express interest in admissions without visiting the school physically.

💡 Solution Overview

This project provides an AI-powered school assistant that answers parent queries using a controlled knowledge base.

The system uses a Retrieval-Augmented Generation (RAG) approach to ensure that answers come only from verified school data, not from general AI knowledge.

Parents can:

- Ask questions via a website chatbot

- Get accurate, context-aware answers

- Receive an official admission form link when they show interest

This reduces administrative workload and improves parent experience.

🏗️ System Architecture (High Level)

The system is divided into two main workflows:

1️⃣ Knowledge Base Sync Workflow

- School data is stored in Google Docs (policies, details)

- FAQs are managed in Google Sheets

- Data is merged, embedded, and stored in Supabase Vector Database

2️⃣ Chatbot Interaction Workflow

- Parent asks a question via website chatbot

- AI Agent retrieves relevant context from Supabase

- Response is generated using RAG

- Parent queries are logged for future improvement

- Admission-related interest triggers a Google Form link

✨ Key Features

- RAG-based question answering (no hallucination)

- Admin-managed knowledge base

- FAQ auto-update via Google Sheets

- Parent query logging

- Admission interest redirection via Google Form

- Clear separation between data ingestion and user interaction

🛠️ Technologies Used

- n8n – Workflow automation

- Supabase – Vector database for retrieval

- Google Docs – Static school information

- Google Sheets – FAQs and query logging

- LLM (AI Agent) – Response generation

- Local Website – Chatbot interface (prototype)

🔄 How the System Works (Step-by-Step)

- Admin updates school information in Google Docs or FAQs in Google Sheets

- n8n syncs and embeds the data into Supabase

- A parent visits the school website and asks a question

- The AI Agent retrieves relevant content from the knowledge base

- The chatbot responds with accurate information

- If the parent asks about admissions, the chatbot shares the official admission form link

- Parent questions are logged for future analysis and improvement

📌 Use Case Example

Scenario:
A parent wants to know about school admission.

Flow:

- Parent asks: “What is the admission process?”

- Chatbot searches the school knowledge base

- AI responds with admission details

- Chatbot provides a Google Form link for admission inquiry

- Parent fills the form to request a callback

⚠️ Limitations

- Uses synthetic data to simulate real school information (privacy reasons)

- Website is locally hosted as a prototype

- Admission form processing can be fully automated in future

🚀 Future Improvements

- Automatic processing of admission form submissions

- Email or WhatsApp notifications

- Analytics dashboard for parent queries

- Deployment on cloud hosting

🎥 Demo

- Workflow screenshots included

- AI-generated demo video attached

🎯 Project Goal

The goal of this project is to demonstrate end-to-end AI automation, RAG implementation, and real-world system design, rather than just a simple chatbot.
