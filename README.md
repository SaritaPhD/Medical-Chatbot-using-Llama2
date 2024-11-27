# Medical-Chatbot-using-Llama2
## Project Description
This project is a medical chatbot powered by the open-source Llama 2 model and integrated with Pinecone for efficient vector search. The chatbot is designed to answer user queries based on information extracted from medical documents (PDFs). Key features include:

- Flask Web Application: Provides an interactive interface for users to input queries and receive responses.
- Llama 2 Integration: Uses the Llama 2 model for generating natural and contextually relevant answers.
- Pinecone Vector Database: Manages embeddings and performs efficient similarity search to retrieve relevant context for user queries.
- Dynamic Prompting: Customizable prompt templates ensure accurate and context-driven responses.
- Retrieval-Augmented Generation (RAG): Combines information retrieval from PDFs with generative AI to deliver precise answers.
This chatbot is optimized for medical use cases, enabling professionals or users to query medical documents with ease and accuracy.



# How to run?
### STEPS:

Clone the repository

```bash
Project repo: git clone git@github.com:SaritaPhD/Medical-Chatbot-using-Llama2.git
```

### STEP 01- Create a conda environment after opening the repository

```bash
conda create -n mchatbot python=3.8 -y
```

```bash
conda activate mchatbot
```

### STEP 02- install the requirements
```bash
pip install -r requirements.txt
```


### Create a `.env` file in the root directory and add your Pinecone credentials as follows:

```ini
PINECONE_API_KEY = "xxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
PINECONE_API_ENV = "xxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
```


### Download the quantize model from the link provided in model folder & keep the model in the model directory:

```ini
## Download the Llama 2 Model:

llama-2-7b-chat.ggmlv3.q4_0.bin


## From the following link:
https://huggingface.co/TheBloke/Llama-2-7B-Chat-GGML/tree/main
```

```bash
# run the following command
python store_index.py
```

```bash
# Finally run the following command
python app.py
```

Now,
```bash
open up localhost:
```


### Techstack Used:

- Python
- LangChain
- Flask
- Meta Llama2
- Pinecone


