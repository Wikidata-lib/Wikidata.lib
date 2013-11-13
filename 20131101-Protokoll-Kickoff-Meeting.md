Bachelorprojekte am HPI
=======================
- Prof. Naumann stellt Bachelorprojekte am HPI allgemein vor
- Auswahl der Studenten
- erstes Semester Teilzeit, zweites Vollzeit
- Zeitrahmen, regelmäßige Organisation
- Bewertung
- Bachelorarbeit - Umfang, Inhalt

BP2013N2 speziell
-----------------
- Lernveranstaltung, aber auch Gewinn für Wikidata
- Bewertung: Teamarbeit, Projektnote für alle, Individuelle Note aus Vorträgen und Bachelorarbeit
- Bonus: Libs/Tools schon verwendet vor Ende des Bachelorprojekts

Geschichte von Wikidata
-------------------------
- Vorzeigeprojekt von Wikimedia Deutschland
- große freiwillige Community, > 600 Leute mit >100 Edits/30 Tage

Vorstellung der BP-Themen (VW, CD)
----------------------------------
- Intelligente Formulare
  - schon länger bei Wikidata geplant
  - gibt bereits Code, nicht gut gelaufen
  - „Objekte mit Eigenschaften A,B haben normalerweise auch C und D“
  - Muss ohne manuelle Wartung machbar sein
  - Einfacherer, flexibler Ansatz: Welche Eigentschaften werden i.d.R. zusammen verwendet?
  - „Wikidata muss flexibel genug sein, um einen sehr großen Teil der System-Komplexität zu repräsentieren“
  - bereits halbwegs Vollständig, „noch 1 Monat Arbeit für 1 Person“
  - „Suggester“-Engine, Modul für mediawiki-API, wird noch nicht verwendet (basiert auf Hadoop)

  - Instance-of-Methode (unsere)
    - Erst Attribute anlegen, daraufhin „Typ“ vorschlagen

  - „Alle“ Ansätze entwickeln, dann vergleichen
  - es gibt eine Übersichtsseite mit Properties in Wikidata (auch nach Themen sortiert)
  - nicht nur Existenz von Properties, sondern auch deren Wert berücksichtigen
  - Team aufteilen in Backend (Algorithmen) und Frontend
  - Frontend: Statt neue UI die Autovervollständigung ersetzen/verändern durch Algorithmen-basierte Suche statt Präfixsuche
  - es existiert bereits ein klassifizierungs-basiertes Eingabesystem, funktioniert nicht mehr, da das relevante Klassifizierungs-Attribut nicht mehr existiert
  - Interesse vom BP (CD, MF)

- PubSubHubbub
  - von den Anforderungen her nicht schwierig
  - kann leicht vom System entkoppelt werden
  - Problem: Skalierung
  - GSoC-Projekt, wurde nicht durchgeführt
  - gibt einige Abnehmer eines anderen Protokolls, wird demnächst abgeschaltet
  - Problem: Kann jeweils Wochen dauern, auf Produktiv-Servern eingesetzt zu werden
  - Interesse vom BP [SB]

- Libs
  - Python und Java machen Sinn, es gibt bereits eine schlechte Python-Variante und einen Entwurf für Java
  - „Requirement“ für Beispielanwendungen
  - Unser Vorschlag: damit anfangen
  - pyWikipedia / pyWikidata gibt es schon, ansehen und testen / Qualität überprüfen
    - wird von Bots bereits verwendet
  - es gibt Java-Bots, Problem: Keine „Kunden“ für neue Java-Bibliothek
  - Wikidata-Datenmodell in Java implementieren / API-Anbindung

- Beispielanwendungen
  - gibt schon welche von der Community (Wikidata:Tools)
  - Erst Anwendungen überlegen, und dafür dann Libs entwickeln

- Plausibilitätscheck
  - selbe Logik wie Suggester, nur andersrum
  - Könnte man verbinden

- Suche verbessern
  - vermutlich nicht relevant, da 2 Mitarbeiter daran arbeiten

- Integration
  - nichts spezifisches, soll nicht online verwendet werden
  - Eher eine Lib, die auf extra-Instanzen die Integration mittels leichter Anpassung erlaubt
  - Seite auf Wikidata „Zusatzprojekte“, auf der ein ähnliches Projekt beschrieben (allerdings nicht umgesetzt) ist

- Amazon-Spiegelung
  - Erstmal ungeeignet (Daten liegen in der SQL-DB als JSON-Blobs)
  - Potentielle Möglichkeit: In NoSQL-DB verpackt anbieten, da auf Dokumente ausgelegt
  - Statt Amazon eher mit der Wikimedia Test-Cloud
  - „Stößt nicht auf Begeisterung“ [Naumann]

Entscheidung für Projekte
-------------------------
  - [4/6] Suggester (Intelligente Formulare)
  - [2/6] PubSubHubbub

Infrastruktur
-------------
- Wikipedia/Wikidata wird von der Foundation in den USA gehostet, manche (technologische) Aspekte werden nicht zugelassen
- Staging-Cloud der Foundation, neue (fast)-produktiv Instanzen

Accounts
--------
  - Entwickler-Accounts bei Wikimedia beantragen
    -> Zugriff auf Wikimedia Labs
  - Links von WM-Team

Termine
-------
  - Regelmäßige Treffen
  - wöchentliche Telefonate, Agenda vorab, Statusupdates, regelmäßiger Termin wird noch festgelegt

Kommunikation BP<->WM
---------------------
  - Kommikationsbeauftragter (evtl. 1 Organisation, 1 pro aktivem Projekt)
  - E-Mail, Adressen sind im BP2013-N2-Verteiler
  - grundsätzlich Englisch

Weiteres Vorgehen
-----------------
  - Projekte, Aufwand, was kann getan werden
  - Terminvorschläge
  - Teamaufteilung (per Mail rumschicken)
  - in 2 Wochen wieder treffen/telefonieren