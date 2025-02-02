# Natural Language Processing Fundamentals

## Sessions

1. Fundamental Concepts
   - [Python examples](https://github.com/satuelisa/NLPF/blob/main/NLPF_01_P.ipynb)
   - [R examples](https://github.com/satuelisa/NLPF/blob/main/NLPF_01_R.ipynb)
2. Topic Detection
   - [R examples](https://github.com/satuelisa/NLPF/blob/main/NLPF_02_R.ipynb)
3. Sentiment Analysis
   - [R examples](https://github.com/satuelisa/NLPF/blob/main/NLPF_03_R.ipynb)
4. Tagging
   - [Python examples](https://github.com/satuelisa/NLPF/blob/main/NLPF_04_P.ipynb)
   - [R examples](https://github.com/satuelisa/NLPF/blob/main/NLPF_04_R.ipynb)
5. Word Networks
   - [Python examples](https://github.com/satuelisa/NLPF/blob/main/NLPF_05_P.ipynb)
6. Correction & Prediction
   - [Python examples](https://github.com/satuelisa/NLPF/blob/main/NLPF_06_P.ipynb)
7. Stemming
   - [Python examples](https://github.com/satuelisa/NLPF/blob/main/NLPF_07_P.ipynb)
8. Vectorization
   - [R examples](https://github.com/satuelisa/NLPF/blob/main/NLPF_08_R.ipynb)
9. Chatbots
   - [Python examples](https://github.com/satuelisa/NLPF/blob/main/NLPF_09_P.ipynb)
10. Speech
    - [Python examples](https://github.com/satuelisa/NLPF/blob/main/NLPF_10_P.ipynb)

## Tools and libraries

For each library that requires installation, the parenthesis indicates the sessions that employ the package.

On macos: first install portaudio. Otherwise an error will occur when installing pyaudio.

```shell
brew install portaudio
```

Install all the python libraries from the requirements file (do this in a new virtual environment)

```shell
pip install -r requirements.txt
```

a. [Python](https://www.python.org/) &mdash; [Create a new Colab in Python](https://colab.research.google.com/notebook#create=true)
* `gutenbergpy` (S01)
* `nltk` (S01)
* `wordcloud` (S01)
* `matplotlib` (S01)
* `numpy` (S01)
* `pandas` (S01)
* `speechrecognition`(S10)
* `pyaudio` (S10)
* `pyttsx3` (S10)
* `scipy` (S10)
* `ffmpeg-python` (S10)

b. [R](https://www.r-project.org/) &mdash; [Create a new Colab in R](https://colab.research.google.com/notebook#create=true&language=r)
* `gutenbergr` (S01)
* `tidytext` (S01)
* `ggplot2` (S01)
* `quanteda` (S01)
* `quanteda.textplot` (S01)
* `tm` (S02)
* `reshape` (S02)
* `reshape2` (S02)
* `topicmodels` (S02)
* `wordcloud` (S02)
* `RColorBrewer` (S02)
* `textdata` (S03)
* `reshape2` (S03)
* `igraph` (S04)
* `stopwords` (S08)
* `plot.matrix` (S08)
* `proxy` (S08)
* `word2vec` (S08)
* `plot3D` (S08)
* `NbClust` (S08)
* `factoextra` (S08)

You can either run things on an online environment like Google Colab
or install both of these open-source tools on your own computer. Note
that some installable packages come pre-installed for the Colab Python
environment (like *pandas* and *numpy*) but need to be installed with
`pip` if you set up your own environment.

## Bibliography

![R](https://learning.oreilly.com/covers/urn:orm:book:9781491981641/200w/) | ![Python](https://learning.oreilly.com/covers/urn:orm:book:9780596803346/200w/)
:------------------:|:------------------:
[Text Mining with R](https://learning.oreilly.com/library/view/text-mining-with/9781491981641/) | [NLP with Python](https://learning.oreilly.com/library/view/natural-language-processing/9780596803346/)

Additionally to the above books available through the library, we use the freely available online versions of the following textbooks:
- [Speech and Language Processing](https://web.stanford.edu/~jurafsky/slp3/) referred to as SLP
- [Supervised Machine Learning for Text Analysis in R](https://smltar.com/) referred to as SMLTAR

## Data sets

- [Project Gutenberg](https://www.gutenberg.org/ebooks/): the raw text of numerous books
- [Open Multilingual Wordnet](http://compling.hss.ntu.edu.sg/omw/): `WordNet` data in other languages

# Assignments

The contents of each assignment is detailed on myCourses and also as a single file on [Overleaf](https://www.overleaf.com/read/dgwcbnnzjjbz) for easier access so you can prepare your responses offline.

# Concepts

## Session 1: Fundamental Concepts
- *token* = a meaningful unit (of text)
- *tokenization* = the process of extracting tokens from text
- *string* = a data representation for a sequence of characters
- *metadata* = tags or other type of data associated to a string or a token describing its origin, meaning, or some other characteristic thereof
- *corpus* = a collection of textual data that contains strings, possibly with associated metadata
- *stopword* = a word the presence of which is deemed meaningless in a given context
- *term-document matrix* = a matrix in which each row represents a document and each column represents a term, with the cells indicating the frequency of occurrence of each term in each document

## Session 2: Topic Detection
- *tf-idf* = term-frequency versus inverse-document-frequency matrix that assigns higher weight for terms that are not frequent across *all* of the documents; the *idf* is the natural logarithm of the fraction of total number of documents divided by the number of documents that contain a term
- LDA = Latent Dirichlet Allocation, a topic-modeling algorithm: represent a **document** as a mixture of *topics* and a *topic* as a mixture of **words**

## Session 3: Sentiment Analysis
- *lexicon* = a set of words, a vocabulary
- *unigram* = a unit of language that is a single word

## Session 4: Tagging
- *part of speech* (POS) = *lexical category* = *word class* = the "grammar classes" of words such as nouns, adverbs, verbs, adjectives, etc.
- *bigram* = a two-word sequence
- *n-gram* = a sequence of *n* words

## Session 5: Word Networks
- `WordNet` = a graph-format thesaurus of relationships between English words
- *hyponym* = a more **specific** synonym of a word
- *hypernum* = a more **general** synonym of a word
- *meronym* = component of a concept
- *holonym* = container of a concept
- *antonym* = the counterpart of a word (the contrary version: vertical/horizontal, positive/negative)

## Session 6: Correction & Prediction
- *edit distance* = the total cost of alterations that need to be made on a string to convert it into another one

## Session 7: Stemming
- *stemming* = removal of affixes (suffixes, mostly; sometimes prefixes) to cut down all variants of a word to their "common core"
- *normalization* = a process of regularizing text in some way, such as making all of it lowercase
- *lemmatization* = taking each (conjugated, plural, capitalized, ...) word into the form in which it would appear in a dictionary

## Session 8: Vectorization
- *cosine similarity* = the dot product of two numerical vectors divided by the product of their norms
- *PMI* = pointwise mutual information, a measure to quantify how often do two words appear together than what one would expect if they were ordered at random
- *lemma* = the "dictionary form" of a word
- *wordform* = the specific variant of a word, such as the conjugated form, that may not be a lemma as such
- *polysemous* = having more than one meaning
- *(word) embedding* = a vectorization of a text that attempts to capture semantics based on word context, such as `word2vec`
- *skipgram window* = a token subsequence of a determined length
- *skipgram probability* = the probability (relative frequency) of two tokens appearing together in a skipgram window

## Session 9: Chatbots
- *reflection* = a word pair in which one serves as a response to the other in the sense that if the point of view of the speaker is reversed, the substitution maintains consistency ("this is my dog", "your dog is cute")
- *rule-based chatbot* = one that picks a response to an incoming message based on a set of rules, often expressed in terms of regular expressions
- *self-learning chatbot* = one that uses machine learning to determine responses
- *bag of words* = representing a part of text (sentence, document, etc.) as the set of words it contains (or a binary representation thereof)

## Session 10: Speech
- *text to speech* = have the computer read out loud a text given as input
- *speech to text* = have the computer create a string from a recording (live or file) of spoken language


## Other NLP Courses at McGIll

- [COMP 345/LING 345](https://docs.google.com/document/d/1PnWEGzfTYB_MB_g35tHWGvozAeME7puURoOT3JVj53c/edit)
- [COMP 445/LING 445](https://www.cs.mcgill.ca/media/academic/courses/118_COMP_445.pdf)
- [COMP 550](https://www.cs.mcgill.ca/~jcheung/teaching/fall-2017/comp550/#lectures)
- [COMP 599/LING 484](https://mcgill-nlp.github.io/teaching/comp599-ling782-484-f22/)
- [Quantitative analysis](http://people.linguistics.mcgill.ca/~morgan/qmld-book/)
