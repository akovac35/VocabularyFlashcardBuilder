# VocabularyFlashcardBuilder
A small project to build English vocabulary expanding flashcards from interesting literature. Word definitions are fetched from online and custom sources. Initial set of common English words is provided for word filtering. It is possible to define a custom set of words as an additional exclusion filter.

## Usage instructions
Review the contents of the following folders first:
* input_text
* filters
* external_definitions
* results

*external_definitions* folder defines the means with which it is possible to manually or automatically generate definitions for words in the *results/unknown_words.txt* file. Use *filters/not_interesting_words.txt* and *external_definitions/\** to iteratively improve the interesting words set by executing *interesting_words.nb* and *generate_definitions.nb* in the same order.

Main processing results are stored in *results/interesting_words.txt* and *results/interesting_words_definitions.txt*.
