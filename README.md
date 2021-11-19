# Automated-ICD10-Medical-Coding-

A pipeline that takes in a Medical Diagnosis from a Physician as text and suggests possible ICD10
Medical codings by extracting symptoms with NLP and Machine Learning techniques.

This tool is only intended to assist practitioners with medical coding only. 

The project is currently in 2 phases.
1) Extraction of keywords from the text of a diagnosis
(Stanzaandgensimbasedmatching.ipynb)
This notebook uses the stanza library to parse text and extract the "problems" and"anatomy" the diagnosis involves.

Then using the gensim library, a semantic word similarity is performed using gensim library.
The Library takes in the first alphabet as a suggestion and then suggests the most appropriate codes accordingly

2) Prediction of first alphabet for medical code
(Ongoing)
Using deep learning frameworks to design a pipeline to predict the alphabet so accurate codings can be suggested
