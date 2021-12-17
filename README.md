# Project proposal
Study on gender bias centered around the theme of the articles and occupation of the speakers

## Abstract

Our project aims to perform a thematic analysis of the quotes featured in newspapers with a focus on the speaker’s gender and occupation. First, the idea is to study the male to female ratio within speakers quoted for a certain news topic. We are curious to see in which fields there are more men or women who expressed themselves, which gender is more quoted and, in some sort, has a larger voice in the media. Then, we can investigate how related the speaker is to the topic they were quoted in.

## Research Questions

We would like to know if there is a gender bias in the number of quotes and the length of quotes, how this possible bias evolves along the years, and how related it is to the occupation of the speaker. We also want to understand how related each speaker’s occupation is compared to the theme of the original article, and if certain themes/topics also present a gender bias.

## Additional Dataset

For the external source, we use the provided additional metadata about speakers, since their gender and occupations are the subject of our study. The dataset contains 9055981 entries and it gives us different information such as date of birth, ethnicity and religion of the speaker. The aliases show different names associated with the same person. We only keep the columns containing the gender, occupations and Qid using which we merge this dataset with the original ones. We dropped speakers without an occupation, there are ​​4893542 entries remaining.

Additionnally, we used a [pre-trained GloVe word vectors dataset](https://nlp.stanford.edu/projects/glove/) (specifically the glove.6b.zip) for classification of the occupations of each speakers. This dataset is available under the public Domain, and was made by the standford university using GloVe on Wipipedia 2014 and Gigaword 5. We used the dataset as-is, by comparing the distances of words in different categories for classification.

## Methods

In this section we list the methods that we plan to employ in the future to reach our goals. The methods we used to perform the initial analysis and data cleaning are displayed and explained in the notebook.

With the number of occurrences of each quote (the number of articles the quote is featured in), in addition to the gender and occupation of each speaker, we can plot various statistics in order to find correlations and potential answers to our research questions.

Meanwhile, we can analyse the themes of the quote’s associated article(s) by following the corresponding links, as we started in the notebook. Realistically not all website urls can be parsed to extract topics, but we aim to select the ones with the most quotes in the dataset, and to have some variety in the choice of websites, as they have different areas of expertise and focus. After that, we have to make the different thematic categories consistent across the chosen websites (e.g. “celebs” in one website’s theme might be “celebrities” in another). 

Finally we can do a thematic analysis of the quotes, focusing again on gender and occupation.

## Proposed timeline

- Perform the statistical analysis on the speaker’s gender and occupation

- Extract themes from as many sites as we deem feasible

- Clean up those themes to be consistent across the sites, i.e. aggregate synonyms

- Perform the statistical analysis on the articles’ theme, with a focus on the speaker’s gender and occupation.

- Present our findings in a “data story”

## Organization within the team

Matthieu: Perform the first statistical analysis on gender and occupation 

Danaé: decide on the websites to use for topic extraction and extract themes for the quotations.

Yingxuan: Group similar themes together across the sites and analyse the themes with respect to gender and occupation

All of the team: Help write the data story with the conclusions we found.

