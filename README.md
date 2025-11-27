YouTube Video Question-Answering Using RAG (LangChain + OpenAI + FAISS)
📅 Duration: Jan 2025 – Feb 2025
🛠️ Tech Stack:

Python, LangChain, OpenAI (LLMs & Embeddings), YouTube Transcript API, FAISS Vector Store, ChromaDB, tiktoken

📌 Project Overview

This project implements an end-to-end Retrieval-Augmented Generation (RAG) system that takes any YouTube video link, extracts its transcript, and allows users to ask natural-language questions about the video. The pipeline processes transcripts, converts them into embeddings, stores them in a vector database, retrieves the most relevant chunks, and generates accurate, context-grounded responses using OpenAI LLMs.

This ensures factual answers, reduced hallucinations, and efficient retrieval even for long videos.

🚀 Key Features

Extracts official YouTube subtitles using YouTube Transcript API

Handles missing, disabled, or unavailable transcripts with exception handling

Chunks long transcripts using RecursiveCharacterTextSplitter

Creates embeddings with OpenAIEmbeddings

Stores and retrieves context using FAISS & ChromaDB

Uses LangChain Runnables (RunnableParallel & RunnableLambda) for modular RAG flow

Custom prompting for contextual, grounded LLM answers

Responds to any user query about the video content

🧩 System Architecture

Transcript Extraction

Fetches and merges YouTube caption chunks into a clean transcript.

Text Chunking & Preprocessing

Splits transcript into optimized chunks for embedding and retrieval.

Embedding Generation

Converts each chunk to vector embeddings using OpenAI.

Vector Storage

Stores embeddings in FAISS for fast similarity search.

Context Retrieval

Retrieves the top-k relevant chunks for any user query.

LLM Response Generation

Passes query + retrieved context into ChatOpenAI for grounded answers.

🔧 Key Contributions

Implemented transcript extraction and robust error handling

Designed optimized chunking for better embedding accuracy

Built FAISS vector store for high-speed similarity search

Orchestrated RAG pipeline using LangChain RunnableParallel and RunnableLambda

Created custom prompts for factual, context-bound LLM responses

Integrated ChatOpenAI for final answer generation

Enabled scalable workflows using ChromaDB and FAISS

📈 Outcome & Impact

Highly accurate, hallucination-resistant answers grounded strictly in video content

Reduced token usage via optimized chunking and retrieval

Modular RAG pipeline that can be reused for:

Educational content summarization

Video-based Q&A systems

AI tutoring systems

Long-form content search
