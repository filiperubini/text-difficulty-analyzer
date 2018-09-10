# text-difficulty-analyzer
Corpus-based text difficulty analyzer for language learners based on word dispersion; also a text corpus management framework powered by [Pymongo](https://anaconda.org/conda-forge/pymongo). First described in a [master's thesis](http://buscatextual.cnpq.br/buscatextual/visualizacv.do?id=K4479428E6) advised by Prof. [Heliana Ribeiro de Mello](http://www.letras.ufmg.br/profs/helianamello/) ([Poslin](http://www.poslin.letras.ufmg.br/), [UFMG](https://ufmg.br/)).

## Demo (Difficulty Highlighter)

![high_tex](https://www.dropbox.com/s/yftolqrt7bpfgg0/highlighter_latex_github.png?raw=1)
*Difficulty highlighting of part of the summary of the Wikipedia article [**Johann Sebastian Bach**](https://en.wikipedia.org/wiki/Johann_Sebastian_Bach)*

## Prerequisites / Tutorial
1. [An Anaconda Python 3.6 distribution](https://www.anaconda.com/download/)
2. [MongoDB Atlas](https://www.mongodb.com/download-center?jmp=nav)
3. Libraries: [tqdm](https://anaconda.org/conda-forge/tqdm), [wikipedia](https://anaconda.org/conda-forge/wikipedia)
4. Text (.txt) files in UTF-8 encoding. If you already have these, 

## Contents
| Last Update          | Description        |
| ------------- | ------------- |    
| 09/10/2018      | **00. Automatic Wikipedia extractor.ipynb** -- Extracts random articles from Wikipedia from a language of your choosing and saves them as text files in the ./output_dir folder. Useful for corpus building, if you don't have text files laying around.| 
| 09/10/2018      | **01. Corpus builder.ipynb** -- Extracts text data as tokens and inserts them into a Pymongo database. Adds Gries' (2008, 2010) *deviation of proportions* (DP) to the built corpus. | 
| 09/10/2018      | **02. Text Difficulty Analyzer + Difficulty Highlighter.ipynb** -- The Difficulty Highlighter can output the analyzer's results in .html and .tex with or without the DP values in superscript.|


