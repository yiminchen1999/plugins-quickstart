# ChatGPT plugins quickstart

Get a todo list ChatGPT plugin up and running in under 5 minutes using Python. This plugin is designed to work in conjunction with the [ChatGPT plugins documentation](https://platform.openai.com/docs/plugins). If you do not already have plugin developer access, please [join the waitlist](https://openai.com/waitlist/plugins).

## Setup locally

To install the required packages for this plugin, run the following command:

```bash
pip install -r requirements.txt
```
```bash
pip install numpy
pip install matplotlib
pip install quart
pip install quart-cors
pip install langchain
pip install openai
pip install PyPDF2
pip install faiss-cpu
pip install tiktoken
pip install PyDrive
pip install streamlit 
pip install langchain
pip install openai
```

To run the plugin, enter the following command:

```bash
python main.py
```

Once the local server is running:

1. Navigate to https://chat.openai.com. 
2. In the Model drop down, select "Plugins" (note, if you don't see it there, you don't have access yet).
3. Select "Plugin store"
4. Select "Develop your own plugin"
5. Enter in `localhost:5003` since this is the URL the server is running on locally, then select "Find manifest file".

The plugin should now be installed and enabled! You can start with a question like "What is on my todo list" and then try adding something to it as well! 

## Setup remotely

### Cloudflare workers
