# 🔐 Password Generator (Python)

This project is a **terminal-based password generator** that allows users to choose the length of the password and select character-type combinations. It automatically copies the generated password to the clipboard using `pyperclip`.

## ✨ Features
- Choose password length  
- Select from **Uppercase**, **Lowercase**, **Numbers**, **Symbols**  
- 15 possible character-type combinations  
- Randomized and secure password generation  
- Automatically copies generated password to clipboard  
- Colored terminal output for better readability  

## 📦 Requirements
- Python 3.x  
- `pyperclip` library  

Install missing dependency:
`pip install pyperclip`

## ▶️ How to Run
Save the script as password_generator.py, then run:
`python password_generator.py`

You will be asked to enter:
1. Password length
2. Character-type combination (1–15)

After selecting, the program prints a secure password and copies it to your clipboard.

## 🧠 How It Works

- Uses itertools to generate all character-type combinations
- Prompts user to choose one combination
- Splits password length evenly across selected character groups
- Fills extra characters from a full pool
- Randomizes the final output before displaying
- Copies the final password using pyperclip

## 📁 Project Structure
``password_generator.py   # Main program
README.md               # Documentation``

## 📝 Example Output
```bash
Starting Password Generator...

    Length of Password: 12

Select Character type number from the list:
     1  ---  ('Numbers',)
     2  ---  ('Uppercases',)
     ...
     15 ---  ('Numbers', 'Uppercases', 'Lowercases', 'Symbols')

Type any serial number from the above list of combinations: 15

Your password: Q9m$2g_Ab1!d
Your password is copied to your clipboard.
