### Word Embeddings for the Albanian Language
The data folder contains the downloaded corpus in XML format for the Albanian Wiki. The file is in bz2 format so it needs to be decompressed first.



### Installation

#### Compatibility Matrix


| Technology  | Version | Notes | 
|---------------|-----------|-----------|
| [Python](https://www.python.org/)  | 3.5+  | -  | 
| [Jupyter Notebook](https://jupyter.org/)  | 4.x+  | -  | 
| [TensorFlow](https://www.tensorflow.org/)  | 1.x+  | -  | 

> TODO: Add all the stack and prereqs necessary to get started


### Get started

- Decompress the .bz2 file
```bash
bzip2 -dk sqlwiki-20181220-pages-articles-multistream.xml.bz2 

```
- Clean the xml file by stripping all non-alphas out 
```bash
cd scr && perl -C clean_wikisq.pl ../data/sqlwiki-20181220-pages-articles-multistream.xml

```


## Getting Involved

Are you interested in contributing to the NLP for Albanian Language Project? We, the maintainers and community,
would love your help and contributions! We have a quick-start guide on [adding a feature]().

We encourage every community contributor to act as if they are
maintainers, even if you might not have "official" write permissions. This is a
community effort!

You can reach us in the channels below:  
Slack: https://thinkgradient.slack.com  
Email: -



__Issues__  
Define the issues reporting rules

__Pull Requests__  
Define the PR rules

