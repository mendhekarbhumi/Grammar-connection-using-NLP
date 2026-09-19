grammar_nlp.py

import nltk
from nltk.tokenize import
 word_tokenize
from nltk import pos_tag

nltk.download('punkt')
nltk.download('averaged_perceptron_tagger')

sentence = input("Enter a sentence: ")

words = word_tokenize(sentence)
tags = pos_tag(words)

print("\nWords and their Grammar Tags:")
for word, tag in tags:
    print(word, ":", tag)