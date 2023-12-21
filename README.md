## Exploration of Change Over Time Within the Annual Review of Anthropology

This repository contains a corpus of text samples from the articles published in first issue of the Annual Review of Anthropology (1972) and from the most recent issue from 2023.
The text was manually scraped by me from https://www.annualreviews.org/journal/anthro. The text samples from the first issue were taken from the preview page of the article (the first page) using the 'copy text in image' feature because the complete articles from this first volume were behind a paywall. Because this feature is not perfect, I examined the result copied and filtered out footnotes, additional characters, and reordered text according to what was on the page. 
However, the articles published in the 2023 journal were available online, and the text sample comes from copying the first two paragraphs of the introduction section. The length of the texts for each entry is about equal because the preview page typically also displays the first 2-3 paragraphs of the article. I believe that for the scope of this analysis, this amount of text will be enough to generate a general understand of the semantic styles and thematic differences that might appear. 

# Intended use
This repository, dataset, and any subsequent analysis may be of interest to those in the field of anthropology who are interested in seeing the development of the field-- especially in regards to language used.

# txt Files
Each txt file contains the article title on one line and the text sample on the other. They are named according to Volume (vol1 refers to Volume 1 from 1972 and vol52 refers to the Volume 52 from 2023) and the article location. For example, text file vol1.15 would refer to the 15th published article in Volume 1 of the Annual Review of Anthropology. 
# CSV Metadata and Information
The anthroreviews_with_spaCy_tags.csv file contains the following data:
| Variable Name | Description |
| --- | --- |
| title | Title of the review as displayed on the journal |
| author | authors names |
| year | the year the volume was published |
| text_sample | The textual data scraped by me-- either the first two paragraphs of the introduction or a copy of the text scanned from the preview page |
| text_filename | The text file that contains the text sample from the indivual review |
| Doc | The text of each review, but as doc object |
| Tokens | Tokens found using the spaCy analysis in each text sample |
| Lemmas | Lemmas or keywords as defined by the spaCy code |
| POS | List of the parts of speech found in each text|
| Proper_Noun | List of proper nouns found by spaCy in each text |
| Named_Entity | List of types of named entities in each text |
| NE_Words | List of the named entities found |

The anthro_reviews_csv.csv file is the original file that I had used to collect my data and was used as a basis of the spaCy csv. This file contains title, author, year, text_sample, and text_filename. 

