# Benchmark Task

Cleaned data is pos_new.txt and neg_new.txt. It contains 125000 samples each of positive and negative moview reviews.

# How to get the best embeddings we got so far

Run 3 epochs (210000) iterations of EmbeddingModifierNetwork network with hyperparameters:
SYN_ANT_MULT=3 ,HYPER_HYPO_MULT=2 ,POS_MULT= 1,TEST_EPOCHS=210000

These are loss multipliers (please refer the report for more information)

Description of each script:

## get_word_embeddings.py
Script used to generate improved word embeddings

## benchmark_embeddings.py
Script used to check how good newly created word embeddings are

## i2w.dill, w2i.dill, vocab.dill, word2vec_embeds.pt
Serialized vocabulary related files for baseline embeddings. These were created so that we don't have to recreate them for every experiment.

## Serialize Vocabulary.ipynb
Script to load and serialize vocabulary



