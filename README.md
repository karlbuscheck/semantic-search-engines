# Building and Testing Semantic Search Engines

I love executing the final cell in a Jupyter Notebook and getting hit with a mic drop moment.

That's exactly what happened at the end of this notebook while building a couple of semantic search engines that used embeddings to grasp the context and nuance of language. One engine relied on pretrained embeddings `(word2vec-google-news-300)`, while the other was fully customized, trained from scratch on my own dataset.

Intuitively, I thought I knew which one would win.

But the results told a different story.

Along the way, I dug into embeddings -- how they work, how they're built, and how they power all sorts of AI tools, like ChatGPT, by turning language into numbers. Below is a roadmap of what this notebook covers.

_Note: This repo includes a small sample (`fake_news_sample.csv`) for demo purposes as the full dataset is roughly 111MB._

## The Roadmap
- Loading and using pretrained embeddings
- A quick word on embeddings
- Preparing the corpus for semantic search
- Creating a TF-IDF search engine for baseline comparison
- Building a semantic search engine with pretrained embeddings
- Creating the document-features matrix
- Engineering the semantic search function
- Building a semantic search engine with custom-trained embeddings
- Creating (another) document-features matrix
- Re-engineering the semantic search function
- Comparing the search engines and crowning an unexpected winner

## Tools & Libraries Used
- **Jupyter Notebook** — for interactive coding and exploration  
- **Python 3.12.2**
- **pandas** — for data manipulation  
- **nltk** — for text preprocessing and lemmatization  
- **gensim** — Word2VEc training and vector lookups
- **scikit-learn** — for modeling and cosine similarity

## Acknowledgements

This all started with a notebook I was working on for my NLP class, taught by  Associate Professor Michele Samorani at Santa Clara University. Big thanks to him and the Leavey School of Business for helping spark the idea
