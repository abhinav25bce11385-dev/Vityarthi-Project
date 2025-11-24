# Project Statement

## Problem Statement
Morse code is a legendary method of communication, but let's be honest—decoding it manually is slow, tedious, and prone to errors. Unless you are a trained telegraph operator, trying to translate a message character-by-character using a reference sheet takes the fun out of it. Currently, there is a need for a simple, lightweight tool that can instantly bridge the gap between natural language and Morse code, allowing users to encode or decode messages without the headache of manual lookup.

## Scope of the Project
This project is designed as a lightweight Command Line Interface (CLI) tool. Its primary scope is to provide accurate, two-way translation between the English alphabet (including numbers and basic punctuation) and standard International Morse Code.
* **In Scope:** Text-to-Morse conversion, Morse-to-Text conversion, handling of word/letter spacing, and a continuous user session loop.
* **Out of Scope:** Audio signal processing (sound input/output), graphical user interface (GUI), or networking features.

## Target Users
This tool is built for:
* **Students & Learners:** Those studying computer science basics (dictionaries/mappings) or the history of communication.
* **Hobbyists:** Ham radio enthusiasts or puzzle solvers who need a quick verification tool.
* **Survival/Scouts:** Individuals practicing emergency signaling who want to check the accuracy of their codes.
* **Developers:** Beginners looking for a clean example of string manipulation and logic flow in Python.

## High-Level Features
* **Bi-Directional Translation:** seamlessly converts standard text into Morse code and interprets Morse patterns back into readable English.
* **Smart Formatting:** Automatically handles the specific spacing required between individual letters and distinct words (using standard `/` notation for spaces).
* **Interactive Session:** Features a "while-loop" menu system, meaning the user can perform multiple translations in a row without having to restart the program every time.
* **Error Handling:** Includes basic validation to ensure the program doesn't crash if the user enters an empty string or an invalid menu option.
