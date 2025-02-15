# Corpus Analysis and Sentence Embeddings

## Overview
This project performs corpus analysis on legal contract documents from the CUAD dataset. It includes text preprocessing using NLTK, statistical analysis with SciPy. The second part involves uses pre-trianed LLM's to do a sentence similarity analysis with the STS Dataset

## Features
- Tokenization and stopword removal using NLTK
- Statistical correlation analysis with SciPy
- Handling and processing of legal text files
- Chatbot-based text analysis with Ollama

## Installation
Ensure you have Python installed and set up a virtual environment:
```bash
python -m venv env
source env/bin/activate  # On Windows use `env\Scripts\activate`
```

Install the required dependencies:
```bash
pip install -r requirements.txt
```

### Installing Ollama and Required LLMs

To use the language models, install Ollama first:

#### MacOS & Linux:
```bash
curl -fsSL https://ollama.com/install.sh | sh
```

#### Windows:
Download and install Ollama from the official website: [Ollama Installation](https://ollama.com/download)

After installing Ollama, pull the required models:
```bash
ollama pull llama3:3.2
ollama pull deepseek:r1:1.5
```

To use the language models, install Ollama first:

```bash
curl -fsSL https://ollama.com/install.sh | sh
```

Then, install the required models:

```bash
ollama pull llama3:3.2
ollama pull deepseek:r1:1.5
```



Create `requirements.txt` with the following dependencies:
```
annotated-types==0.7.0
anyio==4.8.0
appnope==0.1.4
asttokens==3.0.0
certifi==2024.12.14
click==8.1.8
comm==0.2.2
debugpy==1.8.12
decorator==5.1.1
executing==2.2.0
h11==0.14.0
httpcore==1.0.7
httpx==0.28.1
idna==3.10
ipykernel==6.29.5
ipython==8.31.0
jedi==0.19.2
joblib==1.4.2
jupyter_client==8.6.3
jupyter_core==5.7.2
matplotlib-inline==0.1.7
nest-asyncio==1.6.0
nltk==3.9.1
numpy==2.2.2
ollama==0.4.7
packaging==24.2
parso==0.8.4
pexpect==4.9.0
pip==24.2
platformdirs==4.3.6
prompt_toolkit==3.0.50
psutil==6.1.1
ptyprocess==0.7.0
pure_eval==0.2.3
pydantic==2.10.6
pydantic_core==2.27.2
Pygments==2.19.1
python-dateutil==2.9.0.post0
pyzmq==26.2.0
regex==2024.11.6
scipy==1.15.1
six==1.17.0
sniffio==1.3.1
stack-data==0.6.3
tornado==6.4.2
tqdm==4.67.1
traitlets==5.14.3
typing_extensions==4.12.2
wcwidth==0.2.13
```

## Usage
Run the Jupyter Notebook:
```bash
jupyter notebook corpus_analysis.ipynb
```

Make sure the CUAD dataset is available in the correct folder structure:
```
CUAD_v1/
    full_contract_txt/
        contract1.txt
        contract2.txt
        ...
```

## Dependencies
See `requirements.txt` for the full list of dependencies.