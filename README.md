# Talk to Data (CSV Agent)

Welcome to the **Talk to Data (CSV Agent)** project! This Google Colab notebook empowers you to interact with your CSV data using natural language. Powered by **Google's Gemini 1.5 Flash** and **LangChain**, it allows you to ask questions, analyze data, and generate visualizations effortlessly without writing complex code.

## 🚀 Features

*   **Natural Language Queries**: Ask questions about your data in plain English (e.g., "What is the average age?", "Show me the distribution of sales").
*   **Automated Visualization**: The agent can automatically generate and display charts (Matplotlib/Seaborn) based on your queries.
*   **Data Analysis**: Leverages the power of Pandas to perform data manipulation and calculations.
*   **Interactive Interface**: Simple input loop to ask multiple follow-up questions.
*   **Secure API Key Management**: Uses Google Colab's strict Secrets management for your API key.

## 🛠️ Prerequisites

Before you begin, ensure you have the following:

1.  **Google Account**: To access Google Colab.
2.  **Google Gemini API Key**: You need an API key from Google AI Studio. Get one [here](https://aistudio.google.com/app/apikey).

## ⚙️ Installation & Setup

1.  **Open the Notebook**:
    Open the `Talk_to_Data_CSV_Agent.ipynb` file in Google Colab.

2.  **Set up API Key**:
    *   In the sidebar on the left, click on the **Secrets** (key icon) tab.
    *   Add a new secret with the name `GOOGLE_API_KEY`.
    *   Paste your Gemini API Key into the "Value" field.
    *   Toggle the "Notebook access" switch to enable access.

3.  **Install Dependencies**:
    The first cell of the notebook contains commands to install all necessary Python libraries. Run this cell to set up the environment.

## 📖 Usage

1.  **Run All Cells**:
    You can run the cells sequentially.
    *   **Imports & Configuration**: Loads libraries and configures the Gemini API.
    *   **File Upload**: Run the file upload cell. Click "Choose Files" and select your CSV file from your local machine.
    *   **Data Preview**: The notebook will load your CSV into a Pandas DataFrame and display the first few rows.
    *   **Agent Initialization**: Initializes the LangChain Pandas Dataframe Agent with the Gemini model.

2.  **Ask Questions**:
    *   Scroll down to the interactive loop section.
    *   Enter your question in the input box (e.g., "Plot a histogram of the 'Age' column").
    *   The agent will process your query, display the answer, and show any generated plots.

3.  **Exit**:
    *   Type `exit` or `quit` in the input box to stop the agent.

## 🧰 Tech Stack

*   **[Google Colab](https://colab.research.google.com/)**: Interactive development environment.
*   **[LangChain](https://www.langchain.com/)**: Framework for building LLM applications.
*   **[Google Gemini API](https://ai.google.dev/)**: Large Language Model (`gemini-flash-lite-latest`).
*   **[Pandas](https://pandas.pydata.org/)**: Data analysis and manipulation.
*   **[Matplotlib](https://matplotlib.org/)** & **[Seaborn](https://seaborn.pydata.org/)**: Data visualization.
