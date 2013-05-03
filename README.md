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

* NLTK
* Scikit Learn
* NetworkX
* Stanford Dependency Parser
* Stanford Tregex
* Stanford Named Entity Recognizer
* SENNA


Installation
------------



