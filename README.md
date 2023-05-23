# Masters-Thesis-Authorship-Attributon


Masters Thesis topic: Impact of various Parts of Speech taggers in Authorship  Attribution in multiple languages (English, French, Hindi)

Hindi data scraped from hindisamay website. 
English and French data downloaded from Project Gutenberg.

*Final CSVs used in the models will be uploaded after thesis defense.

**DESCRIPTION of Files:

***Hindi Web Scrapper
> Hindi_website_Data_scraper.ipynb (TO CREATE CORPUS CONTAINING HINDI NOVELS FROM VARIOUS AUTHORS)

***Preprocessing
> Create CSV_from_Novel_Data.ipynb (TO CREATE HINDI CORPUS FROM SCRAPED DATA)
> balanced_dataset.ipynb (TO CREATE A CSV CONTAINING EQUAL NUMBER OF SENTENCES PER AUTHOR)
> 200_chunks_dataset.ipynb (TO CREATE A NEW CSV CONTAINING 200 OR A BIT MORE TOKENS, depending of which the next of end-of-line token if not 200th one, LONG CHUNKS PER AUTHOR FROM THE ABOVE CSV)

**French Authorship Attribution

> French_Baseline 
> French_Baseline+POS(POET_Tagger)
> French_Baseline+POS(TreeTagger)
> French_Baseline+POS(Universal_tagset)

As the names suggest, the first file contains only two baseline features: top 100 most frequent function words, and punctuation features. 
The next three files contain the two baseline features + POS features created by different taggers, namely, NLTK's tagger based on Universal tagset, TreeTagger for French, and POET tagger. 

**English Authorship Attribution

> English_Baseline 
> English_Baseline+POS(TreeTagger)
> English_Baseline+POS(NLTK_PennTreebank)
> English_Baseline+POS(Universal_tagset)

The first file contains only two baseline features: top 100 most frequent function words, and punctuation features. 

The next three files contain the two baseline features + POS features created by different taggers, namely, NLTK's tagger based on Universal tagset, TreeTagger for English, and NLTK's tagger based on PennTreebank tagset.

**Hindi Authorship Attribution

> Hindi_Baseline 
> Hindi_Baseline+POS(Universal_tagset)
> Hindi_Baseline+POS(StandfordNLP)

The first file contains only two baseline features: top 100 most frequent function words, and punctuation features. 

The next three files contain the two baseline features + POS features created by different taggers, namely, NLTK's tagger based on Universal tagset, and StandfordNLP's tagger for Hindi based on Hindi Dependency Treebank (HDTB).




