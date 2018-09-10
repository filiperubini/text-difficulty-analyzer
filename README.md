# text-difficulty-analyzer
Corpus-based text difficulty analyzer for language learners based on word dispersion; also a text corpus management framework powered by PyMongo. First described in a master's thesis.

## Prerequisites / Tutorial
1. [An Anaconda Python 3.6 distribution](https://www.anaconda.com/download/)
2. [MongoDB Atlas](https://www.mongodb.com/download-center?jmp=nav)
3. Libraries: [tqdm](https://anaconda.org/conda-forge/tqdm), [wikipedia](https://anaconda.org/conda-forge/wikipedia)
4. Text files in UTF-8, if you want to build a corpus of your own

## Contents
| Date          | Update        |
| ------------- | ------------- |    
| 09/03/2018      | **00. Automatic Wikipedia extractor.ipynb** Extracts random articles from Wikipedia and saves them as text files in the ./output_dir folder. Useful if you don't have text files laying around.| 
| 09/03/2018      | **01. Corpus builder.ipynb** Extracts text data as tokens and inserts them into a Pymongo database.| 
| 09/03/2018      | **02. Text Difficulty Analyzer + Difficulty Highlighter.ipynb** Adds Gries' (2008, 2010) *deviation of proportions* (DP) to the built corpus.|

## The Difficulty Highlighter
Based on the token data gathered by Notebook **01**, calculates the Text Difficulty Scale (TDS) value (0 is most dispersed, so least difficult; 1 is least dispersed, do most difficult), and highlights texts according to the tokens' individual DP values.
