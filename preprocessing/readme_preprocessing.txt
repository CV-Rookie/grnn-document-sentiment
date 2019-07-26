Kurze Erl�uterung:
Ich habe mich bei dem Preprocessing an der Hands-on Session f�r CNNs orientiert. F�r eine embedding-layer braucht es
eine embedding Matrix als Gewichte. Statt der einzelnen Worte werden dann die Indizes in der embedding-matrix als Input
benutzt.
In word2vec_model_imdb ist das komplette word2vec model, trainiert mit gensim (Python package). In der embedding_matrix
ist eine Liste mit den Wortvectoren, geordnet nach dem Index im word2vec-model. In jeder Liste sind Listen f�r die S�tze, S�tze sind wiederum Listen
mit den einzelnen Worten als Elemente. In X_train, X_test sind die Worte durch ihren Index ersetzt. F�r Worte die im 
Trainingsdatensatz (imdb-train.text.ss) nicht vorkommen, wurde ein Vector f�r unbekannte Worte als Mittelwert aus den anderen
Vektoren eingesetzt.

 