# Projekt-Dokumentation

Simon Veljkovic, Agachan Atputharasa

| Datum | Version | Zusammenfassung                                              |
| ----- | ------- | ------------------------------------------------------------ |
| 10.01.2025 | 0.0.1 | Wir haben den Projektantrag eingereicht und das Projekt begonnen. |
| 17.01.2025 | 0.0.2 | Wir haben unsere Planung vervollständigt und mit der Implementation der Grundfunktionen begonnen. |
| 24.01.2025 | 0.0.3 | Wir haben das Login implementiert. |
| 31.01.2025 | 0.0.4 | Wir haben die Grundfunktionen für die Umfragen implementiert und mit dem Aufsetzen der DB begonnen. |                                            | 21.02.2025 | 0.0.5 | Wir haben die Speicher- und Löschfunktion umgesetzt und versucht, die Auswertung per Diagramme zu implementieren. |
| 28.02.2025 | 0.0.6 | Wir haben den PDF/CSV Export eingebaut, und versucht, den Code von Fehlern zu befreien. |                                                        | 07.03.2025 | 1.0.0 | Wir haben die Dokumentation vervollständigt, den Mahara-Eintrag geschrieben und das Projekt beendet. |                                                             

## 1 Informieren

### 1.1 Ihr Projekt

Projektidee:

Wir haben uns als Gruppe dazu entschieden, das Projekt mit den Programmiersprachen HTML, CSS, JavaScript für das Frontend sowie MongoDB für das Backend zu einer Website umzusetzen. Diese Anwendung bietet dem Benutzer die Möglichkeit, eine feste Umfrage auszufüllen und auch eigene Umfragen zu erstellen und zu verwalten. Dabei werden wir die folgenden drei Hauptfunktionen implementieren:

1.Korrekte Interaktion mit den Buttons: Nur eine Antwortmöglichkeit soll möglich sein.

2.Login: Die Benutzer sollen sich mit Benutzername und Passwort einloggen können.

3.Verwaltung: Antworten sollen gespeichert werden und die selbstkreierten Unfragen sollen gespeichert und gelöscht werden können.

Projektorganisation:

Wir haben dieses Projekt organisiert, indem wir eine Discord-Gruppe erstellt haben, GitHub zur Zusammenarbeit genutzt und Daily-Meetings vereinbart haben.

Deklaration der Vorkenntnisse:

HTML: Gute Vorkenntnisse 

CSS: Gute Vorkenntnisse

JavaScript: Ordentliche Vorkenntnisse

MongoDB: Ordentliche Vorkenntnisse

IPERKA: Sehr gute Kenntnisse, da wir es regelmässig im Lernatelier anwenden.


### 1.2 User Stories

| US-№ | Verbindlichkeit | Typ  | Beschreibung                       |
| ---- | --------------- | ---- | ---------------------------------- |
| 1    | Muss            | Funktional | Als ein User möchte ich, dass ich die Möglichkeit habe, eine fixe Umfrage auszufüllen. |
| 2    | Muss            | Funktional | Als ein User möchte ich, dass ich mich auf der Website registrieren kann mit Username und Passwort. |                           | 3    | Muss            | Funktional | Als ein User möchte ich, dass ich eigene Umfragen erstellen kann. |
| 4    | Muss            | Funktional | Als ein User möchte ich, dass ich meine Umfragen speichern und löschen kann. |



## 2 Planen

### 2.1 Software-Architektur

Die Architektur der App basiert auf einer klaren Trennung der Verantwortlichkeiten:

•	Frontend (UI): Verantwortlich für die Benutzeroberfläche und Interaktionen.

•	Backend (Logik): Speicherung der Daten.

•	Datenmanagement: Speicherung und Löschung der Berechnungen und Benutzerdaten.

### 2.2 Mockup

![image](https://github.com/user-attachments/assets/63466f97-9f2b-485c-b5ef-8dc8fc7f830c)



### 2.3 Testfälle

| TC-№ | Ausgangslage | Eingabe | Erwartete Ausgabe |
| ---- | ------------ | ------- | ----------------- |
| 1.1  | Website geöffnet | Alle Antwortmöglichkeiten werden angeklickt | Nur eine Antwort bleibt gespeichert |
| 2.1  | Website geöffnet | Ganze Umfrage ausgefüllt | Auswertung als Diagrammform |
| 3.1  | Website geöffnet, Eigene Umfrage erstellt | Umfrage speichern Button angeklickt | Die Umfrage wird gespeichert. |
| 4.1  | Website geöffnet | Verwaltung der eigenen Umfragen | Bearbeiten/Löschen Button erscheint |

### 2.4 Meilensteine

Meilenstein 1: Anforderungsanalyse und Entwurf (bis 17.01.2025)

•	Projektidee und Hauptanforderungen festlegen.

•	Anwendungsarchitektur und Mockups entwickeln.

Meilenstein 2: Grundlegende Funktionalitäten implementieren (bis 31.01.2025)

•	Benutzeroberfläche entwerfen und erstellen.

•	Login implementieren.

•	Basisfunktion für die Umfragen implementieren.

Meilenstein 3: Erweiterte Funktionen und Speicherung (bis 21.02.2025)

•	Speicher- und Löschfunktion entwickeln (Backend).

•	Grafische Auswertung per Diagramme.

•	PDF und CSV Export implementieren.

Meilenstein 4: Fehlerbehebung und Optimierung (bis 28.02.2025)

•	Systemtest: Alle Funktionen testen, Fehler beheben.

•	Allfällige Design-Anpassungen vornehmen.

Meilenstein 5: Projektabschluss (bis 07.03.2025)

•	Dokumentation vervollständigen.

•	Endgültige Testberichte erstellen.

•	Fertige Version auf GitHub bereitstellen.

•	Portfolioeintrag schreiben und abgeben.


## 3 Entscheiden

### 3.1 Gründe für die Wahl der Technologie

Nach gründlicher Analyse der möglichen Technologien haben wir uns entschieden, HTML, CSS und JavaScript fürs Frontend und MongoDB für das Backend zu nutzen. Die Entscheidung beruht auf folgenden Überlegungen:
1.	Kenntnisse seit über einem Jahr:  HTML und CSS, JavaScript und MongoDB benutzen wir schon seit mehr als einem Jahr, sodass uns dies die Entwicklung schneller ermöglicht, da wir uns nicht erst in eine neue Sprache einarbeiten müssen. sondern wir das Gelernte einfach anwenden können.
2.	Single-Page-Applikation: Da unsere Website Daten speichern soll und sie interaktiv ist, eignet sich eine SPA besser als eine MPA.

Abgelehnte Alternativen:
•	Konsolen-App mit C#: Zu wenig Spielraum für das Design und gewisse Funktionen sind da schwieriger zu implementieren.
•	Mobile-App mit MAUI: Zu wenig Erfahrung mit der Sprache.

### 3.2 Präferenzmatrix

![image](https://github.com/user-attachments/assets/473855f9-026a-41d1-b87b-b19e5911876d)




## 4 Realisieren

### 4.1 Realisierungsbericht

Meilenstein 1: Anforderungsanalyse und Entwurf (bis 17.01.2025)

•	Projektidee und Hauptanforderungen festlegen.

•	Anwendungsarchitektur und Mockups entwickeln.

Ergebnis: Alles zeitlich erfüllt.

Meilenstein 2: Grundlegende Funktionalitäten implementieren (bis 31.01.2025)

•	Benutzeroberfläche entwerfen und erstellen.

•	Login implementieren.

•	Basisfunktion für die Umfragen implementieren.

Ergebnis: Aufgrund eines Fehlers, welches später in einem anderen Feature passiert ist, mussten wir den Code umbauen. Dies hat leider dafür gesorgt, das man sich nicht mehr ausloggen kann.

Meilenstein 3: Erweiterte Funktionen und Speicherung (bis 21.02.2025)

•	Speicher- und Löschfunktion entwickeln (Backend).

•	Grafische Auswertung per Diagramme.

•	PDF und CSV Export implementieren.

Ergebnis: Die grafische Auswertung per Diagramme funktionierte so schlecht, dass wir es leider nicht in unserem Code behalten konnten.

Meilenstein 4: Fehlerbehebung und Optimierung (bis 28.02.2025)

•	Systemtest: Alle Funktionen testen, Fehler beheben.

•	Allfällige Design-Anpassungen vornehmen.

Ergebnis: Keine Design-Anpassungen waren nötig, jedoch brauchten wir länger für den Systemtest, da unser Programm durch die genannten Fehler angefangen hat zu spinnen.

Meilenstein 5: Projektabschluss (bis 07.03.2025)

•	Dokumentation vervollständigen.

•	Endgültige Testberichte erstellen.

•	Fertige Version auf GitHub bereitstellen.

•	Portfolioeintrag schreiben und abgeben.

Ergebnis: Trotz nicht einwandfreiem Code waren diese Aufgaben noch rechtzeitig machbar.

## 5 Kontrollieren

### 5.1 Testumgebung

Testumgebung: 
Betriebssystem: Windows 11

Entwicklungsumgebung: Microsoft Visual Studio Code 

### 5.2 Testprotokoll

| TC-№ | Datum | Resultat | Tester |
| ---- | ----- | -------- | ------ |
| 1.1  | 07.03.2025 | OK | Simon Veljkovic |
| 2.1  | 07.03.2025 | NOK | Simon Veljkovic |
| 3.1  | 07.03.2025 | OK | Simon Veljkovic |
| 4.1  | 07.03.2025 | OK | Simon Veljkovic |

### 5.3 Testfazit

Testfall 2 funktioniert nicht, da wir die grafische Darstellung per Diagramme nicht richtig umsetzen konnten. Alles andere ist aber zufriedenstellend.

## 6 Auswerten


