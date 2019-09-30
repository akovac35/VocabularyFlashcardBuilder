# VocabularyFlashcardBuilder
A small project to build English vocabulary expanding flashcards from interesting literature. Word definitions are fetched from online and custom sources. An initial set of common English words is provided for word filtering, with the possibility to define a custom set of words as an additional exclusion filter. Flashcard format is custom, with an example provided for Memorang.

## Usage instructions
Review the contents of the following folders first:
* **input_text** - contains two files, **directly_included_words.txt** (contains a list of words to be directly included for processing) and **ctmu_words.txt** (contains a list of words from literature, to be included for processing); this file has a custom name which you can change, continue reading,
* **filters** - contains files with words to be excluded from processing,
* **external_definitions** - contains files with word definitions, to be used for supplementing Mathematica sources,
* **results** - contains processing results; a file containing a list of all processed words (**interesting_words.txt**), a file containing definitions for interesting words (**interesting_words_definitions.txt**) and a file containing a list of words whose definitions were not found (**unknown_words.txt**),
**flashcards** - contains generated flashcard files.

Word processing is in part manual and iterative:

1. Prepare a list of all distinct words to be processed from a book or some other literature by editing the files in the **input_text** folder. Words to be directly included for processing should be listed in the **directly_included_words.txt** file. The **ctmu_words.txt** file can be renamed at this point,
2. execute the contents of **interesting_words.nb** (you may want to replace the custom file name **ctmu_words.txt** with your actual file name at this step, the parameter is the first line in the **interesting_words.nb**) and **generate_definitions.nb**,
3. review the contents of the **results** folder, **EXIT** if satisfied with the results,
4. edit the files in the **filters** folder to exclude words which are not interesting to you,
5. edit the files in the **external_definitions** folder to provide word definitions for supplementing Mathematica sources,
6. GOTO #2 to process the words again.

Finally, interesting word definitions are ready to be used for generating a flashcard deck. An example is provided for Memorang, execute the contents of **Memorang.nb** and review the results in the **flashcards** folder.
