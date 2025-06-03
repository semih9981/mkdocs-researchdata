# Verarbeitung & Analyse

## Datenverarbeitung

- Parsing der FASTA-Dateien
- Erstellung von Sequenzstatistiken
- Mustererkennung
- Klassifikation nach Strangrichtung

## Crunching mit Python

Tools: `pandas`, `matplotlib`

Beispiele:
- Sequenzlänge
- Nukleotidzusammensetzung (A, T, C, G)


## Sequenzvereinfachung & Export

### Vereinfachte Darstellung statt Vollsequenz 
- Vollständige RNA-Sequenzen sind oft mehrere 1000 Basen lang
Für Wikibase-Integration ungeeignet → Entscheidung für gekürzte Darstellung
- Stattdessen: Speicherung von Länge, Basenhäufigkeit, ID, Typ

### Export zur Wikibase Cloud Instanz
- Strukturierte Items: RNA, Organismus, Länge, Strang, Typ
- SPARQL-Queries ermöglichen z. B.: 
  - Alle RNAs eines bestimmten Organismus 
  - Filterung nach Längenbereichen oder RNA-Typ
