# Restaurant_Name_and_Food_Suggestion_using_langchain_and_OpenAi

This project uses LangChain and OpenAI to generate creative restaurant names and menu suggestions based on different cuisines. It is implemented using Streamlit for the user interface and LangChain for language processing.

## Features

- **Generate Restaurant Names**: Suggests unique and creative restaurant names based on the selected cuisine.
- **Menu Item Suggestions**: Provides a list of potential menu items that match the generated restaurant name.

## Files

1. **`main.py`**
   - This file contains the Streamlit application.
   - Users can select a cuisine from a sidebar, and the app will display a generated restaurant name and menu items.

2. **`automate.py`**
   - Contains the logic for generating restaurant names and menu items.
   - Utilizes LangChain to process prompts and OpenAI's language model to generate responses.
   - Requires an API key for OpenAI, which should be set in the environment.

3. **`my_api.py`**
   - A placeholder file for storing API keys.
   - Ensure you have your OpenAI API key and, if applicable, a SerpAPI key stored here.

## Getting Started

To run the project, follow these steps:

1. **Clone the repository**:
   ```bash
   git clone <your-repository-url>
   cd <your-repository-folder>
   
2. **Installation**:

To install the required packages, run the following command:

```bash
pip install -r requirements.txt

3. **Set up API keys**:

Open `my_api.py` and add your OpenAI API key:

```python
openapi_key = "your_openai_api_key"
serpapi_key = "your_serpapi_key"  # if needed

