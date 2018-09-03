# text-difficulty-analyzer
Corpus-based text difficulty analyzer for language learners based on word dispersion; also a text corpus management framework powered by PyMongo. First described in a master's thesis.

## Prerequisites
1. [An Anaconda Python 3.6 distribution](https://www.anaconda.com/download/)
2. [MongoDB Atlas](https://www.mongodb.com/download-center?jmp=nav)
3. [Pymongo](https://anaconda.org/anaconda/pymongo)
4. Text files in UTF-8, if you want to build a corpus of your own

## Contents
| Date          | Update        |
| ------------- | ------------- |    
| 09/03/2018      | **00. Automatic Wikipedia extractor.ipynb** Extracts random articles from Wikipedia and saves them as text files. Useful if you don't have text files laying around.| 
| 09/03/2018      | **01. Corpus builder.ipynb** Extracts text data as tokens.| 
| 09/03/2018      | **02. Dispersion calculator.ipynb** Adds Gries' (2008, 2010) *deviation of proportions* (DP) to the built corpus.| 
| 09/03/2018      | **03. Calculate Text Difficulty Scale.ipynb** Calculates Text Difficulty Scale (TDS) values for any text file.| 
| 09/03/2018      | **04. Difficulty Highlighter.ipynb** Highlights especially difficult words in a text.| 

## Tutorial
