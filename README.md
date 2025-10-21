# Is Less Really More? Fake News Detection with Limited Information

Paper link: https://kdd.org/exploration_files/p20-Is_Less_Really_More.pdf

# Limited Information 
KeyWords - Extracts keywords

POS     - Extracts adjectives and adverbs

NER     - Extracts Named Entities



# Files

{x}keywords.py => Input dataset as csv, outputs dataset with new column containing {x} keywords.

{x}SLIM.py    => Input dataset generated from {x}keywords.py, prints output of SLIM model on dataset.

shannon.py => Input dataset as csv, outputs dataset with new column containing shannon score of another column

# How to use

Modify n in a {x}keywords.py file to desired percentage and replace pd.read_csv(...) lines. 

```python {x}keywords.py```

Modify n in a {x}SLIM.py to be the same as n in {x}keywords.py.

```python {x}SLIM.py```

Modify Fcsv in shannon.py to desired csv and change column names.

```python shannon.py```

# Notes
Column ["merged_info"] used in some files, this column contained purely article text. Replace with column name containing article text for other datasets.

Requirements.txt lists required packages for running SLIM files. Please refer to the github pages of DOCEMB, MisRoBÆRTa, and CapsNet respectively if using the other models.

## Citation

If you use this work, please cite:

Zhaoyang Cao, John Nguyen, and Reza Zafarani. 2025. Is Less Really More? Fake News Detection with Limited Information. SIGKDD Explor. Newsl. 27, 1 (June 2025), 20–31. https://doi.org/10.1145/3748239.3748243
