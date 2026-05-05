# Data Analytics mit SQL & Python

**Von Daten zur Entscheidung**  
5 Tage Intensivkurs, 40 UE, mit SQL, Python, Pandas, Visualisierung und Abschlussprojekt.

Dieser Kurs ist für Einsteigerinnen und Einsteiger konzipiert. Programmierkenntnisse sind nicht erforderlich, aber grundlegende Computerkenntnisse und Interesse an Daten sind hilfreich.

## Kursziel

Am Ende der Woche kannst du:

- Daten aus CSV-Dateien und einfachen Datenbanken laden
- mit SQL Tabellen abfragen, filtern, gruppieren und verbinden
- mit Python und Pandas Daten prüfen, bereinigen und analysieren
- Diagramme mit Matplotlib und Seaborn erstellen
- Analyseergebnisse in klare Erkenntnisse und Empfehlungen übersetzen
- eine kurze datenbasierte Entscheidungsvorlage präsentieren

## Benötigte Tools

Empfohlen:

- Jupyter Notebook oder JupyterLab
- Python 3.10+
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SQLite über Python `sqlite3`

Optional:

- Google Colab
- Plotly
- Power BI

Einige Notebooks laden Daten direkt von GitHub. Dafür brauchst du eine aktive Internetverbindung.

## Ordnerstruktur

```text
Tag 1/
  Day_1_Data_Analytics_SQL_Python.ipynb
  Day_1_Data_Analytics_SQL_Python_Exercises.ipynb
  data_practice_tables/

Tag 2/
  Day_2_Data_Analytics_SQL_Python.ipynb
  Day_2_Data_Analytics_SQL_Python_Exercises.ipynb

Tag 3/
  Day_3_Data_Analytics_SQL_Python.ipynb
  Day_3_Data_Analytics_SQL_Python_Exercises.ipynb

Tag 4/
  Day_4_Data_Analytics_SQL_Python.ipynb
  Day_4_Data_Analytics_SQL_Python_Exercises.ipynb

Tag 5/
  Day_5_Data_Analytics_SQL_Python.ipynb
  Day_5_Data_Analytics_SQL_Python_Exercises.ipynb
```

Pro Tag gibt es:

- ein Hauptnotebook für Input, Beispiele und gemeinsame Arbeit
- ein Exercise-Notebook für Gruppenarbeit, Wiederholung und Transfer

## So arbeitest du mit den Notebooks

1. Öffne zuerst das Hauptnotebook des jeweiligen Tages.
2. Führe die Setup-Zellen am Anfang aus.
3. Lies die Markdown-Erklärungen vor den Code-Zellen.
4. Führe Code-Zellen Schritt für Schritt aus.
5. Bearbeite danach das Exercise-Notebook.
6. Ersetze Platzhalter wie `_____` durch passende Spaltennamen, Funktionen oder SQL-Bausteine.
7. Schreibe bei Reflexionsfragen kurze Antworten direkt ins Notebook oder in deine Notizen.

Wenn eine Zelle einen Fehler zeigt:

- Prüfe zuerst, ob die Setup-Zelle ausgeführt wurde.
- Prüfe, ob ein Platzhalter `_____` noch nicht ersetzt wurde.
- Prüfe, ob du eine Internetverbindung hast, wenn externe Daten geladen werden.

## Kursüberblick

### Tag 1: SQL-Grundlagen

**Fokus:** Einstieg in Data Analytics und einfache SQL-Abfragen.

Inhalte:

- Was ist Data Analytics?
- relationale Datenbanken
- `SELECT`, `FROM`, `WHERE`
- Filtern, Sortieren, Begrenzen
- `COUNT`, `SUM`, `AVG`
- erste `GROUP BY`-Analysen

Exercise:

- Household-Budget-Daten
- Einnahmen und Ausgaben
- Kategorienanalyse
- Monatsanalyse

Zeitlich passt Tag 1 gut für einen Einstiegstag. Die geplante HAVING-Vertiefung aus der Kursplanung ist in den aktuellen Materialien sinnvoller auf Tag 2 verschoben, weil HAVING didaktisch besser nach sicherem `GROUP BY` funktioniert.

### Tag 2: SQL-Vertiefung, Joins und Datenmodellierung

**Fokus:** Tabellen verbinden und aggregierte Fragen beantworten.

Inhalte:

- `GROUP BY` wiederholen
- Unterschied zwischen `WHERE` und `HAVING`
- `INNER JOIN`
- mehrere Tabellen verbinden
- Subqueries
- CTEs mit `WITH`
- Primärschlüssel und Fremdschlüssel

Hauptnotebook:

- Shop-Daten mit `orders`, `customers`, `products`

Exercise:

- Teil A: 30 Minuten Refresh mit Fitness-Bookings
- Teil B: Fitness-Daten als Transferübung

Zeitlich ist Tag 2 realistisch, wenn Joins und HAVING nicht zu schnell behandelt werden. Für Subqueries und CTEs reichen kurze, einfache Beispiele; sie müssen an diesem Tag noch nicht vollständig automatisiert beherrscht werden.

### Tag 3: Python, Pandas und Visualisierung

**Fokus:** Wechsel von SQL zu Python.

Inhalte:

- Python-Grundlagen
- Variablen, Datentypen, Bedingungen, Schleifen
- Pandas DataFrames
- Filtern, Sortieren, Kennzahlen
- Merge/Join in Pandas
- Matplotlib und Seaborn
- einfache Zeitreihen
- Mini-Projekt

Exercise:

- Teil A: 30 Minuten SQL-Recap mit Household Budget
- Teil B: Pandas mit `shop_joined`
- Teil C: Transfer mit `fitness_joined`

Tag 3 ist inhaltlich sehr voll. Der Zeitplan ist machbar, wenn Python-Grundlagen kompakt bleiben und der Fokus schnell auf Pandas und Visualisierung wechselt. Für absolute Anfängerinnen und Anfänger sollte die Dozentin bei Schleifen und `input()` nicht zu lange verweilen.

### Tag 4: Explorative Datenanalyse & Reporting

**Fokus:** EDA an realistischeren Daten.

Inhalte:

- Data Cleaning Recap
- Job-Posting-Daten verstehen
- Gehaltsspannen aus Text extrahieren
- statistische Kennzahlen
- Verteilungen und Ausreißer
- Gruppenvergleiche
- Korrelationen
- SQL + Python für Reporting
- Erkenntnisse formulieren

Hauptnotebook:

- `Uncleaned_DS_jobs.csv` aus dem Repository `eyowhite/Messy-dataset`
- Business-Frage: Welche Faktoren hängen mit Data-Science-Gehältern zusammen?

Exercise:

- Teil A: Shop-Warm-up als Recap zu Tag 3
- Teil B: messy HR Data für Cleaning, EDA und Reporting
- Mini-Projekt: HR-Frage zu Gehaltsstruktur, Zufriedenheit oder Fluktuationsrisiko

Tag 4 passt gut zur Kursplanung. Die Nutzung von Job-Posting- und HR-Daten ist stärker als ein kleiner sauberer Shop-Datensatz, weil typische Datenprobleme sichtbar werden. Wichtig ist, die Cleaning-Schritte zu begrenzen: Ziel ist eine brauchbare Analysebasis, kein perfekter Datensatz.

### Tag 5: Abschlussprojekt & Storytelling mit Daten

**Fokus:** Ergebnisse überzeugend präsentieren und eine Business Analytics Challenge bearbeiten.

Inhalte:

- von Analyse zur Entscheidung
- Data Storytelling
- Zielgruppe, Business-Frage, KPI, Visualisierung, Empfehlung
- Beispiele mit cleaned datasets
- KI-gestützte Tools reflektiert nutzen
- Abschlussprojekt in Gruppen
- Präsentation und Feedback

Hauptnotebook:

- `Cleaned_DS_jobs2.csv`
- `cleaned_messy_HR_data.csv`
- beide dienen als Storytelling-Vorlagen

Exercise:

- Teil A: 30 Minuten EDA-Warm-up mit Household Budget
- Teil B: Storytelling-Übungen
- Teil C: Gruppenprojekt mit Warehouse, IMDB oder Healthcare messy data

Der Tag ist zeitlich stimmig: 30 Minuten EDA-Warm-up, danach ungefähr 2 Stunden Storytelling, und am Nachmittag etwa 3 Stunden Gruppenprojekt. Für das Projekt ist wichtig, dass jede Gruppe eine klare Business-Frage wählt und nicht versucht, den gesamten messy Datensatz vollständig zu bereinigen.

## Einschätzung zur Kursplanung

Die aktuellen Materialien passen insgesamt gut zur ursprünglichen Planung:

- Tag 1 baut solide SQL-Grundlagen auf.
- Tag 2 vertieft SQL mit Joins, HAVING, Subqueries und CTEs.
- Tag 3 führt Python und Pandas ein und verbindet die SQL-Denkweise mit DataFrames.
- Tag 4 nutzt realistischere messy datasets für EDA und Reporting.
- Tag 5 führt alles in Storytelling und Abschlussprojekt zusammen.

Kleine didaktische Anpassungen gegenüber der ursprünglichen Planung sind sinnvoll:

- `HAVING` wird praktisch ab Tag 2 vertieft, nicht schon voll in Tag 1.
- Data Cleaning ist über Tag 3-5 verteilt, mit Schwerpunkt an Tag 4.
- Tag 5 nutzt cleaned datasets für Storytelling, damit die Projektgruppen nachmittags mehr Orientierung haben.

## Empfohlener Tagesrhythmus

Für jeden Kurstag:

1. Kurzer Rückblick auf den Vortag
2. Warm-up im Exercise-Notebook
3. Input im Hauptnotebook
4. Gemeinsames Code-Along
5. Gruppenübung oder Mini-Projekt
6. Kurze Reflexion: Was bedeutet das Ergebnis fachlich?

## Datensätze

Lokale Kursdaten:

- Household Budget
- Shop-Daten
- Fitness-Daten

Externe Daten:

- `eyowhite/Messy-dataset`
- Raw CSV-Dateien von GitHub für Job Posting, HR, Warehouse, IMDB und Healthcare

Wenn externe Daten nicht geladen werden:

- Internetverbindung prüfen
- Notebook-Zelle erneut ausführen
- bei Bedarf CSV manuell aus GitHub herunterladen

## Nützliche Ressourcen

- SQL practice platform: https://www.sql-practice.online/
- Data Science Interview Questions: https://github.com/youssefHosni/Data-Science-Interview-Questions-Answers/tree/main
- Messy datasets: https://github.com/eyowhite/Messy-dataset

## Abschluss

Das Ziel des Kurses ist nicht, möglichst viele Befehle auswendig zu lernen. Das Ziel ist, einen vollständigen Analyseprozess zu verstehen:

```text
Rohdaten -> Datenqualität prüfen -> Bereinigen -> Analysieren -> Visualisieren -> Erkenntnisse -> Entscheidung
```

Wenn du am Ende der Woche eine Datenfrage sauber strukturieren, mit SQL und Python untersuchen und als kurze Empfehlung präsentieren kannst, hast du den wichtigsten Schritt geschafft.
