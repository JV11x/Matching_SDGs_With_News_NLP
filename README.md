# Using Similarity Scoring Techniques to Match Sustainability Topics with News Articles.

Link to Jupyter Notebook in Google Colab: https://colab.research.google.com/drive/1l16stfwbDaX0Ptupb1A-n2RAPdUSfSew?usp=sharing
The full report can be found here: https://drive.google.com/file/d/1hf9RqRUNuUGoqvj3U3iavv8bu_gbQGa9/view?usp=sharing 

This research investigates developing an automated tool to monitor global progress of the United Nations' 17 Sustainable Development Goals (SDGs). The research considers how tracking global news streams, could help in identifying areas of sustainability that are receiving attention, as well as early warning signs of potential issues. The paper evaluates the performance of contemporary semantic modelling approaches at identifying similarities between news articles and SDG topics.

The research will involve three datasets, including two from Hugging Face and the UN's Sustainability Goals. The first dataset, comprising BBC news articles categorized by topics, will test each model's accuracy in associating articles with correct topics. The second dataset, containing articles from CNN and the Daily Mail, will be used for a final evaluation of the models' abilities to link news articles with the SDGs. The study aims to benchmark various semantic representation techniques and develop a system for effectively monitoring SDG-related developments.

The approaches considered in this research are Word2Vec, SentBERT, Doc2Vec, and DistilBERT (Sent2Vec). The common theme between all these techniques is that they produce a vector representation of text. Cosine similarity can be used to measure the similarity between the vector representations and produce similarity scores. 

### Research hypothesis
Given the task of text similarity matching, this paper aims to demonstrate that transformer models focused on text sequences of at least a sentence in length will outperform our baseline of a word2vec implementation.

## Main experiments
- Using a sample of the CNN Daily Mail dataset and the UN SDGs, develop an average similarity score for each SDG topic across all the articles in the dataset, before manually assessing the outputs for accuracy and errors.
- Hand label a subset of the CNN Daily Mail dataset with their most related SDG topic areas, before testing whether each embedding technique can classify the article with its correct SDG topic label.
