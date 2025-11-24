# Morse Code Translator

## Overview
The Morse Code Translator is a Python-based command-line interface (CLI) tool designed to facilitate communication using standard Morse code. This project allows users to encode regular text into Morse code patterns and decode Morse code sequences back into readable English text. It serves as a practical application of string manipulation, dictionary mapping, and user input handling in Python.

## Features
* **Text-to-Morse Conversion:** Instantly converts alphanumeric characters and punctuation into their corresponding Morse code representations.
* **Morse-to-Text Conversion:** Decodes Morse code strings back into readable text, intelligently handling character and word spacing.
* **Interactive Menu System:** A continuous loop interface that allows users to perform multiple translations without restarting the program.
* **Input Validation:** Includes checks for empty inputs and invalid menu choices to ensure a smooth user experience.
* **Comprehensive Symbol Map:** Supports letters (A-Z), numbers (0-9), and common punctuation marks.

## Technologies/Tools Used
* **Programming Language:** Python 3.x
* **Libraries:** Standard Python Library (no external dependencies required)

## Steps to Install & Run the Project
1.  **Prerequisites:** Ensure you have Python installed on your machine. You can verify this by typing `python --version` in your terminal.
2.  **Download:** Save the file `Morse Code Translator 3.py` to a local directory.
3.  **Run the Application:**
    * Open your terminal or command prompt.
    * Navigate to the directory where the file is saved.
    * Execute the following command:
        ```bash
        python "Morse Code Translator 3.py"
        ```

## Instructions for Testing
To verify the functionality of the project, follow these test cases:

**Test Case 1: Text to Morse**
1.  Run the program and select Option **1**.
2.  Enter the text: `HELLO WORLD`
3.  **Expected Output:** `.... . .-.. .-.. --- / .-- --- .-. .-.. -..`

**Test Case 2: Morse to Text**
1.  Run the program and select Option **2**.
2.  Enter the code: `... --- ...`
3.  **Expected Output:** `SOS`

**Test Case 3: Invalid Input**
1.  Run the program.
2.  When asked for a choice, enter `5`.
3.  **Expected Output:** `Hmm, that's not a valid option. Try 1, 2, or 3.`
