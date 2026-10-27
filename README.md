\# Ofrenda 🕯️



\*\*A local-first memory altar powered by Ollama and open-weight AI.\*\*



Ofrenda is a small experimental project inspired by Día de los Muertos. Add meaningful memories as candles, ask questions about them, and let a local AI model help you recall what you've saved.



\## Features



\- 🕯️ Add and save personal memories as candles

\- 💬 Ask questions about saved memories

\- 🧠 Uses Ollama to run an AI model locally

\- 🔒 Keeps memories in browser local storage and sends selected memories to the local Ollama service

\- ✨ Highlights candles relevant to a question

\- 🌱 Responds when it cannot find a relevant saved memory



\## Requirements



\- Python 3

\- \[Ollama](https://ollama.com/)

\- A supported Ollama model, such as `llama3.2:3b`



\## Run locally



1\. Install Ollama and download the model:



&#x20;  ```powershell

&#x20;  ollama pull llama3.2:3b

&#x20;  ```



2\. Open PowerShell in the project directory and start a local web server:



&#x20;  ```powershell

&#x20;  python -m http.server 8000 --bind 127.0.0.1

&#x20;  ```



3\. Open `http://127.0.0.1:8000/ofrenda.html` in your browser.



4\. Make sure Ollama is running and the app's model field matches the installed model name.



If the browser blocks requests to Ollama, configure Ollama's allowed origins for the local address, then restart Ollama.



\## Privacy notes



Ofrenda is designed for local use. Memories are stored in your browser's local storage, and selected memories are sent to the local Ollama service to generate answers. Browser local storage is not encrypted, and this setup should not be treated as a secure vault.



\## Limitations



Memory matching and answer checks use lightweight text-based heuristics. They can miss relevant memories or reject valid answers, and they cannot guarantee that every AI response is accurate.



\## License



No license has been added yet. Contact the repository owner before reusing this project unless a license is added.



