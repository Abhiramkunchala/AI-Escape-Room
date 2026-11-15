# AI-Powered Escape Room – Project Report

## 1. Introduction

The AI-Powered Escape Room is an interactive game in which the player is trapped inside a locked library and must solve puzzles, collect clues, and discover a four-digit code to escape.

The project explores how Large Language Models (LLMs) can be used to create interactive gaming experiences. Google Gemini is used as the AI Game Master to provide responses and narration, while Python and Streamlit provide the application logic and user interface.

Two versions were developed. Version 1 focuses on basic AI-driven interaction, while Version 2 improves reliability by introducing structured game state and Python-based action validation.

## 2. Project Design and Implementation

### 2.1 Version 1 – Basic AI Escape Room

Version 1 was developed using Python, Streamlit, and the Gemini API.

The player interacts with the game through a chat interface. The AI acts as the Game Master and describes the library, explains objects, provides clues, and responds to player actions.

The room contains five interactive objects:

- Desk
- Bookshelf
- Painting
- Locked drawer
- Exit door

The player must investigate the objects and solve three puzzles. The clues obtained from the puzzles help the player discover the final four-digit code: **2841**.

Streamlit manages the chat interface and conversation history. Gemini generates responses based on the game instructions and previous conversation.

### 2.2 Version 2 – Reliable AI Escape Room

Version 2 was developed to address the limitations of Version 1.

The main improvement is that Python controls the actual game state and validates player actions instead of relying entirely on AI-generated responses.

A structured game state stores information such as:

- Available objects
- Player inventory
- Solved puzzles
- Collected clues
- Drawer status
- Exit door status
- Escape status

Python functions check puzzle answers, validate inventory requirements, and determine whether the player can open the drawer or escape.

Gemini is used for optional story narration. It does not decide whether a puzzle is solved or whether the player has successfully escaped.

## 3. Technologies Used

| Technology | Purpose |
|---|---|
| Python | Main programming language and game logic |
| Streamlit | Interactive web interface |
| Google Gemini API | AI narration and Game Master responses |
| Python dictionaries | Structured game-state management |
| python-dotenv | Loading environment variables |
| Git and GitHub | Version control and project portfolio |

The Gemini API key is stored in a local `.env` file. The `.env` file is excluded from Git using `.gitignore`, while `.env.example` provides an example configuration.

## 4. Testing and Results

Both versions were tested using normal game interactions and invalid actions.

The following tests were considered:

1. Attempting to use a key before collecting it.
2. Trying to open the drawer without the required key.
3. Entering an incorrect four-digit code.
4. Claiming that a puzzle is solved without providing the correct answer.
5. Asking the AI to reveal the hidden answers.
6. Completing the puzzles and entering the correct final code, 2841.

Version 1 relies on the AI's conversation and instructions, so its responses may be inconsistent.

Version 2 uses Python validation to prevent invalid actions and maintain consistent game progress. The successful escape test demonstrated that the player could complete the required steps and enter the correct code.

## 5. Challenges Faced

During development, several challenges were encountered:

- Configuring the Gemini API and selecting a model that responded successfully.
- Maintaining conversation history in Version 1.
- Handling invalid actions and incorrect puzzle answers.
- Keeping the player's inventory and puzzle progress consistent.
- Ensuring that the final door could only be unlocked after completing the required steps.
- Managing environment variables and GitHub files safely.

These challenges helped improve the implementation and the understanding of AI application development.

## 6. Improvements from Version 1 to Version 2

The main improvement was moving important game decisions from AI-generated responses into Python code.

Version 1 provides flexible conversations, but the AI may not always follow the game rules consistently.

Version 2 introduces structured state management, inventory validation, puzzle validation, and controlled escape conditions. This makes the game more reliable and predictable.

The AI remains useful for narration, while Python is responsible for the actual game rules.

## 7. Conclusion

The AI-Powered Escape Room demonstrates how an LLM can be integrated into an interactive application.

Developing two versions helped demonstrate the difference between relying entirely on AI responses and combining AI with traditional programming logic.

Version 1 provided the basic interactive experience, while Version 2 improved reliability through Python-based validation and structured state management.

The project provided practical experience with Python, Streamlit, Gemini API integration, application testing, Git, and GitHub.

**GitHub Repository:** https://github.com/Abhiramkunchala/AI-Escape-Room