# Division of our notebooks in OERs + Formats

?0. Operationalization of the research question: How to examine media waves
 * Where are we starting from? (newspaper articles in various formats)
 * Where do we want to end up? (wikipedia like plot on the newspaper coverage on the Spanish flu)

## Notebook 1
1. Text as digital object – formats: xml, pdf / jpg, txt: Text / Video 
2. What is OCR?: Text / Video
3. OCR services: Text / Table  
  * What libraries are they?
  * What are we using and why?
4. Application of OCR: Notebook (with Text)
  * What does input data look like?
  * How is it applied?
  * What does the output look like?
5. Post-Correction: Notebook 
  * Manual 
  * (automatic, GPT)
6. Quality of OCR : Text / Video & Notebook 
 * How to compare output?
 * measurements: accuracy, precision, recall, F1
 * result of our OCR pipeline: Notebook
7. XML as format: Text / Video
8. XML text extraction: Notebook
(9. output format: txt): Notebook 

## Notebook 2
11. More to 1.: What do plain texts look like?: Text & Notebook
  * Texts as lists of characters
12. NLP as a method to 'semantizise' texts: Text / Video
  * Was ist NLP
  * Which libraries are available?
  * What tasks can be carried out by the libraries?
13. Methods of NLP: Text & Notebook
  * Tokenization (also: lazy tokenization) 
  * Lemmatization
  * sentence splitting
  * PoS-Tagging
14. Annotated Text format (Text as a table): Text
15. Post-Correction of NLP output?: Text & Excel
  * sentence splitting, lemma, pos?
  * --> refer back OR focus on NOUNS: are all found, are
16. Quality of NLP services?: Notebook
 * How to compare output?
 * measurements: accuracy, precision, recall, F1
10. Metadata (conceptual introduction)?: Text / Video
 * What fields do we need? 
 * What fields are there, what fields should be added?
 * Format 
17. Metadata Extension: Notebook
 * What can we extract at this point?
 * Small comparison of the texts: sentence length,number of token, number of lemma, vocab
 * Writing to file

## Notebook 3
18a. How to get from a table like text to media waves? (conceptual introduction to Operationalization): Video
 * Basis for analysis: Notebook
   * Lemmata
   * Metadata: year, newspaper
18b: Line plot: Text / Video
  * analysing word frequencies over time 
  * analysing groups of words over time (conceptual: group of words as semantic field / topic?)
19a. Analysis 1 – Talking about the flu: Text & Notebook
  * absolute frequency: of one word / group of words
  * relative frequency: "" 
  * discussion of results
20. Analysis 2 – Who is talking about the flu: Notebook
 * relative frequency
 * newspaper specific -> parameterization

(21. How does the flu conincide with other 'topics'?): Notebook
 * create field of words
 * plot against flu field
 * KWIC output 

## Questions
* It is not important how tesseract and spacy do it under the hood – right? only conceptual understanding
