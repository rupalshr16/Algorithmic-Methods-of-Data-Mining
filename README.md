import pypandoc

readme = """# Homework 1 – Algorithmic Methods of Data Mining

This repository contains my work for Homework 1. The assignment is mainly about practising Python and solving programming problems on HackerRank.

## What's included

- `README.md` – information about the homework and the files in this repository.
- `scripts.py` – Python solutions for the exercises.
- `printouts/` – screenshots showing completed exercises.

I also use a Jupyter Notebook instead of `scripts.py`, with a separate cell for each exercise.

## Problem 1: Python practice

For the first problem, I worked through the Python challenges listed in the assignment:

- Introduction
- Data Types
- Strings
- Sets
- Collections
- Date and Time
- Exceptions
- Built-ins
- Python Functionals
- Regex and Parsing
- XML
- Closures and Decorators
- NumPy

The challenges are available through the [HackerRank Python section](https://www.hackerrank.com/domains/python).

## Problem 2: Algorithms

The second problem includes these HackerRank challenges:

1. [Birthday Cake Candles](https://www.hackerrank.com/challenges/birthday-cake-candles)
2. [Kangaroo](https://www.hackerrank.com/challenges/kangaroo)
3. [Strange Advertising](https://www.hackerrank.com/challenges/strange-advertising)
4. [Recursive Digit Sum](https://www.hackerrank.com/challenges/recursive-digit-sum)
5. [Insertion Sort – Part 1](https://www.hackerrank.com/challenges/insertionsort1)
6. [Insertion Sort – Part 2](https://www.hackerrank.com/challenges/insertionsort2)

These problems give practice with basic algorithms, loops, recursion, and sorting.

## Running the code

You need Python 3 installed. Open a terminal in the project folder and run:

```bash
python scripts.py
```

If the file contains separate solutions for different questions, run the relevant solution as needed. NumPy exercises require NumPy to be installed.

## Submission

The assignment asks for a public GitHub repository containing a README, the Python solutions (or a notebook), and screenshots in the `printouts/` folder. Follow the submission instructions in the homework PDF and submit the required HackerRank printout as well.

## Author

**Name:**  Rupal Sharma

**Course:** Algorithmic Methods of Data Mining  
**Assignment:** Homework 
"""

output_path = "/mnt/data/README.md"
pypandoc.convert_text(readme, "md", format="md", outputfile=output_path, extra_args=["--standalone"])
print(f"Created {output_path}")
