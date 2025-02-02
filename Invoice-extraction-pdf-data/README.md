# Invoice data processing LLM RAG on CPU with Ollama and ChromaDB

### RAG runs offline on local CPU
   
1. Install the requirements: 

```
pip install -r requirements.txt
```

2. Install <a href="https://ollama.ai">Ollama</a> and pull LLM model specified in config.yml

3. Copy text PDF files to the `data` folder.
   
4. Run the script, to convert text to vector embeddings and save in Chroma vector storage: 

```
python ingest.py
```

5. Run the script, to process data with LLM RAG and return the answer: 

```
python main.py "What is the client name?"
```
