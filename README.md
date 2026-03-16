# TradeFind — AI-Powered Import/Export Trade Directory
An AI-powered web application to search global importers and exporters by country, product, and trade type. Built with Flask, SQLite, and three AI features.


TradeFind is an AI-powered import/export trade intelligence platform 
built as an AI/ML internship project. It allows users to search verified 
trade companies worldwide by country, product, and trade type — and 
download complete contact lists in Excel instantly.

The platform features three AI layers:

1. NLP Semantic Search — uses sentence-transformers to match queries 
   by meaning, not just keywords. Searching "petroleum" finds "oil" 
   companies. Searching "garments" finds "textile" companies.

2. Smart Recommendations — uses TF-IDF vectorization and cosine 
   similarity to suggest similar companies on every detail page, 
   ranked by match percentage.

3. AI Chatbot Assistant — powered by Groq Llama 3, understands 
   natural language queries like "find oil exporters in UAE with 
   email" and returns real company results instantly.


## Features
- Classic search by country, product, and trade type
- AI semantic search using sentence-transformers (petroleum finds oil)
- Similar company recommendations using TF-IDF cosine similarity
- AI chatbot powered by Groq Llama 3 for natural language queries
- Excel export with all contact details
- Company detail page with products, services, address, and website

## Tech Stack
- Python, Flask, SQLite
- sentence-transformers (all-MiniLM-L6-v2)
- scikit-learn (TF-IDF + cosine similarity)
- Groq API (llama-3.3-70b-versatile)
- openpyxl for Excel export
- Cloudflare Tunnel for public URL

## How to Run on Google Colab
1. Open TradeFind_FINAL.ipynb in Google Colab
2. Save your Groq API key in Colab Secrets as: API
3. Run Cell 1 — installs libraries
4. Run Cell 2 — builds app and launches it
5. Run Cell 3 — gets your public URL
6. Click the URL to open the live app

## Get Free Groq API Key
https://console.groq.com — free, no credit card needed

## Sample Searches
- UAE + Oil + Exporter → 8 companies
- Pakistan + Textile + Exporter → 3 companies
- AI search: type petroleum Gulf
- Chatbot: find oil exporters in UAE with email

## Project Structure
- app.py — Flask web application
- ai/nlp_search.py — NLP semantic search engine
- ai/recommender.py — TF-IDF similarity recommender
- ai/chatbot.py — Groq LLM chatbot
- templates/ — HTML templates with inlined CSS and JS
- data/trade.db — SQLite database

## Internship Project
Built as an AI/ML internship project demonstrating:
- NLP text embeddings and vector search
- Content-based recommendation systems
- LLM API integration and prompt engineering
- Full-stack web development with Flask
