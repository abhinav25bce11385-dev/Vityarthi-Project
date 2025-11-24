# The Morse Code Translator (MCT)

> Ever wanted to talk like an old-school telegraph operator? Now you can!

This simple Python CLI tool lets you translate back and forth between regular text and the iconic dots and dashes of Morse code. It's a quick, easy way to encode and decode secret messages right in your terminal—no fancy setup required!

## What It Can Do

### Text to Morse
Give it any message (letters, numbers, even punctuation!) and it will instantly spit out the corresponding dots and dashes. We use a single `/` to mark spaces between words.

**Example:**
```
Input:  Hello World!
Output: .... . .-.. .-.. --- / .-- --- .-. .-.. -.. .-.-.-
```

### Morse to Text
Paste in your series of dots and dashes, and the translator will turn it back into readable text for you. 

**Remember:** Separate letters with single spaces and words with ` / ` (space-slash-space)!

**Example:**
```
Input:  .-- . .-.. -.-. --- -- . / - --- / -- --- .-. ... .
Output: WELCOME TO MORSE
```

### Easy Menu
Everything is managed through a simple, friendly menu when you run the script. No complicated commands needed!

## Getting Started (It's Quick!)

### Prerequisites
You only need **Python 3** installed on your computer—chances are, you already do!

- Python 3.x (any recent version works)

### How to Chat in Code

1. **Save the file**: Make sure the code is saved as a Python file (e.g., `morse_translator.py`)

2. **Open your terminal** and run the script:
   ```bash
   python morse_translator.py
   ```

3. **Follow the prompts!** The main screen will guide you:
   ```
   ==================================================
   Welcome to Morse Code Translator!
   ==================================================

   What would you like to do?
     1 - Turn text into morse code
     2 - Turn morse code into text
     3 - I'm done, exit

   Your choice: 
   ```

## Let's See It in Action

### Encoding a Message

Type in your message and watch it transform into Morse code!

```
Type something: Hello World!

Here's your morse code:
.... . .-.. .-.. --- / .-- --- .-. .-.. -.. .-.-.-
```

The script automatically converts everything to uppercase and maps out the code. Easy!

### Decoding a Message

Just paste in your Morse sequence and let the magic happen!

```
Paste your morse code below.
(Tip: Use spaces between characters, ' / ' between words)
> .-- . .-.. -.-. --- -- . / - --- / -- --- .-. ... .

Decoded message:
WELCOME TO MORSE
```

**Pro-Tip:** Make sure you use that ` / ` to separate your words for the best results!

## Behind the Scenes

The translation magic happens thanks to two simple lookup tables (dictionaries) built right into the script:

### The Dictionaries

1. **`MORSE_MAP`**: The master list, mapping every character (like `'A'`) to its Morse equivalent (like `'.-'`)
2. **`TEXT_MAP`**: The reverse of the first map, allowing us to quickly look up letters from code

This reverse-dictionary approach is way faster than searching through the list every time!

### The Main Logic

**`convert_to_morse(text)`**
- Takes your text and uppercases it
- Builds the code list character by character
- Substitutes spaces with `/` for word breaks

**`convert_to_text(morse_code)`**
- Splits the code string into words (at the `/` marker)
- Then splits words into individual letters (at single spaces)
- Looks up each code in the TEXT_MAP dictionary
- Reconstructs the original message

**`main()`**
- Keeps the whole show running with the interactive menu
- Handles user input and output
- Makes everything user-friendly!

## Supported Characters

- **Letters**: A-Z (automatically converted to uppercase)
- **Numbers**: 0-9
- **Punctuation**: `,` `.` `?` `/` `-` `(` `)`
- **Spaces**: Converted to `/` in Morse code

## Fun Morse Code Facts

- **SOS** (`... --- ...`) is the most famous distress signal—easy to recognize, hard to misinterpret!
- Morse code was invented in the 1830s and is still used today by amateur radio operators
- You can actually learn to "hear" Morse code with practice!

## Want to Contribute?

This is a learning project, and contributions are welcome! Here are some ideas:

- Add sound output (beeps for dots and dashes)
-  Create a GUI version
-  Add file input/output support
- Support international Morse code variants
-  Add a practice mode to help users learn Morse code

Feel free to fork, improve, and submit a pull request!


**Ready to start sending secret messages?** Download the code and start translating!

If you found this useful, give it a on GitHub!
