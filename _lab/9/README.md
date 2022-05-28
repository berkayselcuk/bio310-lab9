---
title:  BIO310 - Introduction to Bioinformatics
author: Ogun Adebali
geometry: margin=2cm
---


# BIO310 - Introduction to Bioinformatics - Lab 9 - Differential Gene Expression Analysis

**Deadline:** You need to submit (push) your task by the end of lab hours.

## What is this lab about?

In this lab you are going to follow the instructor and run the R script called lab9.r by using RStudio. Then you are going to make slight changes and run the code yourself. 
You will need to push certain outputs throughout the lab.


**Write your code in `answer.py` file**

You are expected to commit after you completed each task and after every major or minor change, you feel it is needed to report separately. Please use your commit messages meaningfully by describing your change or addition. 


Task #1 
=======
### 1.1 Write a python3 script that `globally` aligns two sequences and calculates the `alignment score`. 

* Introducing gaps are only allowed to the `shorter sequence`. Your strategy will be the following:
    1. Generate all possible alignments without introducing any gap to the longer sequence (seq 1).
    2. Calculate score for all alignments
    3. Return the best alignment(s)
   
* The only difference of this lab from the material covered in the lecture is the gap extension penalty. You should use the code that we went over in the lecture and modify it to accomodate the gap extension penalty.

* You will use the substitution matrix shown below to calculate the `match` and `mismatch` scores of the alignment.

|     |  A  |   C |  G  |  T  |
| --- | :-: | --: | :-: | :-: |
| A   |  2  |     |     |     |
| C   | -7  |   2 |     |     |
| G   | -5  |  -5 |  2  |     |
| T   | -7  |  -7 | -7  |  2  |

* `Gap opening penalty`, the penalty for opening a gap, is `-8`.
* `Gap extension penalty`, the penalty for extending a gap by one residue, is `-6`.

* You will print the best alignment and its score.



