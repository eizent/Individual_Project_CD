# Exploration of Change Over Time Within the Annual Review of Anthropology

This repository contains a corpus of text samples from the articles published in first issue of the Annual Review of Anthropology (1972) and from the most recent issue from 2023.
The text was manually scraped by me from https://www.annualreviews.org/journal/anthro. This journal covers significant developments in the field of anthropology and is a peer-reviewed academic journal.
The text samples the first issue were taken from the preview page of the article (the first page) using the 'copy text in image' feature because the complete articles from this first volume were not available without a subscription. Because this feature is not perfect, I examined the result copied and filtered out footnotes, additional characters, and reordered text according to what was on the page. 
The articles published in the 2023 journal were available online as open-access articles, and the text sample comes from copying the first two paragraphs of the introduction section. The length of the texts for each entry is about equal because the preview page typically also displays the first 2-3 paragraphs of the article. I believe that for the scope of this analysis, this amount of text will be enough to generate a general understand of the semantic styles and thematic differences that might appear. 

# Intended use and ethical considerations
This repository, dataset, and any subsequent analysis may be of interest to those in the field of anthropology who are interested in seeing the development of the field-- especially in regards to language used. The Annual Reviews are working towards publishing as open access under the Subscribe to Open model (more information can be found in this link: https://www.annualreviews.org/S2O). The reviews from 2023 that are included in this corpus have been published as open access, but the first volume is not. However, as this project does not intent to distribute save the full texts, it should not be against their copyright rules as stated in the Annual Reviews website. 

# txt Files
Each txt file contains the article title on one line and the text sample on the other. They are named according to Volume (vol1 refers to Volume 1 from 1972 and vol52 refers to the Volume 52 from 2023) and the article location. For example, text file vol1.15 would refer to the 15th published article in Volume 1 of the Annual Review of Anthropology. These text files will not be included in this github to avoid copyright issues by sharing these text samples, but I will include the source of the journals: https://www.annualreviews.org/toc/anthro/1/1 and https://www.annualreviews.org/toc/anthro/52/1., 

# CSV Metadata and Information
The anthroreviews_with_spaCy_tags.csv file contains the following data:
| Variable Name | Description |
| --- | --- |
| title | Title of the review as displayed on the journal |
| author | authors names |
| year | the year the volume was published |
| text_filename | The name of text file that contains the text sample from the indivual review |
| Text | The text sample that was scraped |
| Tokens | Tokens found using the spaCy analysis in each text sample |
| Lemmas | Lemmas or keywords as defined by the spaCy code |
| POS | List of the parts of speech found in each text|
| Proper_Noun | List of proper nouns found by spaCy in each text |
| Named_Entity | List of types of named entities in each text |
| NE_Words | List of the named entities found |

The anthro_reviews_csv.csv file is the original file that I had used to collect my data and was used as a basis of the spaCy csv. This file contains title, author, year, and text_filename. 

