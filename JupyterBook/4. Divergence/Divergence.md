# Divergence

Jensen-Shannon Divergence (JSD, or simply Divergence) is a measure of the similarity or difference between two Text Sets. It is based on proportional frequencies of words. It provides a single measure of difference between samples relying on multiple component word frequencies. A typical application is to compare all the words in a collection to the overall average of that collection. Which words are typical, and which words are aberrant?

By looking at the individual word-variables which contribute most to the Divergence score you can quickly determine whether a handful of words have largely created the divergence, or not, and look at what these words are – typically a very common word with a very high or very low proportional frequency, or a usually rare word used intensively in one of the Text Sets.

An example of how you might use Divergence is to find how the words used in each act diverge between Hamlet and Othello. Does Shakespeare commonly use similar words in certain acts?

## Platform Process

1.	From the home page, select **Divergence**.
2.	Select a **Reference Text Set** as the base Text Set and a **Comparison Text Set** to compare with it.
3.	Apply the following settings as required:
***
### General

**XML Options** – This option is for Text Sets that include XML files that have been segmented as markup. Select XML tags to include or exclude in the results.

**Segmentation Options**

- **Segment by Character** – This option is usually for Text Sets that include plays, or XML files that have been segmented as markup. Check this box to separate the Text Sets into blocks divided by character.
- **Block Size** – Set the number of words to include in a block.

**Count Options**

- **Number of NGrams** – Define the value of N for the NGram you want to analyse.

> **What is an NGram?** An NGram refers to a number of words in a sequence. An NGram of 1 can be called a 1Gram, and refers to a single word. A 5Gram is a sequence of 5 words, like “how is it with you” or “get thee to a nunnery”.

- **Count Graphemes** – We strongly recommend that you uncheck this box. If you leave it checked, Divergence will use graphemes/letters as a Gram (i.e. ‘the’ will become a 3Gram).

**Word Options** – Type words into this field to completely exclude from the Divergence process. By default, we exclude punctuation.

- **Include Homograph Forms** – Check this box to separate homograph forms of a word in the results (e.g. separate the noun and verb forms of “read”).

**Divergence Options**

- **Log Base**
- **Per Word Calculation** – Check this box to see which words contributed most to the Divergence score in the results.
- **Log N/M Calculation**
- **Log N/M Mode**

**Output Options**

- **Show Metadata** – Check this box to show metadata from the Text Sets in the results, e.g., the Titles of Texts.

### Filter

**Words** – Type words into this field to specify words to include or hide in the results, depending on the dropdown above.

**Use most frequent words** – Check this box to only use the most frequent words to determine Divergence. Specify the number of words in the Size field.
***
5.	Click **Show Results** to see the results on the right.

## Interpret the Results

Divergence results are split into many tabs.

- **Divergence Table** and **Divergence Column** – These views show the Divergence scores for segments/blocks of the Comparison Text Set. A higher score means the segment diverges less from the Reference Text Set.
- **Reference Entropy Table**, **Reference Entropy Column**, **Reference Weighted Entropy Table** and **Reference Weighted Entropy Column** – These views assign each segment of the Reference Text Set with an Entropy score, which indicates how repetitive the word use is within the segment. A higher score means the word use is less repetitive. The **Reference Entropy Table** includes an Average score.
- **Comparison Entropy Table**, **Comparison Entropy Column**, **Comparison Weighted Entropy Table** and **Comparison Weighted Entropy Column** – These views assign each segment of the Comparison Text Set with an Entropy score, which indicates how repetitive the word use is within the segment. A higher score means the word use is less repetitive. The **Comparison Entropy Table** includes an Average score.

Click **Copy to Clipboard** to copy the results so you can paste them into a document or spreadsheet.

## API Process 
