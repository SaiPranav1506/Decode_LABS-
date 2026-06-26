# Wisp Bot: A Rule-Based AI Chatbot
## Project Overview

**Wisp Bot** is a sophisticated rule-based chatbot designed as part of the DecodeLabs Industrial Training Kit. It demonstrates fundamental concepts of Natural Language Processing (NLP) and Artificial Intelligence, including fuzzy matching, pattern recognition, and context-aware response generation.

This chatbot is built to understand user intents, respond dynamically, remember user information, and provide insightful analytics on conversation patterns.

## Features

-   **Intent-Based Responses:** Uses a structured `KNOWLEDGE_BASE` to match user queries to predefined intents (e.g., greetings, jokes, AI concepts).
-   **Fuzzy Matching:** Employs `difflib.SequenceMatcher` to handle misspellings and variations in user input, ensuring robust pattern recognition.
-   **Context Memory:** Remembers the user's name to personalize future interactions.
-   **Conversation History & Analytics:** Tracks conversation flow, intent usage, and recognition rates, visualized through `matplotlib` charts.
-   **Interactive UI:** Powered by `Gradio`, providing a user-friendly web interface for real-time interaction.
-   **Extensible Knowledge Base:** Easily add or modify intents and responses to expand the bot's capabilities.

## Installation & Setup

To run Wisp Bot, you'll need Python and the necessary libraries. This project is designed to run seamlessly in a Google Colab environment.

1.  **Clone the Repository (if applicable):**
    ```bash
    git clone <your-repo-url>
    cd <your-repo-name>
    ```

2.  **Open in Google Colab:**
    If you're using Colab, simply upload the `.ipynb` notebook to your Colab environment.

3.  **Install Dependencies:**
    The notebook includes a cell to install `gradio`:
    ```python
    !pip install -q gradio
    ```
    Run this cell to ensure all dependencies are met.

## How to Run

Once the notebook is open in Colab and dependencies are installed, you can run the Wisp Bot in a few steps:

1.  **Execute Cells Sequentially:** Run all cells in the notebook from top to bottom.
    -   The `KNOWLEDGE_BASE` cell (`mXYVKJq03cNz`) defines the bot's responses.
    -   The `preprocess` function cell (`a464QFmA3cN5`) sets up text cleaning.
    -   The `WispBot` class cell (`_TUhWSJA3cOA`) defines the bot's core logic.
    -   The `Conversation Demo` cell (`DtCLmkQq3cOD`) provides a textual walkthrough of the bot's capabilities.
    -   The `Conversation Analytics` cell (`rB_4aavQ3cOJ`) visualizes the intent distribution and timeline of the demo conversation.
    -   The `Interactive Gradio App` cell (`_2V7iklo3cOp`) launches the live chatbot interface.

2.  **Interact with the Gradio App:**
    After running the last cell (`_2V7iklo3cOp`), a Gradio interface will appear directly in your Colab output, along with a public URL. You can use this URL to share your chatbot or interact with it in a separate browser tab.

    **Example interactions:**
    -   "Hello!"
    -   "My name is Alex"
    -   "What can you do?"
    -   "Tell me a joke"
    -   "What is AI?"
    -   "I'm feeling bored"
    -   "Bye!"

## Customization

-   **Modify `KNOWLEDGE_BASE`:** To add new functionalities or change existing responses, edit the `KNOWLEDGE_BASE` dictionary in cell `mXYVKJq03cNz`.
-   **Adjust Preprocessing:** The `preprocess` function in cell `a464QFmA3cN5` can be modified for different text normalization needs.
-   **Enhance `WispBot` Logic:** The `WispBot` class in cell `_TUhWSJA3cOA` can be extended to implement more complex AI logic or integrate with external APIs.
-   **Update Visualizations:** The `Conversation Analytics` cell (`rB_4aavQcOJ`) can be customized to generate different types of charts or more detailed reports.
