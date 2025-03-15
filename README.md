# AI agents using LLMs
The repository will let you use AI agents using different LLMs.

![logo_SAK_15](https://github.com/user-attachments/assets/e6b86e25-8a3e-443a-965f-efff77aea8ab)


# Pre-requisites

Firstly, you have to install Ollama on your local machine. The instructions are available on their [official website](https://ollama.com/). Once installed, you can pull Llama 3.3, DeepSeek-R1, Phi-4, Mistral, Gemma 2, and other models, locally. 

For pulling the deepseek model use the following command. 

```  ollama pull deepseek-r1:8b ```

Install all the packages that are required using pip:

```  pip install -r requirements.txt  ```

In order to run the agents you need to add the Tavily API Key. In order to do that, you need to run the following code:

```  export TAVILY_API_KEY = "YOUR_API_KEY"  ```

The API Key will allow you 1000 credits to perform the search.

For the stock analyst agent, the repository uses OPEN AI, therefore you can run the following code:

```  export OPENAI_API_KEY = "YOUR_API_KEY"  ```

For Multimodal Chatbot you have to get your Google Studio API Key

Sign Up for the API Key at [Google AI Studio](https://aistudio.google.com/app/apikey)

Add your API Key to the multimodal_chatbot_gemini.py line 12. 

You can then run your desired agent by running the following code:

``` streamlit run <agent_type>.py   ```


# Agents

## Researcher Agent

It is a simple AI agent that uses web to match the user's query and answers by summarizing the results. The agent uses LangGraph and DeepSeek-R1 to perform the desired operation. 

## Scraper Agent

The scraper agent builds a Retrieval-Augmented Generation (RAG) system that will allow the user to chat with websites and answer complex questions about the desired content. The agent uses LangChain and Ollama.

## PDF Chat Agent

The PDF Chat Agent creates a simple RAG system lets the user chat with the PDFs and answer complex questions about your local documents. The agent uses LangChain and DeepSeek. For this agent, you need to upload the PDFs in the pdfs folder.  

## Stock_Analyst_Agent



I will update more changes so look out for this repository.


# Feel free to use the codes :) 
