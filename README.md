YouTube Video Question-Answering Using RAG (LangChain + OpenAI + FAISS)

Tech Stack: Python, LangChain, OpenAI (LLMs & Embeddings), YouTube Transcript API, FAISS Vector Store, ChromaDB, tiktoken

Description:
Built an end-to-end Retrieval-Augmented Generation (RAG) system that extracts transcripts from YouTube videos and enables users to ask any question about the video content. The system processes raw transcripts, generates embeddings, stores them in a vector database, and retrieves the most relevant context to produce accurate LLM-based answers.

Key Contributions:

Fetched video transcripts using YouTube Transcript API, handled missing/disabled subtitles with exception handling.

Cleaned and chunked long transcripts using Recursive Character Text Splitter to optimize embedding quality.

Generated vector embeddings using OpenAIEmbeddings and stored them in FAISS for fast similarity search.

Designed a RAG pipeline using LangChain RunnableParallel & RunnableLambda to format context dynamically.

Built a custom prompt template to combine retrieved context with user queries for improved LLM reasoning.

Integrated ChatOpenAI model to generate accurate and video-grounded answers.

Enabled scalable retrieval workflows using Chroma & FAISS vector stores.

Outcome / Impact:

Achieved context-aware and hallucination-free answers aligned strictly with video content.

Reduced LLM token usage by implementing optimized chunking & retrieval.

Developed a reusable and modular RAG workflow suitable for educational, summarization, and conversational AI applications.
