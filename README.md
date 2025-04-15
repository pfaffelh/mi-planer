# mi-planer
Streamlit App für die Studiengangkoordination am Mathematischen Institut in Freiburg

Ziel der App ist es, Abläufe der Studiengangkoordination zu automatisieren, und jederzeit einen Überblick der anstehenden Aufgaben zu haben. 

## Datenbank-Struktur

Jeder _Prozess_ (zB Erstellung des Modulhandbuchs) hat dabei
* eine Beschreibung
* ein zugehöriges Datum (das ist zB der Semesterstart oder Start der Vorlesungszeit. Relativ dazu können weitere Termine berechnet werden.)
* einen Verantwortlichen
* Quicklinks (zur Beschreibung des Prozesses)
* eine Wiederholungsfrequenz (meist semesterweise, jahresweise, oder nach Einzelfällen)

Jeder Prozess besteht aus mehreren _Aufgaben_ (zB Versand einer Mail an die Dozent:innen). Eine Aufgabe ist dabei ein kleinerer Teilschritt eines Prozesses. 
Jede Aufgabe hat:
* entweder einen zugehörigen Prozess, oder zugehörige andere Aufgaben, wenn man Aufgaben in kleinere Teilaufgaben zerlegen will.
* eine Beschreibung
* eine Fälligkeit (Zeitraum); dieser kann relativ zur Fälligkeit des zugehörigen Prozesses bzw der zugehörigen anderen Aufgaben angegeben sein.
* einen Verantwortlichen
* Quicklinks (zur Beschreibung der Aufgabe)
* Ein oder mehrere Vorlagen, zB für eine Mail oder einen anderweitigen Text

## Ansichten

Die Hauptansicht soll die relevanten Prozesse darstellen. 

Es soll Umschalter geben: 
* alle Prozesse / Prozesse, an denen ich beteiligt bin
* alle Prozesse / nur Prozesse, die noch nicht fertig sind

Clickt man auf einen Prozess, werden die zugehörigen Aufgaben angezeigt

Eine weitere Ansicht soll "meine anstehenden Aufgaben" darstellen










