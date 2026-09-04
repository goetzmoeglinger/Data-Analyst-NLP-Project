# Data Analyst NLP Project

NLP-Analyse von Verbraucherbeschwerden im Rahmen des Moduls Data Analyst.

## Datengrundlage

Als Datengrundlage dient der Consumer Complaint Dataset des Consumer Financial Protection Bureau (CFPB). Für die Analyse wurde eine zufällige Stichprobe von 20.000 Verbraucherbeschwerden verwendet. Analysiert wurden die frei formulierten Beschwerdetexte.

## Verwendete Verfahren

- Bag-of-Words (BoW)
- TF-IDF
- Latent Dirichlet Allocation (LDA)
- Latent Semantic Analysis (LSA)
- Topic Coherence zur Bestimmung der Anzahl der LDA-Topics
- ergänzende Untersuchung der Lemmatisierung

## Technische Umsetzung

Die Analyse wurde in Python in einem Jupyter Notebook durchgeführt.

Verwendete Bibliotheken:

- pandas – Datenverarbeitung
- scikit-learn – Vektorisierung sowie LDA und LSA
- Gensim – Berechnung der Topic Coherence
- NLTK – Tokenisierung, POS-Tagging und Lemmatisierung mit WordNet

Für die Textdarstellung wurden CountVectorizer für Bag-of-Words und TfidfVectorizer für TF-IDF eingesetzt. Die Themenanalyse erfolgte mit LatentDirichletAllocation und TruncatedSVD aus scikit-learn.

In der ursprünglichen Analyse wurden zwölf LDA-Topics anhand der Topic Coherence ausgewählt und für LSA ebenfalls zwölf Dimensionen verwendet. Ergänzend wurde untersucht, ob eine Lemmatisierung die thematische Abgrenzung verbessert. Dabei wurde das Vokabular zwar reduziert, eine bessere Interpretierbarkeit der Themen zeigte sich jedoch nicht.

## Notebook

Die vollständige Analyse mit Code, Erläuterungen und Ergebnissen befindet sich im Jupyter Notebook `Datenanalyse.ipynb`.
