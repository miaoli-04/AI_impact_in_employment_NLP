# AI_impact_in_employment_NLP
### Data Overview:
• 199600+ articles from four years, with the majority from 2023
• covering 10 main topics*, with ‘AI’, ‘Data’, ‘news’, ‘new’, ‘market’ as most salient tokens

### Methodology: Pre-processing:
• Truncate the content part of the article, cleaning headers and footers from web scraping; tailored algorithm to extract content from frequent source companies (eg. PR Newswire)
• Tokenize content and title: remove numbers, punctuation, website, and stop words and conduct lemmatization
• Remove extremely long n-grams that might be web scraping remains
• Conduct topic modeling and remove articles closely related (> 85%) to 2 irrelevant topics Sentiment Analysis & NER
• Customize models based on financial news sentiments
• Implement sentence-level sentiment analysis with the best model, and use NER in spacy to identify relevant organizations (ORG) and technology (Work of art, product) mentioned in the sentence.
• Calculate the general sentiment of each article Targeted Dataset
• Filter relevant articles based on tokens of title and sentiment analysis score
• Adopt DistilRoBERTa model to classify the main industry discussed in the article
• Conduct text summarization to extract insight from articles Presenting Insights
• Cite quotes from articles to demonstrate insight statement
• Aggregate tokens in article and data cross years, plotting graphs show tendency and weights
