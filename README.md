# text-difficulty-analyzer
Corpus-based text difficulty analyzer for language learners based on word dispersion; also a text corpus management framework powered by PyMongo. First described in a [master's thesis](http://buscatextual.cnpq.br/buscatextual/visualizacv.do?id=K4479428E6).

![high_tex](https://i.imgur.com/aKz0fu3.png)
*Difficulty Highlighter output in LaTeX*

## Prerequisites / Tutorial
1. [An Anaconda Python 3.6 distribution](https://www.anaconda.com/download/)
2. [MongoDB Atlas](https://www.mongodb.com/download-center?jmp=nav)
3. Libraries: [tqdm](https://anaconda.org/conda-forge/tqdm), [wikipedia](https://anaconda.org/conda-forge/wikipedia)
4. Text (.txt) files in UTF-8 encoding. If you already have these, 

## Contents
| Date          | Update        |
| ------------- | ------------- |    
| 09/03/2018      | **00. Automatic Wikipedia extractor.ipynb** Extracts random articles from Wikipedia and saves them as text files in the ./output_dir folder. Useful if you don't have text files laying around.| 
| 09/03/2018      | **01. Corpus builder.ipynb** Extracts text data as tokens and inserts them into a Pymongo database.| 
| 09/03/2018      | **02. Text Difficulty Analyzer + Difficulty Highlighter.ipynb** Adds Gries' (2008, 2010) *deviation of proportions* (DP) to the built corpus.|
