# Python String Word Analysis

> Core Python string operations practised through dictionary-building exercises — mapping words to computed properties using loops, slicing, and built-in string methods.

---

## Overview

This project works through 15 structured exercises that each take a list of words as input and produce a dictionary mapping every word to a derived value. The exercises progressively cover character access, string transformations, vowel/consonant counting, sorting, and arithmetic on string properties — all without external libraries.

---

## Repository Structure

```
python-string-word-analysis/
│
├── notebook/
│   └── python_string_word_analysis.ipynb   # Main exercise notebook
└── README.md
```

---

## Analysis Covered

| Q   | Exercise                           | Concept Practised                        |
|-----|------------------------------------|------------------------------------------|
| Q1  | Word length mapping                | `len()`, dict assignment                 |
| Q2  | First letter mapping               | String indexing `word[0]`                |
| Q3  | Last letter mapping                | Negative indexing `word[-1]`             |
| Q4  | Word and reversed word             | Slice reversal `word[::-1]`              |
| Q5  | Word and uppercase                 | `str.upper()`                            |
| Q6  | Word and lowercase                 | `str.lower()`                            |
| Q7  | Word and vowel count               | Loop + membership check (`in`)           |
| Q8  | Word and consonant count           | Loop + negated membership (`not in`)     |
| Q9  | Word and double word               | String repetition `word * 2`             |
| Q10 | Word and first two letters         | Slice `word[0:2]`                        |
| Q11 | Word and last two letters          | Negative slice `word[-2:]`               |
| Q12 | Word and non-vowel character count | Loop + conditional counting              |
| Q13 | Word and middle character          | Index arithmetic `len(word) // 2`        |
| Q14 | Word and sorted letters            | `sorted()` + `str.join()`                |
| Q15 | Word and length squared            | `len()` + exponentiation `** 2`          |

---

## Getting Started

### Prerequisites

- Python 3.8+

### Installation

```bash
# Clone the repository
git clone https://github.com/<your-username>/python-string-word-analysis.git
cd python-string-word-analysis

# Launch Jupyter Notebook
jupyter notebook python_string_word_analysis.ipynb
```

### Running on Google Colab

1. Upload `python_string_word_analysis.ipynb` to [Google Colab](https://colab.research.google.com)
2. Run all cells — no additional dependencies required

---

## Key Concepts Demonstrated

**String Slicing**
```python
word = "apple"
word[0]     # 'a'   — first letter
word[-1]    # 'e'   — last letter
word[0:2]   # 'ap'  — first two letters
word[-2:]   # 'le'  — last two letters
word[::-1]  # 'elppa' — reversed
```

**Vowel and Consonant Counting**
```python
def word_and_vowel_count(words):
    vowel_count_dict = {}
    vowels = "aeiou"

    for word in words:
        vowel_count = sum(1 for char in word if char in vowels)
        vowel_count_dict[word] = vowel_count

    return vowel_count_dict
```

**Sorting Letters**
```python
def word_and_sorted_letters(words):
    sorted_letters_dict = {}

    for word in words:
        sorted_letters_dict[word] = "".join(sorted(word))

    return sorted_letters_dict
```

---

## Technologies Used

![Python](https://img.shields.io/badge/Python-3.8+-3776AB?style=flat&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=flat&logo=jupyter&logoColor=white)
![Google Colab](https://img.shields.io/badge/Google-Colab-F9AB00?style=flat&logo=googlecolab&logoColor=white)

---

*Built by **Radhika Deshpande** · Practicing Core Python Through String & Word Analysis*
