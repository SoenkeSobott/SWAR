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
  ![alt text](https://github.com/SoenkeSobott/SWAR/blob/master/SWAR-01/images/StyleGuide.png "StyleGuide")


* Dynamisches Verhalten

  * Nachricht senden
  
![alt text](https://github.com/SoenkeSobott/SWAR/blob/master/SWAR-01/images/NachrichtSenden.png "NachrichtSenden")


![alt text](https://github.com/SoenkeSobott/SWAR/blob/master/SWAR-01/images/Nachricht01.png "Nachricht01")

* 1 Der Nutzer wählt die Kundenliste aus

![alt text](https://github.com/SoenkeSobott/SWAR/blob/master/SWAR-01/images/Nachricht02.png "Nachricht02")

* 2 Der Nutzer sucht nach dem Kundennamen in der Suchleiste
* 3 Der Nutzer betätigt den Ändern Button

![alt text](https://github.com/SoenkeSobott/SWAR/blob/master/SWAR-01/images/Nachricht03.png "Nachricht03")

* 4 Der Nutzer verfasst eine Nachricht an den Kunden
* 5 Der Nutzer sendet die Nachricht ab

![alt text](https://github.com/SoenkeSobott/SWAR/blob/master/SWAR-01/images/Nachricht04.png "Nachricht04")

* 6 Der Nutzer bekommt eine Bestätigung das seine Nachricht versendet ist und 
klickt wider zur Home Seite


* Registrieren

![alt text](https://github.com/SoenkeSobott/SWAR/blob/master/SWAR-01/images/Registrierung01.png "Registrierung01")

* 1 Der Nutzer muss den Nutzungsbedingungen zustimmen
* 2 Der Nutzer muss den nächsten Schritt einleiten

![alt text](https://github.com/SoenkeSobott/SWAR/blob/master/SWAR-01/images/Registrierung02.png "Registrierung02")

* 3 Der Nutzer muss seine persönlichen Daten eingeben (Name, Mail, Passwort)
* 4 Der Nutzer wählt eine Zahlungsmethode
* 5 Der Nutzer meldet sich an

![alt text](https://github.com/SoenkeSobott/SWAR/blob/master/SWAR-01/images/Registrierung03.png "Registrierung03")

* 6 Der Nutzer sieht seine angegebenen Daten und kann diese ändern oder 
zur Home Seite navigieren




### Datenschnitstelle

* Mail-Server  

| Typ             |    Werkzeug                                       |
|---------------- |------------------------------------               |
| Organisatorisch | Mail wird automatisiert nach neuer News versendet |
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
