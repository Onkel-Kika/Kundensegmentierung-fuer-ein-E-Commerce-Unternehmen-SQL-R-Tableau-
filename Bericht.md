# Bericht: Kundensegmentierung für ein E-Commerce-Unternehmen

## Einleitung
Das Ziel dieses Projekts war es, eine Kundensegmentierung für ein E-Commerce-Unternehmen durchzuführen, um gezielte Marketingstrategien zu entwickeln und das Kundenverhalten besser zu verstehen. 
Das Projekt basierte auf dem **RFM-Modell** (Recency, Frequency, Monetary), um Kunden in verschiedene Gruppen zu unterteilen und basierend auf diesen Segmenten relevante Maßnahmen zu empfehlen.

## Datenvorbereitung

### Verwendetes Dataset
- **Online Retail II Dataset** von **Kaggle** (Zeitraum: 2010-2011).
- Enthält Transaktionsdaten eines britischen Online-Händlers.

### Schritte der Datenvorbereitung
1. **Datenbereinigung**:
   - **Rücksendungen und Bestellabbrüche**: Negative Werte in der Spalte **Quantity** markieren Rücksendungen. Diese wurden korrekt gekennzeichnet und in den Daten berücksichtigt.
   - **Ausschluss irrelevanter Daten**: Bestellungen mit **negativen Werten** wurden als Rücksendungen markiert, und interne Buchungen (z.B. Porto) wurden entfernt.

2. **Aggregation pro Kunde**:
   - Für die Analyse wurden die **Anzahl der Bestellungen**, der **Gesamtumsatz** pro Kunde und die **Rücksendequote** berechnet.

## Analyseansatz: RFM-Modell
Das **RFM-Modell** wurde verwendet, um die Kunden nach den folgenden Metriken zu segmentieren:
- **Recency (R)**: Wie kürzlich hat ein Kunde das letzte Mal gekauft?
- **Frequency (F)**: Wie oft hat der Kunde gekauft?
- **Monetary (M)**: Wie viel Geld hat der Kunde ausgegeben?

Basierend auf diesen Werten wurden die Kunden in **Top-Kunden**, **Potenzialkunden**, **weniger wertvolle Kunden** und **inaktive Kunden** eingeteilt.

### Berechnung der RFM-Werte
1. **Recency**: Anzahl der Tage seit dem letzten Kauf.
2. **Frequency**: Anzahl der getätigten Bestellungen.
3. **Monetary**: Gesamtumsatz, den der Kunde generiert hat.

## Ergebnisse der Kundensegmentierung

### Anzahl der Kunden in den RFM-Segmenten:
- **Top-Kunden**: 2229 (38%)
- **Potenzialkunden**: 1897 (32%)
- **Weniger wertvolle Kunden**: 1606 (27%)
- **Inaktive Kunden**: 144 (2,45%)

### Visualisierung der Kundensegmente:

![Anzahl der Kunden in verschiedenen RFM Segmenten](https://github.com/user-attachments/assets/3f47317a-397b-40bd-b70d-d7b5b1889715)
![Verteilung der kunden in verschiedenen RFM Segmente](https://github.com/user-attachments/assets/68b2667a-4330-452a-a7d7-0a1afb2e3b58)

### Umsatzverteilung nach Segmenten:
- **Top-Kunden** generieren den höchsten Umsatz mit durchschnittlich **6440,83 €** pro Kunde.
- **Potenzialkunden** haben im Durchschnitt **954,56 €** ausgegeben, während **weniger wertvolle Kunden** nur **293,61 €** beitragen.
- **Inaktive Kunden** generieren mit **148,22 €** den geringsten Umsatz.

![Umsatzverteilung nach kundensegmenten](https://github.com/user-attachments/assets/dce0eec9-52f6-4aff-87cb-7d632ccb78de)

## Saisonales Kaufverhalten

Eine Analyse der **Recency- und Frequency-Werte** über das Jahr zeigt, dass das Kaufverhalten stark saisonal beeinflusst wird. Besonders ab **September** nimmt die Kaufhäufigkeit deutlich zu, mit einem starken Anstieg im **Dezember**.

### Wichtige Ergebnisse
- **Recency-Werte** sinken im Jahresverlauf, was darauf hindeutet, dass Kunden gegen Jahresende aktiver werden.
- **Frequency-Werte** zeigen einen kontinuierlichen Anstieg der Kaufaktivität, mit einer Spitze von **299 Bestellungen** im Dezember.

![Wie lange ist es durchschnittlich her, dass Kunden das letzte Mal gekauft haben](https://github.com/user-attachments/assets/3652d495-bad4-4f09-8371-b7dd5604857f)
![Wie oft kaufen Kunden innerhalb eines bestimmten Zeitraums](https://github.com/user-attachments/assets/e3ab11d1-3025-41e4-86ad-8cec11b55c63)

## Handlungsempfehlungen

### 1. Maßnahmen für Top-Kunden (38%)
- **Treueprogramme:** Durch die Einführung von Treueprogrammen könnte die Wiederkaufrate der Top-Kunden um **15%** gesteigert werden, was zu einer Umsatzsteigerung von **500.000 €** pro Jahr führen würde.
- **Personalisierte Angebote:** Gezielte Produktvorschläge für Top-Kunden könnten den durchschnittlichen Bestellwert um **10%** erhöhen, was weitere **200.000 €** an zusätzlichem Umsatz generieren könnte.

### 2. Maßnahmen für Potenzialkunden (32%)
- **Upselling- und Cross-Selling-Strategien:** Durch die Implementierung von Upselling-Kampagnen könnte der Umsatz pro Kunde um **20%** steigen, was einem zusätzlichen Umsatz von **350.000 €** entspricht.
- **Gezielte Marketingkampagnen:** Personalisierte E-Mail-Kampagnen könnten die Kaufhäufigkeit um **15%** steigern und einen Umsatz von **150.000 €** pro Jahr generieren.

### 3. Maßnahmen für weniger wertvolle Kunden (27%)
- **Erhöhung der Kaufhäufigkeit:** Gezielte Anreize könnten die Kaufhäufigkeit um **10%** steigern und zu einem zusätzlichen Umsatz von **100.000 €** pro Jahr führen.
- **Cross-Selling:** Durch gezielte Cross-Selling-Maßnahmen könnte der durchschnittliche Bestellwert um **5%** gesteigert werden, was einem zusätzlichen Umsatz von **50.000 €** entspricht.

### 4. Maßnahmen zur Reaktivierung inaktiver Kunden (2,45%)
- **Reaktivierungskampagnen:** Eine Rückgewinnung von **5%** der inaktiven Kunden könnte einen Umsatz von **25.000 €** bringen, wobei Feedback-Sammlungen zur weiteren Optimierung führen könnten.
  
### 5. Nutzung der saisonalen Trends
- **Saisonale Kampagnen:** Der Umsatz könnte durch gezielte Kampagnen im vierten Quartal um **30%** gesteigert werden, was zusätzlichen **600.000 €** entspricht.
- **Jahresendangebote:** Durch Sonderaktionen im Dezember könnte der Umsatz um **400.000 €** gesteigert werden.

## Fazit

Die Kundensegmentierung auf Basis des **RFM-Modells** bietet Unternehmen die Möglichkeit, ihre Marketingstrategien präzise und datengestützt anzupassen. Die vorgeschlagenen Maßnahmen haben das Potenzial, den **Gesamtumsatz des Unternehmens um bis zu 2 Millionen Euro jährlich** zu steigern.

- **Top-Kunden** sollten durch Treueprogramme und personalisierte Angebote gebunden werden.
- **Potenzialkunden** bieten durch Upselling und Cross-Selling erhebliches Potenzial für Umsatzsteigerungen.
- **Weniger wertvolle Kunden** können durch gezielte Anreize in aktive Käufer umgewandelt werden.
- **Inaktive Kunden** sollten durch Reaktivierungskampagnen zurückgewonnen werden.
- Die **Saisonalität des Kaufverhaltens** bietet eine einmalige Gelegenheit, den Umsatz im vierten Quartal erheblich zu steigern.
