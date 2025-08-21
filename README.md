# Programming Assignment 1 – Python Basics

**Author:** SAEZ, Eljenzal Hoper U.  
**Course:** Advanced Computer Programming and Algorithms / ECE2112

---

## 📌 Description
This Jupyter Notebook contains solutions to several beginner-level Python programming problems.  
It demonstrates the use of **functions, string manipulation, list unpacking, and dictionaries** in Python.  

The problems solved include:
1. **Alphabet Soup Problem** – Arrange the letters of a string in alphabetical order.  
2. **Emotify Problem** – Replace specific words in a sentence with their corresponding emoticons.  
3. **List Unpacking** – Extract the first, middle, and last elements of a list using unpacking syntax.  

---

## ⚙️ Requirements
- Python 3.x  
- Jupyter Notebook  
- No external libraries required (uses only Python’s built-in functions)

---

## ▶️ How to Run
1. Install [Jupyter Notebook](https://jupyter.org/install) or use Google Colab.  
2. Open the file **`SAEZ_PA1.ipynb`**.   
3. The outputs will appear directly under each code cell.  

---

## 💡 Examples

# --------------------------------------
# ALPHABET SOUP PROBLEM
# --------------------------------------

# Function that arranges letters of a word in alphabetical order
def alphabet_soup(word):
    result = ''.join(sorted(word))  # sort letters, join them back
    return result

# Examples
print('alphabet_soup("hello") ➞', alphabet_soup("hello"))
print('alphabet_soup("hacker") ➞', alphabet_soup("hacker"))


# --------------------------------------
# EMOTIFY PROBLEM
# --------------------------------------

# Function that replaces specific words with emoticons
def emotify(sentence):
    # Dictionary of words mapped to emoticons
    emoticons = {
        "smile": ":)",
        "grin": ":D",
        "sad": ":(",
        "mad": ">:("
    }
    # Replace each word with its corresponding emoticon
    for word, symbol in emoticons.items():
        sentence = sentence.replace(word, symbol)
    return sentence

# Examples
print('emotify("Make me smile") ➞', emotify("Make me smile"))
print('emotify("I am mad") ➞', emotify("I am mad"))
print('emotify("She has a grin") ➞', emotify("She has a grin"))
print('emotify("He looks sad") ➞', emotify("He looks sad"))


# --------------------------------------
# LIST UNPACKING PROBLEM
# --------------------------------------

# Unpack the list into first, middle, and last
writeyourcodehere = [1, 2, 3, 4, 5, 6]
first, *middle, last = writeyourcodehere

# Print results
print("First:", first)
print("Middle:", middle)
print("Last:", last)

