---
title: "Cesar Cipher and Sudoku"
date: 2024-08-03T15:34:30-04:00
categories:
  - Projects
layout: single
author_profile: true
---

# A Short Summary of Two Projects

These two projects were among the first I completed after I started learning how to program in 2023. I was drawn to the idea of creating user interfaces, even if they were simple, so I decided to implement both of these projects using PyQt5. Now, almost a year later, I’ve learned a lot since then, so here’s a brief summary of each project and some key takeaways.

## Sudoku Solver

I wanted my program to do more than just solve any Sudoku board, so I added a few features:

- Found and saved “easy,” “medium,” and “hard” boards to .csv files. If the user wants to play around with the program and not have to manually input sudoku boards.
- Allowed the user to play by themselves and check their solution.
- Used NumPy for impressive solving speeds.

### The Program in Pictures

{% include figure image_path="/assets/images/project-imgs/sudoku-incomplete.png" alt="Alt text" caption="The program after selecting one of the pre stored boards" align="center" %}

Most of the functionality of the buttons and use of the program is self-explanatory but I did include a message area, "results", which responds to most of the button actions in case any clarification is necessary.

{% include figure image_path="/assets/images/project-imgs/sudoku-hard-complete.png" alt="Alt text" caption="A solved board" align="center" %}

Here is a completed board, one of the hardest for the current implementation of the underlying algorithm.

{% include figure image_path="/assets/images/project-imgs/sudoku-empty.png" alt="Alt text" caption="" align="center" %}

The user can also input their own boards and check their solution or ask the program to solve it for them. Only numerical inputs are accepted within each number square.

### Learning Points

- This was the first more meaningfully larger codebase I worked on, so I had to break down functionality into specific functions and learned the importance of commenting and documenting my work.
- The experience of managing a project with multiple features gave me insights into how to structure code effectively.

## Caesar Cipher

At the time, I was just starting to study cryptography and wanted to explore how easily linear ciphers can be broken due to emerging patterns. This program analyzes letter frequency in a coded message and makes an educated guess on the message by determining which rotation (shift) fits best.

### The Program in Pictures

{% include figure image_path="/assets/images/project-imgs/cesar-encode.png" alt="Alt text" caption="Encoding a message" align="center" %}

After selecting a key (random or not), the "run"" button encodes the message based on the corresponding cypher shift. 

{% include figure image_path="/assets/images/project-imgs/cesar-decode.png" alt="Alt text" caption="Decoding a message" align="center" %}

The more interesting part of the program, the coded message is analyzed for letter frequency, most inputs larger than a few words are easily decoded! The program is still missing the functionality to make other languages work. 

### Learning Points

- Working on this project helped me understand the basics of frequency analysis and how to implement it in code.
- The project reinforced the importance of testing and refining algorithms to ensure accuracy.
- At the time I was also learning about test driven development, and so, I wrote simple tests for most functions while writing each function.
