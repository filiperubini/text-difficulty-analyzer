# text-difficulty-analyzer
Corpus-based text difficulty analyzer for language learners based on [*word dispersion*](http://www.linguistics.ucsb.edu/faculty/stgries/research/2008_STG_Dispersion_IJCL.pdf); also a text corpus management framework powered by [Pymongo](https://anaconda.org/conda-forge/pymongo). Calculates text difficulty through a *Text Difficulty Scale* (TDS), with values ranging from 0 (least difficult) to 1 (most difficult).

First proposed in a [master's thesis](http://buscatextual.cnpq.br/buscatextual/visualizacv.do?id=K4479428E6) advised by Prof. [Heliana Ribeiro de Mello](http://www.letras.ufmg.br/profs/helianamello/) ([Poslin](http://www.poslin.letras.ufmg.br/), [UFMG](https://ufmg.br/)).

## Demo (Difficulty Highlighter)

Difficulty highlighting of part of the [English](https://en.wikipedia.org/wiki/Johann_Sebastian_Bach) and [Portuguese](https://pt.wikipedia.org/wiki/Johann_Sebastian_Bach) summaries of the Wikipedia article *Johann Sebastian Bach*, with dispersion values represented in superscript. Download the English version in [.pdf](https://www.dropbox.com/s/gfnfpdvd3njy8e0/bach_en_highlighted.pdf?dl=0), [.html](https://www.dropbox.com/s/eqtv23cni9ydo9w/bach_en_highlighted.html?dl=0), and [.tex](https://www.dropbox.com/s/lik3jfgureka9v7/bach_en_highlighted.tex?dl=0)

![high_tex](https://www.dropbox.com/s/qrkpmftgglfngs2/GIF-Github-LaTeX.gif?raw=1)


## Prerequisites / Tutorial
1. [An Anaconda Python 3.6 distribution](https://www.anaconda.com/download/)
2. [MongoDB Atlas](https://www.mongodb.com/download-center?jmp=nav)
3. Libraries: [tqdm](https://anaconda.org/conda-forge/tqdm), [wikipedia](https://anaconda.org/conda-forge/wikipedia), [Pymongo](https://anaconda.org/conda-forge/pymongo)
4. Text (.txt) files in UTF-8 encoding. If you don't have these, use the Automatic Wikipedia extractor.
5. Execute the MongoDB driver; then execute notebook 01 first and complete the process (may take a few minutes or even hours depending on the size of your data).
6. Calculate TDS (Text Difficulty Scale) values ranging from 0 (very easy) to 1 (very difficult) using the notebook **02. Text Difficulty Analyzer + Difficulty Highlighter.ipynb**. Optionally, you can try the Difficulty Highlighter.

## Contents
| Last Update          | Description        |
| ------------- | ------------- |    
| 09/10/2018      | **00. Automatic Wikipedia extractor.ipynb** -- Extracts random articles from Wikipedia from a language of your choosing and saves them as text files in the ./output_dir folder. Useful for corpus building, if you don't have text files laying around.| 
| 09/10/2018      | **01. Corpus builder.ipynb** -- Extracts text data as tokens and inserts them into a Pymongo database. Good compatibility with languages that use the Latin alphabet. Can work with non-Latin alphabets, but not as well. Adds Gries' (2008) [*deviation of proportions*](http://www.linguistics.ucsb.edu/faculty/stgries/research/2008_STG_Dispersion_IJCL.pdf) (DP), a measure of dispersion that takes into account the size of corpus parts. | 
| 09/10/2018      | **02. Text Difficulty Analyzer + Difficulty Highlighter.ipynb** -- The Difficulty Highlighter can output the analyzer's results in .html and .tex with or without the DP values in superscript.|

## License

This project has an [MIT license](https://opensource.org/licenses/MIT).
