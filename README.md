# NLP_ReAct_RAG_Project

## Google Colab Notebook

The project notebook can be accessed here:
[https://colab.research.google.com/XXXXXXXX](https://colab.research.google.com/drive/1NTprQQ6m5G-q-GCYAG9EW5amYFUPpQBM#scrollTo=xdfnIhCgnf0I)


This project implements a ReAct (Reasoning + Acting) based Retrieval-Augmented Generation (RAG) system
for answering legal questions related to distance sales contracts and the right of withdrawal in Turkey.

## Dataset
The system operates exclusively on two PDF documents:
- on-bilgilendirme-formu.pdf
- cayma_hakki_akademik.pdf

## Method
- PDF text extraction with PyMuPDF
- Chunk-based retrieval
- ReAct agent with tool usage
- Source-cited answers (PDF name and page number)

## Benchmark
- 50 questions in total
  - 40 dataset-based questions
  - 10 reasoning-based questions
- Automatic scoring (1.0 / 0.5 / 0.0)
- Results saved as CSV files in the `results/` directory

## Models
- Llama 3.1 8B (Groq, Free)
- Gemini comparison planned but limited due to API access and quota constraints

## Reproducibility
All experiments were conducted in Google Colab.
Benchmark logs and outputs are provided in CSV format.
