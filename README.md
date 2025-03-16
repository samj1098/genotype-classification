# Genotype Classification Algorithm

## Overview
This project is a Python-based algorithm that classifies genetic test 
samples as "NORM" (normal) or "MUT" (mutant) based on multiplexing test 
results. It determines unknown classifications, detects contradictions, 
and identifies cases where classification is not possible.

## Project Structure
- The website version is adapted to work with web-based input.
- The original version is a standalone script that runs in a local 
terminal.

## Features
- Classifies sample IDs as "NORM" or "MUT" based on given test cases.
- Determines unknown "MUT" samples by checking "NORM" test results.
- Detects contradictions and returns "INCONSISTENT".
- Identifies cases where classification is impossible ("NONUNIQUE").

## How to Run the Project
Standalone Version:
1. Install Python if you haven't already.
2. Run the script:
   python genotype-classification_original_version.py
3. Enter test cases as prompted.

Web Version:
Install dependencies (if required):
pip install flask

Run the web app:
python genotype-classification_website_version.py
Open http://localhost:5000 in a browser.

Example Input & Output
Input:
3
NORM,100,110
MUT,110,12
NORM,200,300

Output (Table View):
Sample ID	Genotype
12	MUT
100	NORM
110	NORM
200	NORM
300	NORM
