Kurze Erl�uterung:
Ich habe mich bei dem Preprocessing an der Hands-on Session f�r CNNs orientiert. F�r eine embedding-layer braucht es
eine embedding Matrix als Gewichte. Statt der einzelnen Worte werden dann die Indizes in der embedding-matrix als Input
benutzt.
Ich habe das Word2Vec Modell mit einer Stichprobe aus beiden Datens�tzen trainiert. Dann habe ich f�r jeden Datensatz 3 Dateien erstellt:
in der X_datei_text datei sind die Daten in Textform also [[[Hier, ist, Satz, eins],[Satz, zwei]],[[Dokument 2],[Dokument, 2, Satz, zwei]]...]
in der y_datei sind die ratings als liste [Rating Doc1, Rating Doc2, ...]
in der X_datei sind die Daten als Indizes also [[[7, 13, 2277, 51],[63, 7614]],[[253 2],[253, 2, 4, 1345]]...]

In der embedding matrix steht eine gro�e Matrix, wobei die Spaltenvektoren die Wortvektoren sind und die Spalten nach den Indizes sortiert sind.
