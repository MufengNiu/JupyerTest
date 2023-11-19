# Word Frequencies

Word Frequencies can measure the frequency of certain words or sets of words (NGrams) within a Text by breaking the text down into blocks.

An example of how you might use Word Frequencies is to analyse the frequencies of the words “has” and “hath” throughout all of Shakespeare’s plays. Go to [Case Studies](https://systemik-solutions.github.io/sia_site/6.%20Case%20Studies/Case%203.html#case-3) to work through this example.

## Platform Process

1.	From the home page, select **Word Frequencies**.
2.	Select a **Text** or **Text Set** to analyse.
3.	Apply the following settings as required:
***
### General

**Segmentation Options**
- **Segment by Character** – This option is usually for Texts that are plays, or are XML files that have been segmented as markup. Check this box to separate the Text into blocks divided by character.
- **Segment by Tag** – This option is usually for Texts that are XML files that have been segmented as markup. ‘Tag’ refers to markup tags in XML that delineate a section of the text, e.g. ‘Act’. Type tags into this field to separate the Text into blocks divided by those tags.
   - **Block Method** – Defines the method for creating blocks:
   - **BlockBigLast** – Assign any words left over from creating blocks to the last block, creating one large end block.
   - **BlockSmallLast** – Assign any words left over from creating blocks to their own block, creating one small end block.
   - **OverlappingBigLast** – Create blocks that overlap with each other. Any words that are left over from creating blocks are assigned to the last block, creating one large end block.
   - **OverlappingSmallLast** – Create blocks that overlap with each other. Any words that are left over from creating blocks are assigned to their own block, creating one small end block.
   - **Text** – Use the entirety of the Text as a single block.
- **Block Size** – Set the number of words to include in a block.
- **Advancement Size** – For overlapping blocks, denote the starting point of the next block, i.e. an advancement size of 100 would mean that each block starts 100 words after the start of the previous block.

**Count Options**
- **Number of NGrams** – Define the value of N for the NGram you want to find the frequency of.

> **What is an NGram?** An NGram refers to a number of words in a sequence. An NGram of 1 can be called a 1Gram, and refers to a single word. A 5Gram is a sequence of 5 words, like “how is it with you” or “get thee to a nunnery”.

- **Emendation** – Emend the words shown in the results. This setting works for Texts that are TEI or Plain Text files that have been marked up with tags for certain words.
   - **reg** – Tag to denote a regularised form of a word
   - **corr** – Tag to denote a corrected form of a word
   - **orig** – Tag to denote an original form of a word
   - **sic** – Tag to denote an original form of a word before correction
- **Count Graphemes** – Check this box to use graphemes/letters as a Gram (i.e. ‘the’ would become a 3Gram).

**Output Options**
- Show Metadata – Check this box to show metadata from the Text or Text Set in the results, e.g., the Title.
- **Show** – Choose which words to show in the results:
  - **Words having highest frequency** – Show the most common words
  - **Words unsorted** – Show words that are entered into the Words field, in the order they are entered.
- **Output Size** – Set the number of common words to show in the results.
- **Words** – Type words into this field to specify words to include or hide in the results, depending on the dropdown above.

### Inclusions/Exclusions

**XML Options** – This option is for Texts that are XML files that have been segmented as markup. Select XML tags to include or exclude in the results.

**Word Options** – Type words into this field to completely exclude from the Word Frequencies process. By default, we exclude punctuation.
   - **Include Homograph Forms** – Check this box to separate homograph forms of a word in the results (e.g. separate the noun and verb forms of “read”).
***
4.	Click **Show Results** to see the results on the right.

## Interpret the Results

Word Frequencies results are split into four tabs.

- **Text Output** – The most general result view. The words or NGrams you searched for are shown in the left column. The Text segments (or blocks) are listed in the top row. The table shows the number of instances of each word or NGram in each block. Toggle **Show proportions** to see the results as percentage values.
- **Shannon Entropy Column** and **Shannon Entropy Table** – These views assign each segment with an Entropy score, which indicates how repetitive the word use is within the segment. A higher score means the word use is less repetitive. The **Shannon Entropy Table** includes an Average score.
- **Segment Endings** – This view helps you find the beginning and end of segments within the Text, so you can apply the results. For each segment, the first four words and the last three words are shown.

Click **Copy to Clipboard** to copy the results so you can paste them into a document or spreadsheet.

## API Process 
