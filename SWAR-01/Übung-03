# Mockups entwerfen mit balsamiq 

* siehe UI-Benutzerschnittstelle dynamisch

# Wie kann eine SRS gegliedert sein?

* Einleitung
  * Projektbeschreibung / Zweck
  * Ziel
* Beschreibung des zu entwicklenden Systems
  * Nutzergruppen
  * Kernaufgaben
  * Teilaufgaben
  * Nutzungsanforderungen
  * Systemanforderungen
    * Kontextdiagramm
    * UI-Benutzerschnittstellen
      * Statisches Verhalten
      * Dynamisches Verhalten
    * Datenschnittstellen
    * Teschnische Schnittstellen
    * Laufzeitumgebung
    * Sonstige Anforderungen an das Produkt
      * Lizenzmangement
      * Update Upgrade
      * Gesetzliche Vorgaben

# Erstellen Sie eine komplette SRS.

## Einleitung

* Produktbeschreibung  
Das System soll die Möglichkeit bieten sich für einen bezahlten Newsletter zu registrieren und diesen Online abrufen zu könne. 
Mitarbeiter können Kundendaten abrufen daran Änderungen vornehmen und Kunden Nachrichten senden. Zudem können Mitarbeiter Newsletter erstellen,
 welche für die Abonnenten dann zur Verfügung stehen.
 
* Ziel  
Das Ziel dieses Dokumentes ist es die oben genannten Funktionen der Software detailliert
und widerspruchsfrei zu dokumentieren.

## Beschreibung des zu entwickelnden Systems

* Nutzergruppen (Stakeholder)  
Abonnenten (Kunden), Mitarbeiter und Interessierte

* Kernaufgabe  
s.o.
* Teilaufgabe  
s.o.
* Nutzungsanforderungen  
s.o.
* Systemanforderungen  
Kontextdiagram

![alt text](https://github.com/SoenkeSobott/SWAR/blob/master/SWAR-01/images/Kontextdiagram.png "Kontextdiagram")

### UI-Benutzerschnittstelle

* Statisches Aussehen
  * Mockups  
 siehe Mockups 

  * Style Guide

* Dynamisches Verhalten




### Datenschnitstelle

* Mail-Server  

| Typ             |    Werkzeug                                       |
|---------------- |------------------------------------               |
| Organisatorisch | Mail wird automatisiert nach neuer News versand   |
| Syntaktisch     | JSON                                              |
| Strukturell     | SMTP, POP3                                        |

Datenbank

| Typ             |    Werkzeug                                             |
|---------------- |------------------------------------                     |
| Organisatorisch | Verschiedene Rollen mit verschiedenen Berechtigunggen   |
| Syntaktisch     | JSON                                                    |
| Strukturell     | HTTPS                                                   |


### Technische Schnitstellen

* Performanz
  * Anzahl der Nutzer die simultan auf das System zugreifen 
  (Registrieren, Einloggen, News abrufen, Nachrichten verschicken)
  * Email bestätigung soll in unter 10 Sekunden beim Kunden ankommen

* Datensicherheit/Datenschutz
  * hashing
  * salting (CSPRNG)
  * Security by Design
  * Cookie/Tokens(API)

* System-System-Schnitstellen
  * LDAP
  
### Laufzeitumgebung

* Das System muss auf gängigen Browsern und Geräten lauffähig sein
* Das System ist Stabil und hat nur sehr geringe Ausfälle


### Sonstige Anforderungen
* Lizenzmanagement
  * Framework Lizenzen
  * Open Source
  
* Gesetzliche Vorgaben
  * Daten der Nutzer müssen vor Missbrauch Dritter geschützt sein
  * Der Nutzer kann sich vom Newsletter abmelden
  * Der Nutzer kann seine vom Unternehmen gespeicherten Daten anfordern
 
* Upgrade/Update
  * Das System ist leicht wartbar
  * Komponenten(z.B. DB) sind austauschbar
