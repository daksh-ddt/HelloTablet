HelloTablet
===========

*Note to self: finish this document!*

Summary
-------

HelloTablet is an app that answers polar (yes or no) and factoid questions using plain text.

For example, when asked the question "was Barack Obama the first African American president?", HelloTablet should respond with
something like "Yes; I found this: Barack Obama was the first African American to become president of the United States."

HelloTabet is activated by saying the word "tablet". Once activated, HelloTablet transcribes your speech, predicts an
answer, and talks back. HelloTablet uses Android's native speech recognizer and an API that wraps Google Translate for
speech synthesis.


The following projects comprise HelloTablet:

* [HelloTablet-API](https://github.com/gavinmh/helloTablet-api)
* HelloTablet client app for Android
* [Aligner API](https://github.com/gavinmh/aligner-api): *Currently a different version of this is contained within the Entailment API. This service should be separated.*
* [Entailment API](https://github.com/gavinmh/entailment-api)
* [Monotonicity Marker socket server](https://github.com/gavinmh/MonotonicityMarker)
* [Factoid Answering API](https://github.com/gavinmh/Factoid-Question-Answering)

*The repositories for these projects are public; I will be refactoring and documenting these projects better in the coming weeks.*


Dependencies
------------

* [NLTK](http://nltk.org/) for tokenization, POS tagging, interfacing to Wordnet, and for some lexical similarity measures, like Jiang-Conrath
and Lin.
* [Scikit-Learn](http://scikit-learn.org/stable/) for random forest and SVM implementations.
* [NetworkX](http://networkx.github.io/) for coreference and anaphora resolution.
* [Stanford Parser](http://nlp.stanford.edu/software/lex-parser.shtml) for shallow parsing. Currently Stanford Parser is only
used when specific words are matched in a sentence.
* [Stanford Tregex](http://nlp.stanford.edu/software/tregex.shtml) for searching parse trees with regex-like patterns to
determine if specific words are in downward- or non-monotone contexts.
* [Stanford Named Entity Recognizer](http://nlp.stanford.edu/software/CRF-NER.shtml)
* [SENNA](https://github.com/baojie/senna) for semantic role labeling, to determine if sentence pairs contain 
similar predicates, like "beat" and "defeated", and tagging argument types. Note that SENNA repeats several tasks in the
pipeline(tokenization, POS tagging, shallow parsing). It was the fastest way I could implement semantic role labeling,
 and is not a permanent solution.


Installation
------------



