# Übung 05

## Metainformationen 

* Newsletter
* Newsletter.dat
* Versionshistorie

| Wer    |    Was            |  Wo                     |Warum               |Wann     |Version |
|--------|-------------------|-------------------------|--------------------|---------|--------| 
| Tom    |Datenbank          |Backend (BitbucketLink)  |Bessere Performanz  |12.03.20 |0.0.1   |
| Til    |Frontend Framework |Frontend (BitbucketLink) |Einfache Handhabung |16.04.20 |0.0.2   |
| Timo   |...                |...                      |...                 |XY.xy.XY |0.0.X   |
  
## Einführung
* Leserkreis
  * Anwender, Entwickler, Auftraggeber
* Zweck des Systems  
  * Das System soll die Möglichkeit bieten sich für einen bezahlten Newsletter zu registrieren und diesen Online abrufen zu könne. 
    Mitarbeiter können Kundendaten abrufen daran Änderungen vornehmen und Kunden Nachrichten senden. Zudem können Mitarbeiter Newsletter erstellen,
    welche für die Abonnenten dann zur Verfügung stehen.
  
## Architekturtreiber
* Geschäftskontext
  * Wo die Datenbank sich befindet (Standort)
  * Welche DB benutzt wird
  * Was wollen sie denn?
* Stakeholder
  * siehe [Aufgabe 03 (Stakeholder)](https://github.com/SoenkeSobott/SWAR/blob/master/SWAR-01/Aufgabe-03.md#beschreibung-des-zu-entwickelnden-systems)
* Begründung für Architektur
  * MongoDB Atlas, weil passend für News und Kunden Struktur. Einfache Abbildung in JSON-Dokument, einfach skalierbar
  * DB in Europa, weil im einklang mit DSGVO

## Einflussfaktoren
* Technische Einflussfaktoren
  * siehe [Aufgabe 04 (Einflussfaktoren)](https://github.com/SoenkeSobott/SWAR/blob/master/SWAR-02/Aufgabe-04.md#was-ist-der-input-was-der-output-seiner-t%C3%A4tigkeit-in-bezug-auf-dokumente)
* Organisatorische Einflussfaktoren
  * siehe [Aufgabe 04 (Einflussfaktoren)](https://github.com/SoenkeSobott/SWAR/blob/master/SWAR-02/Aufgabe-04.md#was-ist-der-input-was-der-output-seiner-t%C3%A4tigkeit-in-bezug-auf-dokumente)

## Bausteinsicht (Komponentendiagramm)
![alt text](https://github.com/SoenkeSobott/SWAR/blob/master/SWAR-02/images/Komponentendiagramm.png "Komponentendiagramm")

## Laufzeitsicht (Sequenzdiagramm)
![alt text](https://github.com/SoenkeSobott/SWAR/blob/master/SWAR-02/images/Sequenzdiagramm.png "Sequenzdiagramm")

## Verteilungssicht (Verteilungsdiagramm)
![alt text](https://github.com/SoenkeSobott/SWAR/blob/master/SWAR-02/images/Verteilungsdiagramm.png "Verteilungsdiagramm")

## Architekturaspekte
* Persistenz
* Fehlerbehandlung
* Transaktionssteuerung
* Logging

## Projektaspekte
* Ansprechpartner
* Werkzeuge

## Anhang
* Glossar
* Referenzen