# Welcome to streamlit

This is the app you get when you run `streamlit hello`, extracted as its own app.

Edit [Hello.py](./Hello.py) to customize this app to your heart's desire. ❤️

Check it out on [Streamlit Community Cloud](https://st-hello-app.streamlit.app/)

# Rules of Thumb for coding with Langchain & Ecosytem
- Don't use Memory, use a DB like Redis for conversation
- Use low-level chains (like LLMChain), not high-level chain (like ConversationalRetrievalChain) --> control everything, easy to customize
- Use VectorStore that allow hybrid search
  - Allow pre-filter by metadata

# myRAGapp
## ==== llm.py ====
python -m venv venv
source venv/bin/activate

pip install streamlit openai langchain

streamlit run llm.py --server.enableCORS false --server.enableXsrfProtection false

