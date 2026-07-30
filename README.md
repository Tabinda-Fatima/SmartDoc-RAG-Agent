# SmartDoc RAG Agent

An AI-powered document question-answering workflow built with **n8n**, **OpenAI**, and **Supabase Vector Database**.

The workflow processes large PDF documents, divides their content into smaller chunks, creates vector embeddings, and stores them in Supabase. When a user asks a question, the system retrieves the most relevant document context and generates an accurate, context-aware response.

---

## Problem It Solves

Finding specific information inside long documents, research papers, reports, and books can be time-consuming.

SmartDoc RAG Agent automates this process by using Retrieval-Augmented Generation (RAG). Instead of manually searching through an entire document, users can ask questions and receive answers based on the most relevant document content.

---

## Features

- Processes large PDF documents
- Automatically divides documents into manageable chunks
- Generates vector embeddings using OpenAI
- Stores document embeddings in Supabase Vector Database
- Retrieves relevant document context
- Generates context-aware answers
- Reduces manual document searching
- Fully automated through n8n
- Supports document-based question answering

---

## How RAG Works

The workflow follows a Retrieval-Augmented Generation process:

1. A PDF document is loaded into the workflow.
2. The document text is divided into smaller chunks.
3. OpenAI generates embeddings for each chunk.
4. The embeddings are stored in Supabase Vector Database.
5. The user submits a question about the document.
6. Supabase retrieves the most relevant document chunks.
7. The AI model uses the retrieved context to generate an answer.

---

## Workflow Architecture

```text
PDF Document
     ↓
Document Loader
     ↓
Text Splitter
     ↓
OpenAI Embeddings
     ↓
Supabase Vector Store
     ↓
User Question
     ↓
Relevant Context Retrieval
     ↓
AI-Generated Answer
```

---

## Tech Stack

- n8n
- OpenAI
- OpenAI Embeddings
- Supabase
- Supabase Vector Database
- Retrieval-Augmented Generation
- PDF Document Processing

---

## Workflow Screenshot

The n8n workflow responsible for processing documents, generating embeddings, storing vectors, retrieving relevant context, and generating answers.

![SmartDoc RAG Agent Workflow](RAG%20Agent.jpg)

---

## Use Cases

SmartDoc RAG Agent can be used to:

- Explore information from long books
- Analyze research papers
- Review business reports
- Extract insights from government documents
- Search technical documentation
- Build document-based AI assistants
- Create internal knowledge-base chatbots
- Reduce manual reading and searching time

---

## Benefits

- Faster access to document information
- Context-aware responses
- Reduced manual document searching
- Reusable vector-based knowledge storage
- Scalable document question-answering workflow
- Improved productivity when working with large files

---

## Setup Instructions

### 1. Import the Workflow

Import the workflow JSON file into your n8n instance.

### 2. Configure OpenAI

Add your OpenAI API credentials to the required OpenAI nodes.

### 3. Configure Supabase

Connect your Supabase account and configure the required vector database table.

### 4. Upload a Document

Provide the PDF document that will be processed and stored in the vector database.

### 5. Run the Workflow

Execute the workflow to divide the document into chunks, generate embeddings, and store them in Supabase.

### 6. Ask Questions

Submit questions related to the uploaded document. The workflow will retrieve relevant context and generate an answer.

---

## Security Note

Credentials and API keys are not included in this repository.

Users must configure their own:

- OpenAI API credentials
- Supabase credentials
- n8n credentials and connections

---

## Author

**Tabinda Fatima**

AI Automation & Workflow Developer
