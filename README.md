# LLM_News_Research_Tool

This is a user-friendly news research tool designed for effortless information retrieval. Users can input article URLs and ask questions to receive relevant insights from the given URLs. ([Reference](https://github.com/codebasics/langchain/tree/main/2_news_research_tool_project))

![tool_screenshot](/tool_screenshot.png)

## Installation

1.Clone this repository to your local machine using:

```bash
  git clone https://github.com/hastinmodi/LLM_News_Research_Tool.git
```
2.Install the required dependencies using pip:

```bash
  pip install -r requirements.txt
```
3.Set up your OpenAI API key by creating a .env file in the project root and adding your API

```bash
  OPENAI_API_KEY=your_api_key_here
```
## Usage/Examples

1.Run the Streamlit app by executing:
```bash
streamlit run main.py
```

2.The web app will open in your browser.

- On the sidebar, you can input URLs directly.

- Initiate the data loading and processing by clicking "Process URLs."

- Observe the system as it performs text splitting, generates embedding vectors, and efficiently indexes them using FAISS.

- The embeddings will be stored and indexed using FAISS, enhancing retrieval speed.

- The FAISS index will be saved in a local file path in pickle format for future use.
- One can now ask a question and get the answer based on those news articles
- The following articles were used in the screenshot:
  - https://electrek.co/2024/01/29/tesla-defending-elon-musk-anti-union-tweet-fifth-circuit/tata-motors-mahindra-gain-certificates-for-production-linked-payouts-11281691.html
  - https://www.marketwatch.com/story/tesla-expects-capex-to-exceed-10-billion-in-2024-4dace5e2
  - https://www.teslarati.com/tesla-employee-headcount-2023/

## Project Structure

- main.py: The main Streamlit application script.
- requirements.txt: A list of required Python packages for the project.
- faiss_store_openai.pkl: A pickle file to store the FAISS index.
- .env: Configuration file for storing your OpenAI API key.