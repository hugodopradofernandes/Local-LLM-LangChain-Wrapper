# LangChain_Wrapper_LocalLLM

Wrapper to chat with a local llm, sending custom content: Webpages, PDFs, Youtube video transcripts.

Oobabooga [Text Generation Web Ui] install is not covered here!!!

This it just a test using with [oobabooga/text-generation-webui](https://github.com/oobabooga/text-generation-webui) api, all running locally.

I added an option to upload multiple PDF files at once, updated Oobabooga api endpoints, changed some limits and more!

The chat on the main page uses ConversationSummaryMemory to keep context.

![screenshot](https://github.com/hugodopradofernandes/LangChain_Wrapper_LocalLLM/blob/main/screenshots/Screenshot_20240222_051136.png)
![screenshot](https://github.com/hugodopradofernandes/LangChain_Wrapper_LocalLLM/blob/main/screenshots/Screenshot_20240222_051021.png)
![screenshot](https://github.com/hugodopradofernandes/LangChain_Wrapper_LocalLLM/blob/main/screenshots/Screenshot_20240222_050925.png)
![screenshot](https://github.com/hugodopradofernandes/LangChain_Wrapper_LocalLLM/blob/main/screenshots/Screenshot_20240222_050737.png)
![screenshot](https://github.com/hugodopradofernandes/Local-LLM-LangChain-Wrapper/blob/main/screenshots/Screenshot_20240223_020138.png)

# To install

1. clone repository
2. create a Conda environment (or venv)
3. install the requirements

# To run 

1. Start your oobabooga-api # Oobabooga [Text Generation Web Ui] install is not covered here!!!
2. Activate your conda environment (or venv)
3. Run start_linux.sh (or run "streamlit run HomePage.py")

# Embeddings model

This solution uses this model for embeddings [flax-sentence-embeddings/all_datasets_v4_MiniLM-L6](https://huggingface.co/flax-sentence-embeddings/all_datasets_v4_MiniLM-L6), which will be download on first run to the huggingface cache.

# Credits

_It started as a fork from https://github.com/sebaxzero/LangChain_PDFChat_Oobabooga_
