# RAG-Powered Bildungsplan Chatbot

## Goal

Design and implement a Retrieval-Augmented Generation (RAG) pipeline in Python (Jupyter Notebook) that allows a user to query the Bildungsplan Baden-Württemberg (Grundschule, Deutsch, 2016).

The chatbot should return answers grounded in the Bildungsplan, with references to the relevant section(s).
👉 Don’t worry about covering the entire Bildungsplan — it’s fine to use a subset, a few chapters, or even example snippets. The main focus is your approach to retrieval, augmentation, and response generation.

## Data Sources (choose freely)

- 📄 PDF (we provide): [Bildungsplan Deutsch Grundschule 2016](Bildungsplan%20Grundschule%20Deutsch.pdf) (alternatives available online)


- 🌐 Online Bildungsplan: [Bildungsplan-BW Website](https://www.bildungsplaene-bw.de/,Lde/LS/BP2016BW/ALLG)

- _Pre-processed JSON (optional help if needed, ask us)_

You may:

Use the full data, or just a part of it. So it fine if u only focus on German in Grade 1-4 or 5-10 etc.

Skip heavy preprocessing if it feels overwhelming.

## Requirements

- Data Handling

- Extract or load text (from PDF, website, or JSON).

- Split the text into meaningful chunks (paragraphs, competence statements, etc.).

- Embedding & Indexing

- Convert chunks into embeddings.

- Store in a vector index (FAISS, Chroma, pgvector, or similar). Inmemory would also be fine

- Retrieval + LLM Pipeline

- Implement retrieval for user queries.

- Pass retrieved text as context to a language model (OpenAI, HuggingFace, Ollama, or another).

- Generate answers grounded in retrieved context.

### Answer Presentation

Show both:

1. the chatbot answer

2. the retrieved source text (for transparency).

## Reflection

Write a short note (in the notebook or as Markdown):

- What works well?

- Where does it fail?

- How could this be improved for real-world teacher/EdTech use?

### Example Queries

“Welche prozessbezogenen Kompetenzen zum Schreiben gibt es in Klasse 1/2?”

“Was versteht der Bildungsplan unter Lesefähigkeit in Klasse 3/4?”

“Welche Leitperspektiven berücksichtigt der Deutschunterricht?”

## Evaluation Criteria

- Functionality: Does the pipeline run end-to-end?

- Correctness: Are answers clearly based on retrieved content?

- Clarity: Is the notebook readable, structured, and documented?

- Critical Thinking: Reflection about limitations & possible improvements.

Feel free to add your thoughts to the text fields of the notebook. Making clear why which decision was made.
