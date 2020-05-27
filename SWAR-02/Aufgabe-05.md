# Übung 05

## Metainformationen 
* Versionshistorie {kp}

| Wer          |    Was          |  Wo       |Warum       |  Wer |Wann |Version |
|--------------|-----------------|-----------|------------| -----|-----|--------| 
| Tom          |Was              |Da         |Nötig       |  Wer |Wann |Version |
| Til          |Was              |Hier       |Muss halt   |  Wer |Wann |Version |
| Timo         |Was              |Sonstwo    |War wichtig |  Wer |Wann |Version |
| Hans         |Was              |Nirgends   |Ist das so  |  Wer |Wann |Version |


* Newsletter
* Newsletter.dat
  
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
  * siehe andere Dokument
* Begründung für Architektur
  * MongoDB Atlas weil passend für die News im Newsletter und kundenverwaltung, flexibler
  * 

## Einflussfaktoren
* Technische Einflussfaktoren
  * siehe oben
* Organisatorische Einflussfaktoren
  * siehe oben

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
* ..

## Projektaspekte
* Ansprechpartner
* Werkzeuge

## Anhang
* Glossar
* Referenzen