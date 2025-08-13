#  🤖 AI Water Tracker

Welcome to the AI Water Tracker! This project helps you monitor your daily water intake with the assistance of an AI agent, providing smart feedback to keep you hydrated and healthy effortlessly.

[![Python 3.8+](https://img.shields.io/badge/python-3.8%2B-blue.svg)](https://www.python.org/)
[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://streamlit.io/)
![LangChain](https://img.shields.io/badge/LangChain-0.1.12-23A562?logo=langchain&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI-1.14.1-412991?logo=openai&logoColor=white)
![LlamaIndex](https://img.shields.io/badge/LlamaIndex-latest-red?logo=llama-index&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-0.109.2-009688?logo=fastapi&logoColor=white)
![Uvicorn](https://img.shields.io/badge/Uvicorn-0.27.0.post1-F70000?logo=uvicorn&logoColor=white)
![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-2.0.27-A34E28?logo=sqlalchemy&logoColor=white)
![SQLite Utils](https://img.shields.io/badge/sqlite--utils-3.35-FFC107?logo=sqlite&logoColor=white)
![Python Dotenv](https://img.shields.io/badge/python--dotenv-1.0.1-F7DF1E?logo=python&logoColor=white)
![Loguru](https://img.shields.io/badge/Loguru-0.7.2-2ECC71?logo=python&logoColor=white)
![APScheduler](https://img.shields.io/badge/APScheduler-3.10.4-orange?logo=python&logoColor=white)
![Typer](https://img.shields.io/badge/Typer-0.9.0-00ADD8?logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-lightgrey?logo=pandas&logoColor=white)

---

## ✨ Features

* **Log Water Intake**: Easily record your daily water consumption in milliliters.
* **AI-Powered Feedback**: Get intelligent insights and feedback on your hydration habits from an integrated AI assistant.
* **Intake History**: View your past water intake data in a clear, interactive dashboard.
* **Data Visualization**: See your hydration trends over time with intuitive charts.

---

## 🛠️ Technologies Used

The AI Water Tracker is built using the following technologies:

* **Frontend**:
    * **Streamlit**: For creating an interactive and user-friendly web interface.
* **Backend & AI**:
    * **Langchain**: An LLM framework for developing the AI agent.
    * **OpenAI**: Powers the AI's language capabilities (via OpenRouter API).
    * **FastAPI**: A modern, fast (high-performance) web framework for building APIs.
    * **Uvicorn**: An ASGI server for running the FastAPI application.
* **Database**:
    * **SQLite**: A lightweight, file-based database for storing water intake data.
    * **SQLAlchemy**: An SQL toolkit and Object-Relational Mapper (ORM) for Python.
    * **sqlite-utils**: A Python library for working with SQLite databases.
* **Other**:
    * **python-dotenv**: For managing environment variables.
    * **Loguru**: For simplified logging and debugging.
    * **APScheduler**: For task scheduling (e.g., for reminders, though not fully implemented in provided files).
    * **Typer**: (Optional) For building command-line interfaces.
    * **Pandas**: For data manipulation and analysis in the dashboard.

---

## 🚀 Getting Started

Follow these steps to set up and run the AI Water Tracker on your local machine.

### Prerequisites

* Python 3.8+
* `pip` (Python package installer)

### Installation

1.  **Clone the repository (if applicable):**
    ```bash
    git clone <repository_url>
    cd water-intake-agent
    ```
    (Note: As the project was provided as files, this step assumes it's part of a larger repository. If not, simply ensure all files are in a single directory.)

2.  **Create a virtual environment (recommended):**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3.  **Install the required dependencies:**
    The `requirements.txt` file lists all necessary libraries.
    ```bash
    pip install -r requirements.txt
    ```

4.  **Set up environment variables:**
    Create a `.env` file in the root directory of your project and add your `OPENAI_API_KEY` and `DATABASE_URL`.
    ```dotenv
    OPENAI_API_KEY="your_openrouter_api_key_here"
    DATABASE_URL=sqlite:///water-tracker.db
    ```
    *Replace `"your_openrouter_api_key_here"` with your actual API key from OpenRouter.*

### Running the Application

1.  **Run the Streamlit Dashboard:**
    ```bash
    streamlit run dashboard.py
    ```
    This command will open the AI Water Tracker dashboard in your web browser.

## 🚀 Usage

1.  **Start Tracking**: Click the "Start Tracking" button on the welcome page.
2.  **Enter User ID**: Provide a unique user ID in the sidebar. The default is `user_123`.
3.  **Log Water Intake**: Enter the amount of water (in ml) you've consumed and click "Submit".
4.  **View Feedback and History**: The dashboard will display AI feedback and update your intake history, including a line chart visualizing your progress.

---
