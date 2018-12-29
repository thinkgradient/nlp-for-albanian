Word Embeddings for the Albanian Language
=========================================

The data folder contains the downloaded corpus in XML format for the Albanian Wiki. The file is in bz2 format so it needs to be decompressed first.

To get started:

- Decompress the .bz2 file
-- bzip2 -dk sqlwiki-20181220-pages-articles-multistream.xml.bz2 
- Clean the xml file by stripping all non-alphas out 
-- cd scr && perl -C clean_wikisq.pl ../data/sqlwiki-20181220-pages-articles-multistream.xml

