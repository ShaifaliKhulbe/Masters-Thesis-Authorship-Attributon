# Masters Thesis: Authorship Attribution

**Thesis Topic:** Impact of Various Parts of Speech Taggers in Authorship Attribution in Multiple Languages (English, French, Hindi)

## Data Sources

- **Hindi Data**: Scraped from hindisamay website.
- **English and French Data**: Downloaded from Project Gutenberg.

*Note: Final CSVs used in the models will be uploaded after thesis defense.*

## Machine Learning Models

The project employs SVM machine learning technique on various models as well as natural language processing (NLP) techniques to accomplish authorship attribution. These models include but are not limited to:

- **Baseline Models**: Utilizing fundamental linguistic features, such as the top 100 most frequent function words and punctuation features.
- **POS Tagging**: Incorporating POS features from different taggers for enhanced analysis.


## Description of Files

### Hindi Web Scraper
- `Hindi_website_Data_scraper.ipynb`: Creates a corpus containing Hindi novels from various authors.

### Preprocessing
- `Create CSV_from_Novel_Data.ipynb`: Creates a Hindi corpus from the scraped data.
- `balanced_dataset.ipynb`: Creates a CSV containing an equal number of sentences per author.
- `200_chunks_dataset.ipynb`: Creates a new CSV containing 200 or more tokens, depending on the end-of-line token if not the 200th one, with long chunks per author from the above CSV.

## French Authorship Attribution

- `French_Baseline`: Contains baseline features, including the top 100 most frequent function words and punctuation features.
- `French_Baseline+POS(POET_Tagger)`: Combines baseline features with POS features from the POET tagger.
- `French_Baseline+POS(TreeTagger)`: Combines baseline features with POS features from the TreeTagger.
- `French_Baseline+POS(Universal_tagset)`: Combines baseline features with POS features from NLTK's tagger based on the Universal tagset.

## English Authorship Attribution

- `English_Baseline`: Contains baseline features, including the top 100 most frequent function words and punctuation features.
- `English_Baseline+POS(TreeTagger)`: Combines baseline features with POS features from TreeTagger.
- `English_Baseline+POS(NLTK_PennTreebank)`: Combines baseline features with POS features from NLTK's tagger based on the PennTreebank tagset.
- `English_Baseline+POS(Universal_tagset)`: Combines baseline features with POS features from NLTK's tagger based on the Universal tagset.

## Hindi Authorship Attribution

- `Hindi_Baseline`: Contains baseline features, including the top 100 most frequent function words and punctuation features.
- `Hindi_Baseline+POS(Universal_tagset)`: Combines baseline features with POS features from NLTK's tagger based on the Universal tagset.
- `Hindi_Baseline+POS(StanfordNLP)`: Combines baseline features with POS features from StandfordNLP's tagger for Hindi based on Hindi Dependency Treebank (HDTB).

## Conclusion

This project represents a significant effort in exploring authorship attribution and the role of POS taggers in multiple languages. The use of diverse linguistic features and machine learning models offers valuable insights into this field of study.
