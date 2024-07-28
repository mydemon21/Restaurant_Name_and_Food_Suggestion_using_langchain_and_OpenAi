# Restaurant_Name_and_Food_Suggestion_using_langchain_and_OpenAi

This project uses LangChain and OpenAI to generate creative restaurant names and menu suggestions based on different cuisines. The application provides a simple web interface using Streamlit for users to interact and generate names and menu items.

## Features

- **Generate Restaurant Names**: Suggests unique and creative restaurant names based on the selected cuisine.
- **Menu Item Suggestions**: Provides a list of potential menu items that match the generated restaurant name.

## Requirements

- Python 3.x
- Libraries:
  - `streamlit`
  - `langchain`
  - `openai`

## Installation

1. **Clone the repository**:

    ```bash
    git clone <your-repository-url>
    cd <your-repository-folder>
    ```

2. **Install dependencies**:

    Create a virtual environment (optional but recommended):

    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

    Install the required libraries:

    ```bash
    pip install -r requirements.txt
    ```

3. **Set Up API Keys**:

    Open `my_api.py` and add your OpenAI API key:

    ```python
    openapi_key = "your_openai_api_key"
    serpapi_key = "your_serpapi_key"  # if needed
    ```

    Alternatively, you can set the API key as an environment variable:

    ```bash
    export OPENAI_API_KEY="your_openai_api_key"
    ```

## Model Description

The application uses LangChain to interact with OpenAI's language models for generating restaurant names and menu items. Here’s a brief overview of how the model integration works:

1. **LangChain Integration**:
    - **Restaurant Name Generation**: A prompt template is used to generate creative restaurant names based on the selected cuisine.
    - **Menu Item Suggestion**: A subsequent prompt uses the generated restaurant name to suggest relevant menu items.

2. **Process Flow**:
    - **Input Handling**: The application takes user input for cuisine type via the Streamlit interface.
    - **Prompting and Response**: LangChain processes the input through predefined templates and sends it to OpenAI's API to get responses.
    - **Output Display**: The generated names and menu items are displayed to the user.

## Usage

1. **Run the application**:

    ```bash
    streamlit run main.py
    ```

2. **Using the application**:
   - Select a cuisine from the sidebar dropdown.
   - The application will generate and display a restaurant name along with a list of menu items.

## Notes

- Ensure your API keys are secure and not exposed in public repositories.
- You may need to adjust settings or paths in the code according to your environment.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

Special thanks to the creators of Streamlit and LangChain for providing powerful tools for building language-based applications.

## Author

Sajal Patel

