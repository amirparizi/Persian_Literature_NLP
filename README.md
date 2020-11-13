# Persian_Literature_NLP

n persian literature history, Hafiz (https://en.wikipedia.org/wiki/Hafez (14th century) and Ferdowsi (https://en.wikipedia.org/wiki/Ferdowsi) (12 Century) was among the best poem of all time.

The most remarkable work of Ferdowsi called Shahname. (https://en.wikipedia.org/wiki/Shahnameh). the Shahnameh is one of the world's longest epic poems.

A collection of numerous multilayered poems by Hafiz, the Divan consists primarily of sonnet-like verses (ghazals) quatrains (ruba‘is), and a few miscellaneous odes (qasidas) and fragments (qit‘as). Strong mystical themes abound, along with social criticism and philosophical and intellectual insights.

To compare these classical persian literature with a modern poem , I decided to work on my favorite modern poem named Akhavan-Sales (https://en.wikipedia.org/wiki/Mehdi_Akhavan-Sales). He is one of the pioneers of Free Verse (New Style Poetry) in the Persian language.

In section 1, I preprocessed some of Divan from Hafiz (Which is my his favorite work) and trained the RNN system using n-grams to predict poem in Hafiz style. Model (Embedding -> Bidirectional LSTM -> Dense) reach to 90% accuracy and predict rest of seed_test in his style (Sorry for the persian words but if you are not persian, believe me those predictions make sense and look like Hafiz try to write poem when he is a little drunk!)

In section 2, I preprocessed some parts of Shahnameh from Ferdowsi,Divan from Hafiz and collection poet from Akhavan to train my RNN (Embedding -> Dropout -> Conv1d -> MaxPooling -> 2* Bidirectional LSTM -> Dense) network. The goal was to train a network that can predict other works by their other works which model achieved almost 100% accuracy on training set and 95% accuracy on validation set. Also model works well on test samples. You can try your sample but try to use distinctive samples from each poet.
