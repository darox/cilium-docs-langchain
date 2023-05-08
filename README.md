# Cilium Docs Langchain

A huge drawback of LLMs is their outdated knowledge. This is because they are trained on a static dataset. This is a problem for Cilium because it is constantly being updated.
But there are some ways to overcome this problem. This repository is an attempt to use LLMs like OpenAI's [GPT-3](https://openai.com/product) and [Pinecone](https://www.pinecone.io/) vector database for Cilium documentation.


## How to use

This is more of a proof-of-concept than a fully functional application. Thus it only consists of a jupyter notebook. The notebook will guide you through the process.

Note: For the proof of concept I'm only scraping the docs for Cilium v1.13.x.


## How it works

1. Scrape the docs
2. Tokenize the scraped docs
3. Create OpenAI embeddings 
4. Create Pinecone index
5. Load embeddings into Pinecone index
6. Now you can query GPT with augmented queries


All of this is mostly based on https://github.com/pinecone-io/examples/blob/master/generation/gpt4-retrieval-augmentation/gpt-4-langchain-docs.ipynb


