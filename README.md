# WhatsApp Chat Analysis with Interest Modeling (Streamlit App)

[![Python Version](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)


## Overview

This project provides an interactive web application (built with Streamlit) to analyze your WhatsApp chat logs. It not only offers standard chat statistics and visualizations but also incorporates an interest modeling component to potentially identify key topics of discussion within your chats. The application allows you to upload your chat log, process it, and explore various insights through an intuitive user interface.

## Key Features

* **Chat Log Parsing:** Processes exported WhatsApp chat log files (`.txt` format) using `chat_parser.py`.
* **Comprehensive Statistics:** Calculates total messages, words, media shared, active participants, and their contributions.
* **Time-Based Analysis:** Visualizes message frequency over time (daily, weekly, monthly) within the Streamlit app.
* **Word and Emoji Frequency:** Displays the most frequently used words and emojis.
* **Interest Modeling:** Leverages a pre-trained machine learning model (`interest_model.pkl`) to infer potential topics of interest within the chat.
* **Interactive Streamlit Interface:** Provides an easy-to-use web application for uploading chat logs and exploring the analysis results.
* **Instructions Page:** Includes a dedicated page (`pages/1_Instructions.py`) within the Streamlit app to guide users on how to export and upload their chat logs.
* **Model Training (Separate Script):** Includes `model_trainer.py` for training or updating the interest modeling component.

## Installation

1.  **Clone the repository:**
    ```bash
    git  clone https://github.com/nathanmendis/whatsappchat-analysis
    cd your-repo-name
    ```

2.  **Install the required dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
    *(Note: The `requirements.txt` file should list libraries such as `streamlit`, `pandas`, `matplotlib`, `seaborn`, `wordcloud`, `emoji`, `scikit-learn` or any other libraries used in your scripts.)*

## Usage

1.  **Export your WhatsApp chat log:**
    * Open the specific chat in WhatsApp on your phone.
    * Tap on the three vertical dots (menu).
    * Select "More" and then "Export chat".
    * Choose "Without media" to speed up the process (or "Include media" if the application supports media analysis).
    * Save the exported `.txt` file to a location accessible by your computer.

2.  **Run the Streamlit application:**
    ```bash
    streamlit run streamlit_app.py
    ```

3.  **Interact with the application:**
    * Open your web browser to the address displayed in the terminal (usually `http://localhost:8501`).
    * Follow the instructions on the "Instructions" page to upload your chat log file.
    * Explore the various analysis and visualization tabs within the Streamlit application.

## Project Structure
