# TOPSIS (Technique for Order of Preference by Similarity to Ideal Solution)

## Table of Contents

1. [Description](#description)
2. [Installation](#installation)
3. [Usage](#usage)
4. [Example](#example)

## Description

### Topsis-Aaditya-102117021

*for: Project-1(UCS654) submitted-by: **Aaditya Vardhan** Roll no: **102117021** Group: **3CS-1***

Topsis-Aaditya-102117021 is a Python library for dealing with Multiple Criteria Decision Making(MCDM) problems by using Technique for Order of Preference by Similarity to Ideal Solution(TOPSIS)

## Installation

Use the package manager **pip** to install Topsis-Aaditya-102117021

`pip install Topsis-Aaditya-102117021`

## Usage

Enter csv filename followed by *.csv* extension, then enter the *weights* vector with vector values separated by commas, followed by the *impacts* vector with comma-separated signs *(+,-)*

```bash
python sample.py sample.csv "1,1,1,1,2" "+,+,-,+,+" sample-result.csv
```

## Example

### sample.csv

A csv file showing data for different mobile handsets having varying features

| Model | Storage space (in GB) | Camera (in MP) | Price (in $) | Looks (out of 5) |
|-------|------------------------|-----------------|---------------|------------------|
| M1    | 16                     | 12              | 250           | 5                |
| M2    | 16                     | 8               | 200           | 3                |
| M3    | 32                     | 16              | 300           | 4                |
| M4    | 32                     | 8               | 275           | 4                |
| M5    | 16                     | 16              | 225           | 2                |

weights vector = [1, 1, 1, 1]
impacts vector = [+,+,-,+]

### input:

`python sample.csv "1,1,1,1" "+,+,-,+" sample-result.csv`

### output:

|   Topsis-score   | Rank |
|-------------|------|
| 0.534277    | 3    |
| 0.308368    | 5    |
| 0.691632    | 1    |
| 0.534737    | 2    |
| 0.401046    | 4    |






