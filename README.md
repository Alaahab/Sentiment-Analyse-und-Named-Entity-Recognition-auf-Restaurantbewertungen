# Sentiment Analyse und Named Entity Recognition auf Restaurantbewertungen

Diese Ausarbeitung ist Teil des Studiengangs Angewandte Künstliche Intelligenz (M. Sc.) im Modul Natural Language Processing an der Fachhochschule Südwestfalen. Ziel der Arbeit ist die Untersuchung von Methoden zur Stimmungsanalyse und Named Entity Recognition (NER) auf Restaurantbewertungen. Dabei werden verschiedene Machine Learning- und Deep Learning-Modelle wie Naive Bayes, LSTM und BERT verglichen.

## Inhaltsverzeichnis
1. [Einleitung](#einleitung)
2. [Grundlagen zu NLP](#grundlagen-zu-nlp)
3. [Daten und Explorative Datenanalyse](#daten-und-explorative-datenanalyse)
4. [Sentiment Analyse](#sentiment-analyse)
5. [Named Entity Recognition (NER)](#named-entity-recognition-ner)
6. [Ergebnisse und Vergleich der Modelle](#ergebnisse-und-vergleich-der-modelle)
7. [Fazit und Ausblick](#fazit-und-ausblick)

## Einleitung
Mit der zunehmenden Nutzung von Online-Bewertungen in der Gastronomiebranche sind Methoden zur Analyse von Kundenfeedback entscheidend geworden. Diese Arbeit zielt darauf ab, Stimmungsanalysen durchzuführen und Entitäten wie Gerichte oder Orte in den Bewertungen zu erkennen, um Einblicke in die Kundenzufriedenheit und spezifische Präferenzen zu gewinnen.

## Grundlagen zu NLP
Der Abschnitt behandelt grundlegende NLP-Techniken und -Modelle:
- **Transformer und LSTM**: Beide Modelltypen werden zur Verarbeitung von Sequenzdaten eingesetzt, wobei Transformer wie BERT oft eine höhere Genauigkeit erreichen.
- **Named Entity Recognition (NER)**: Hier werden Methoden zur Erkennung und Kategorisierung benannter Entitäten vorgestellt.

## Daten und Explorative Datenanalyse
Für die Analysen wurde ein Datensatz von Restaurantbewertungen aus Kaggle verwendet, der Bewertungen in Textform sowie eine Angabe zur Bewertungspolarität (positiv/negativ) enthält. In der Datenaufbereitung wurden Schritte wie Textnormalisierung, Tokenisierung und die Bereinigung von Stopwörtern durchgeführt.

## Sentiment Analyse
Die Arbeit vergleicht verschiedene Methoden zur Sentimentanalyse:
- **Naive Bayes**: Ein einfaches, probabilistisches Modell zur Klassifikation.
- **LSTM**: Ein rekurrentes neuronales Netzwerk, das gut für die Verarbeitung von Textsequenzen geeignet ist.
- **BERT**: Ein Transformer-Modell, das in der Lage ist, kontextbezogene Informationen besser zu erfassen.

## Named Entity Recognition (NER)
Für die Erkennung benannter Entitäten wurde ein eigenes Modell mit spaCy erstellt. Ziel ist es, spezifische Entitäten wie Restaurantnamen, Gerichte und Orte aus den Bewertungen zu extrahieren. Da vortrainierte Modelle die gewünschten Entitäten nicht optimal erkannten, wurde ein benutzerdefiniertes NER-Modell trainiert.

## Ergebnisse und Vergleich der Modelle
Die Ergebnisse der Sentiment Analyse zeigen, dass BERT mit einer Genauigkeit von 95 % das leistungsfähigste Modell ist. Naive Bayes und LSTM erreichten niedrigere Genauigkeiten von 74,5 % bzw. 73 %. Auch in der NER-Aufgabe schnitt das benutzerdefinierte spaCy-Modell akzeptabel ab, zeigte jedoch einige Fehlklassifikationen, die auf die begrenzte Menge an Trainingsdaten zurückzuführen sind.

## Fazit und Ausblick
Diese Arbeit zeigt, dass fortschrittliche Modelle wie BERT deutlich höhere Genauigkeiten erreichen als traditionelle Ansätze und dass NER eine wertvolle Ergänzung für die Analyse von Restaurantbewertungen sein kann. Für die Zukunft wird eine Erweiterung der Datenbasis und eine genauere Anpassung der Modelle empfohlen.

## Installation und Ausführung
### Voraussetzungen
- Python 3.9

### Installation
1. Klonen Sie das Repository:
   ```bash
   git clone https://github.com/Alaahab/Sentiment-Analyse-und-Named-Entity-Recognition-auf-Restaurantbewertungen.git
