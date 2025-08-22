# Programming Assignment 1 – Python Essentials

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
1. Install [Jupyter Notebook](https://jupyter.org/install).
2. Open the file **`SAEZ_PA1.ipynb`**.   
3. The outputs will appear directly under each code cell.  

---

## 💡 Examples

### 01 🔠 Alphabet Soup Problem  

```python
def alphabet_soup(word):  # define the function
    return "".join(sorted(word))  # sort characters and join them back
```

- **Creates a function** named `alphabet_soup` that takes one parameter, a string `word`.  
- `sorted(word)` → breaks the string into characters and arranges them alphabetically.  
- `"".join(sorted(word))` → joins the sorted characters back into a single string.  
- Output:  
```python
alphabet_soup("python")  # output: 'hnopty'
```

---

### 02 😀 Emoticon Problem  

```python
def emotify(sentence):  # define the function
    
    emoticons = {  # dictionary to map words into emoticons
        'smile': ':)',
        'grin': ':D',
        'sad': ':(((',
        'mad': '>:(('
    }
    
    for word, emoticon in emoticons.items():  # loop through dictionary
        sentence = sentence.replace(word, emoticon)  # replace matching words
    
    return sentence  # return modified sentence
```

- A function named `emotify` that takes one string `sentence`.  
- `emoticons` dictionary maps words (`smile`, `grin`, `sad`, `mad`) to symbols (`:)`, `:D`, `:(((`, `>:((`).  
- Loops through the dictionary:  
  - `sentence.replace(word, emoticon)` replaces the word with its emoticon.  
- Returns the updated sentence.  
- Output:  
```python
emotify("I am sad but I grin")  # output: 'I am :((( but I :D'
```

---

### 03 📤 Unpacking List Problem  

```python
writeyourcodehere = [1, 2, 3, 4, 5, 6]  # sample list

first, *middle, last = writeyourcodehere  # unpack list

print("first:", first)
print("middle:", middle)
print("last:", last)
```

- Creates a list `[1, 2, 3, 4, 5, 6]`.  
- `first, *middle, last = list` → unpacks values:  
  - `first` → first element (`1`)  
  - `middle` → all elements in between (`[2, 3, 4, 5]`)  
  - `last` → last element (`6`)  
- Prints the unpacked values.  
- Output:  
```
first: 1  
middle: [2, 3, 4, 5]  
last: 6
```

---
