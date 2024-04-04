# FakeNewsProject
The fake news project by Noah Wenneberg Junge, Kevin Mark Lock and Marcus Friis-Hansen
04-04-2024

To reproduce the results in this report do the following:

Files needed to start:

- news_sample.csv
- 995Data.csv
- GoogleNews-vectors-negative300.bin (For advanced model) Link: (https://drive.google.com/file/d/0B7XkCwpI5KDYNlNUTTlSS21pQmM/edit?resourcekey=0-wjGZdNAUop6WykTtMip30g)
- train_liar.tsv (we use the train data from liar as it has the largest amount of rows and since we dont train on it we can use it for testing )

Steps:

1. Open the jupyter notebook and run the setting up section. Change the DATA_PATH to your data folder (where you have the two files)
2. Run the entire section "Part 1 - Task 1: Cleaning Functions and testing on News Sample"
3. To see all the plots from data exploration, run "Part 1 - Task 2: Explore the FakeNewsCorpus" 
4. Run the sections : "Part 1 - Task 3: Clean entire data" and "Part 1 - Task 4: Split the data". These are meant to be ran one after another. This will save some files in your folder for later usage.
5. From this point, the document splits into two parts:
  a. File setup
    To train the models, there are some sections, that need to be ran to create the necessary files.
     1. Run the "Make BoW vector" Section. Used for simple models. This is a requirement for making the TFIDF vector
     2. Run the "Make TFIDF Vector" Section. This is used for models 1, 2, 3, 7
     3. Run the "Make Embedding Vector" Section. Used for models 4
     4. Run the "N Embeddings pr document" Section. Used for models 5, 6, 7
  b. Training models
    To train each model. Make sure you ran the section above for that specific model. Then run the section and the model gets trained, testet, and saved.
    Note: Each model section has a validation part and a test-part, that we only used once.
  c. Loading models:
     We have uploaded all our models in the GitHub repository in models.zip. Download them and load them in the "Loading Models" section. Then run any model section except for the training part to test it.
6. For our evaluation, make sure to have completed all the other steps and then run the entire section. Scores will show for model2_simple and model 7
  





