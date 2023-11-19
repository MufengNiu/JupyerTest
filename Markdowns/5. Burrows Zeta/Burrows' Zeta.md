# Burrows' Zeta

Burrows’ Zeta is a method for using the frequencies of mid-range words for a classification exercise. We take a Text Set of Class A samples and a Text Set of Class B samples. Which words which are used regularly in Class A and rarely in Class B, and vice-versa? Each sample in the analysis is then given two scores, based on how many of the words in the two lists occur in it.  A mystery sample which has many of the Class A words in its vocabulary and rather few of the Class B words can be assigned to Class A.

An example of how you might use Burrows’ Zeta is…

## Platform Process

1.	From the home page, select **Burrows’ Zeta**.
2.	Select **Text Sets** to **Add for Experiment**.
3.	Click **Edit** next to a Text Set to change its analysis criteria. Apply the following settings as required:
***
**Segmentation Options**

- **Segment by Tag** – This option is usually for Text Sets that include XML files that have been segmented as markup. ‘Tag’ refers to markup tags in XML that delineate a section of the text, e.g. ‘Act’. Type tags into this field to separate the Text Set into blocks divided by those tags.
- **Block Method** – Defines the method for creating blocks:
  - **BlockBigLast** – Assign any words left over from creating blocks to the last block, creating one large end block.
  - **BlockSmallLast** – Assign any words left over from creating blocks to their own block, creating one small end block.
  - **OverlappingBigLast** – Create blocks that overlap with each other. Any words that are left over from creating blocks are assigned to the last block, creating one large end block.
  - **OverlappingSmallLast** – Create blocks that overlap with each other. Any words that are left over from creating blocks are assigned to their own block, creating one small end block.
  - **Text** – Use the entirety of the Texts in the Text Set as single blocks.
- **Block Size** – Set the number of words to include in a block.
- **Advancement Size** – For overlapping blocks, denote the starting point of the next block, i.e. an advancement size of 100 would mean that each block starts 100 words after the start of the previous block.

**Word Selection Criteria** – Fill in the fields to define how words are selected in the Text Set.

**Test Segments**

- **Extract random test segments from this text set** – Check this box and set a **Test segment proportion** to extract random segments to test and compare to the score for the whole Text Set.
- **Zeta Index Calculation**
***
4.	Apply the following settings as required:
***
### General

**Zeta Parameters**

- **Output Size** – Set the number of Zeta Words that you want to include in the results.
- **Minimum Zeta score to output** – Set…
- **Random seed for test segment extraction**
- **Words** – Type words into this field to specify words to include or hide in the results, depending on the dropdown above.

**NGrams**

- **Number of NGrams** – Define the value of N for the NGram you want to analyse.

> **What is an NGram?** An NGram refers to a number of words in a sequence. An NGram of 1 can be called a 1Gram, and refers to a single word. A 5Gram is a sequence of 5 words, like “how is it with you” or “get thee to a nunnery”.

### Inclusions/Exclusions

Select XML tags to include or exclude in the results.

**Words to Exclude from Process** – Type words into this field to completely exclude from the Burrows’ Zeta process. By default, we exclude punctuation.

- **Include Homograph Forms** – Check this box to separate homograph forms of a word in the results (e.g. separate the noun and verb forms of “read”).
***
5.	Click **Show Results** to see the results on the right.

## Interpret the Results

Burrows’ Zeta results are split into a few tabs.

- **Zeta Experiment Summary** – This view lists the Zeta Words that have been analysed. Use the dropdown to see the **Hits**, **Frequencies**, and **Proportions** of each Zeta Word in each Text Set, as well as in any random test segments.
- **Text Sets** – Each Text Set has its own result view, where you can see the frequencies of each Zeta Word in each segment/block of the Text Set. If you chose to extract random test segments from a Text Set, that will have its own tab as well.

Click **Copy to Clipboard** to copy the results so you can paste them into a document or spreadsheet.


## API Process 
