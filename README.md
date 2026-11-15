# AI Escape Room – The Forgotten Library

## 1. Project Overview

The AI Escape Room is an interactive game developed using Python, Streamlit and Google's Gemini AI.

The player wakes up inside a mysterious library and must investigate objects, solve puzzles, collect clues and unlock the exit door.

The project contains two versions that demonstrate the improvement of the application.

## 2. Technologies Used

- Python
- Streamlit
- Google Gemini API
- Google GenAI Python SDK
- Python-dotenv
- Git and GitHub

## 3. Project Structure

```text
AI-Escape-Room/
│
├── version1.py
├── version2.py
├── game_logic.py
├── requirements.txt
├── .env.example
├── .gitignore
└── README.md
```

## 4. Version 1 – Basic AI Escape Room

Version 1 provides a basic conversational escape room experience.

Features:
- Interactive chat interface.
- Gemini AI integration.
- Library environment and story.
- Three puzzles.
- Final four-digit exit code.
- Restart game functionality.

## 5. Version 2 – Improved AI Escape Room

Version 2 improves the original application by introducing additional game management features.

Improvements:
- Player inventory system.
- Brass key collection.
- Puzzle progress tracking.
- Locked drawer functionality.
- Exit door validation.
- Improved game logic.
- Final escape confirmation.

## 6. Installation

Clone the repository:

```bash
git clone https://github.com/Abhiramkunchala/AI-Escape-Room.git

Navigate to the project folder:

```bash
cd AI-Escape-Room

Install dependencies:

```bash
pip install -r requirements.txt

Create a `.env` file and configure:

```env
GEMINI_API_KEY=your_api_key
GEMINI_MODEL=gemini-3.5-flash-lite

## 7. Run the Application

Run Version 1:

```bash
streamlit run version1.py

Run Version 2:

```bash
streamlit run version2.py

## 8. Game Objective

The objective is to solve three puzzles, collect the brass key, open the locked drawer, discover the final code and escape the Forgotten Library.

## 9. Development

Version 1 was developed as the initial conversational prototype. Version 2 introduced structured game progress, inventory management and additional validation to improve the gameplay experience.

## 10. Author

AI Escape Room – Academic Project

Developed as part of the course assignment on AI Escape Room and GitHub Portfolio.
