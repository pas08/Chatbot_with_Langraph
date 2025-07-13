# Chatbot_with_Langraph

A simple chatbot built using [LangGraph](https://github.com/langchain-ai/langgraph), [LangChain](https://github.com/langchain-ai/langchain), and [Groq](https://groq.com/) LLMs.

## Features

- Uses LangGraph for stateful conversational flows
- Integrates Groq's Gemma2-9b-it model via LangChain
- Supports streaming responses
- Easy to extend with new nodes and edges

## Setup

1. **Install dependencies:**
    ```bash
    pip install langgraph langsmith langchain langchain_groq langchain_community
    ```

2. **Set up API keys:**
    - `groq_api_key` for Groq LLM
    - `langsmith_api_key` for LangSmith tracing (optional)

3. **Configure environment:**
    ```python
    import os
    os.environ["LANGCHAIN_API_KEY"] = "<your_langsmith_api_key>"
    os.environ["LANGCHAIN_TRACING_V2"] = "true"
    os.environ["LANGCHAIN_PROJECT"] = "CourseLanggraph"
    ```

## Usage

Run the notebook `Chatbot_with_Langraph.ipynb` and follow the prompts.  
Type your message and get responses from the assistant.  
Type `quit` or `q` to exit.

## Example

```
User: Hello!
Assistant: Hi! How can I help you today?
```

## Customization

- Add new nodes or edges to the graph for more complex workflows.
- Swap out the LLM model by changing the `model_name` parameter.

## License