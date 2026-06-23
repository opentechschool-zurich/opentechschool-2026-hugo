+++
date = '2026-06-16T22:21:49+02:00'
draft = false
title = 'June 16th 2026: Starting with Python and C++ & Advent of Code 2020'
+++

Today, we introduced two new participants to C++ and Python.

For C++ he settled with the [C++ Primer](https://en.wikipedia.org/wiki/Stanley_B._Lippman)

And for Python she went for a [Youtube tutorial](https://www.youtube.com/watch?v=SR5NYCdzKkc) teaching FastAPI and React!

For tonight exercise we picked day 1 of the [Advent of Code 2020](https://adventofcode.com/2020/day/1). Here is a sample solution in Python:

```py
import itertools

numbers = []

with open("data.txt") as file:
    for line in file:
        numbers.append(int(line.rstrip()))

print(numbers)

def find_2020(numbers):
    for i, a in enumerate(numbers):
        for j, b in enumerate(numbers):
            if i == j:
                continue
            if a + b == 2020:
                return a * b
            
def find2_2020(numbers):
    for a, b in itertools.combinations(numbers, 2):
        if a + b == 2020:
            return a * b

print(find2_2020(numbers))
```
