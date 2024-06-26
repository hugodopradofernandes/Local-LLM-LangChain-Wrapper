# LangChain_Wrapper_LocalLLM

Wrapper to chat with a local llm, sending custom content: Webpages, PDFs, Youtube video transcripts.

This it just a test using with [oobabooga/text-generation-webui](https://github.com/oobabooga/text-generation-webui) api, all running locally.
Oobabooga [Text Generation Web Ui] install is not covered here!!! You can replace the API and then use the OpenAI(chat GPT) api instead.

Items added from forked repo, which I used as a starting point to learning how to interact with LLM API with embeddings.
- Added multiple file upload.
- Updated packages.
- Target Text Generation Web UI API endpoints updated.
- Option to query Wikipedia or URLs.
- Option to query Plain text files.
- Option to query Youtube video transcripts.
- Added a chat page, with history and context, using _ConversationSummaryMemory_.
- Many UI improvements, pratically a new app.

Works great with *WizardLM-2-7B* LLM model (tested using Q5_K_M quantized)

![screenshot](https://github.com/hugodopradofernandes/LangChain_Wrapper_LocalLLM/blob/main/screenshots/Screenshot_20240419_175425.png)
![screenshot](https://github.com/hugodopradofernandes/Local-LLM-LangChain-Wrapper/blob/main/screenshots/Screenshot_20240419_174526.png)
![screenshot](https://github.com/hugodopradofernandes/LangChain_Wrapper_LocalLLM/blob/main/screenshots/Screenshot_20240419_174647.png)

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
