Assign 1:
1. Tokenize
(a) Write the name of the corpus to stdout.
(b) Delimit the sentences for each document in the corpus.
(c) Tokenize the words in each sentence of each document.
(d) Count the number of total words in the corpus and write the result to stdout.

2. Part-of-Speech
(a) Apply the default part-of-speech tagger to each tokenized sentence.
(b) Write a file named CORPUS NAME-pos.txt that has each part-of-speech tagged sentence on a separate line and a blank newline separating documents. Where CORPUS NAME is either fables or blogs. The format of the tagging should be a word-tag pair with a / in between. For example: The/DT boy/NN jumped/VBD ./.

3. Frequency
(a) Write the vocabulary size of corpus to stdout. Please note that you should use the lowercased
word.
(b) Write the most frequent part-of-speech tag and its frequency to the stdout.
(c) Find the frequency of each unique word (after lowercasing) using the FreqDist module and write the list in decreasing order to a file named CORPUS NAME-word-freq.txt.
(d) Find the frequency of each word given its part-of-speech tag. Use a conditional frequency dis- tribution for this (CondFreqDist) where the first item in the pair is the part-of-speech and the second item is the lowercased word. Note, the part-of-speech tagger requires upper- case words and returns the word/tag pair in the inverse order of what we are asking here. Use the tabulate() method of the CondFreqDist class to write the results to a file named CORPUS NAME-pos-word-freq.txt.

4. Similar Words
(a) For the most frequent word in the NN (nouns), VBD (past-tense verbs), JJ (adjectives) and RB (adverbs) part-of-speech tags, find the most similar words using Text.similar(). Write the output to stdout (this will happen by default).
