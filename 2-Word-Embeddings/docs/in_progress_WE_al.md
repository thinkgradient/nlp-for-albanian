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