# RAG-Chatbot-Bedrock
Here's a polished and attractive `README.md` for your GitHub repository based on your project *"Set Up a RAG Chatbot in Bedrock"* using the content from the provided PDF:

---

# 🤖 Legendary AI RAG Chatbot with Amazon Bedrock

A hands-on project demonstrating how to build a **Retrieval Augmented Generation (RAG)** chatbot powered by **Amazon Bedrock**, **S3**, and **OpenSearch Serverless**. This chatbot responds using custom knowledge—your own documents!

## 🚀 Project Overview

RAG (Retrieval Augmented Generation) is an AI technique that **enhances LLM responses by retrieving relevant content from a knowledge base** (KB). In this project, we set up a full-stack RAG chatbot on AWS, linking documents in **S3**, a **vector store**, and **AI models on Bedrock**.

> 📚 This project was created as a learning journey to explore Amazon Bedrock, Knowledge Bases, and vector-based search systems.

---

## 🛠️ Tools & Services Used

| Service                      | Purpose                                                 |
| ---------------------------- | ------------------------------------------------------- |
| **Amazon Bedrock**           | Access and use foundation models from various providers |
| **Amazon S3**                | Store knowledge documents                               |
| **OpenSearch Serverless**    | Vector store to enable semantic search                  |
| **Titan Text Embeddings v2** | Used to embed documents into vectors                    |

---

## 🧠 How It Works

1. **Upload Documents to S3**

   * Upload your `.pdf`, `.txt`, etc., into an S3 bucket (in the same region as your Bedrock KB).

2. **Create a Knowledge Base**

   * Connect your S3 bucket to Amazon Bedrock.
   * Configure chunking (\~300 tokens) for better embedding and search accuracy.

3. **Sync the KB**

   * Ingest → Chunk → Embed → Store (in OpenSearch vector store).

4. **Connect to a Bedrock AI Model**

   * Request model access.
   * We used **LLaMA 3.3 70B** (since 8B was unavailable on demand).

5. **Test the Chatbot**

   * Ask questions! The bot pulls relevant data chunks and generates human-like answers.
   * You can also view raw KB responses by turning off "Generate Response".

---

## 📸 Demo Preview

> *"Ask the chatbot a question and see it respond based solely on the documents you’ve provided."*
> It won’t hallucinate extra data—it only knows what it’s fed.

---

## 🧩 Key Concepts Learned

* RAG (Retrieval Augmented Generation)
* Semantic vector search
* Chunking and embedding text
* AI model provisioning in AWS
* Document-grounded AI conversations

---

## ⏱️ Time & Reflections

🕒 Total time: \~2 hours
💡 Challenge: AI model access and inference mode (on-demand vs. pre-provisioned)
🏁 Result: A working chatbot that responds intelligently using your own knowledge base!

---

## 📎 Related Links

* 🌐 [Amazon Bedrock Documentation](https://docs.aws.amazon.com/bedrock/)
* 🧪 [NextWork Project](https://community.nextwork.org/c/i-have-a-question?automatic_login=true)

---

## 👨‍💻 Author

**Vinay Pal Singh**
[LinkedIn](https://www.linkedin.com/in/vinay-pal-singh).
---

