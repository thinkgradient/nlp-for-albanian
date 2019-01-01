### Word Embeddings for the Albanian Language
The data folder contains the downloaded corpus in XML format for the Albanian Wiki. The file is in bz2 format so it needs to be decompressed first. We will use the WikiCorpus module from the gensim library in order to extract the contents from the bz2 file.
 


### Installation

#### Compatibility Matrix


| Technology  | Version | Notes | 
|---------------|-----------|-----------|
| [Python](https://www.python.org/)  | 3.5+  | -  | 
| [gensim python package](https://radimrehurek.com/gensim/install.html)  | 3.2+  | Refere to the link for install instructions  | 

> TODO: Add all the stack and prereqs necessary to get started


### Get started

- Step 1. Decompress and extract the contents of the downloaded .bz2 file from Wikimedia
```bash
python process_sq_wiki.py sqlwiki-xxx.xml.bz2 wiki.sq.text

```
- Step 2. Traing a Word2Vec model on the Albanian Corpus extracted from Step 1
```bash
python train_word2vec_sq_model.py wiki.sq.text wiki.sq.word2vec.model

```
- Step 3. Load the model and experiment with word similarities in Albanian. 
```python
import gensim

model = gensim.models.Word2Vec.load("wiki.sq.word2vec.model")

model.most_similar("gjuha")

[('gjuhën', 0.7616620063781738), 
('gjermanishtja', 0.7423202991485596), 
('gjuhë', 0.7314091324806213), 
('gjuhët', 0.727870762348175), 
('anglishtja', 0.7259993553161621), 
('gjuhen', 0.714989185333252), 
('shqipja', 0.7140241861343384), 
('frëngjishtja', 0.7039558291435242), 
('dialekti', 0.699836254119873), 
('spanjishtja', 0.6830302476882935)]

```

## Getting Involved

Are you interested in contributing to the NLP for Albanian Language Project? We, the maintainers and community,
would love your help and contributions! We have a quick-start guide on [adding a feature]().

We encourage every community contributor to act as if they are
maintainers, even if you might not have "official" write permissions. This is a
community effort!

###You can reach us in the channels below:  
Slack: https://thinkgradient.slack.com  

Email: projects@thinkgradient.com

###Instructions to join this project: 

Follow the instructions at: https://www.thinkgradient.com/getstarted ("Enroll in an AI Project")

More details about the project: https://www.thinkgradient.com/nlp-for-albanian-language (You must sign up on ThinkGradient.com to view this page - takes a few seconds)



__Issues__  
Define the issues reporting rules

__Pull Requests__  
Define the PR rules

