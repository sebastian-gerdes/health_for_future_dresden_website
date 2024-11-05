# Website for "Health for Future Dresden"
This is the github repository for the [quarto](https://quarto.org/)-based website of the Health for Future Group Dresden, a group belonging to the [Friday for Future](https://en.wikipedia.org/wiki/School_Strike_for_Climate) movement.

Currently, the website is still under construction.

The site is deployed via netlify [here](https://h4f-dresden.netlify.app/). The subdomain [(http://dresden.healthforfuture.de/](http://dresden.healthforfuture.de/) points to netlify.

Feel free to give feedback and contact me if you want to fork this site (should not be a problem).

## Zu klären:
* Plena auf Webseite ankündigen?
* Duzen / Siezen? Groß oder klein schreiben?
* Titel auf mobiler Seite
* E-Mail obfuscation
* Link zu Telegram-Kanal? Link zu Mailingliste von H4F-Deutschland?
* Evtl. noch Seite mit Terminen machen?
* Impressum klären
* Suchmaschinen brauchen immer etwas - bisher wird die Seite nicht gefunden
* Kontaktformular?
* ~~Instagram-Account geht nicht mehr~~

## Anleitung
### Installation
* Benötigte Software (evtl. kann RStudio quarto und git gleich mitinstallieren)
  - RStudio mit Paketen
  - quarto
  - git
* Github Zugang
* Githubzugang in RStudio einrichten
* Projekt erstellen

### Zu beachten
* Keine Zugangsnamen und Passwörter im Text speichen, da die Daten möglicherweise von außen gelesen werden können

### Beim Start 
* Falls jemand anderes in der Zwischenzeit etwas an der Webseite geändert hat diese Änderungen in die eigene lokale Kopie integrieren:  `git pull` auf der Konsole eingeben oder im entsprechenden Menü klicken

### Neuen Post erstellen
* Datei `code_snippets.qmd` öffnen
* `create_post(post_title = 'Das ist ein Test')` ausführen
* Datei mit Starttext wird automatisch geöffnet

### Seite editieren
* Seite für Datei öffnen
* Seite editieren, dabei nach Belieben Vorschau über die Schaltfläche 'Render' nutzen (oder auf `Render on Save` umstellen und dann speichern)
* Wenn Post fertig ist:
  * Registerreiter Git öffnen
  * Hochzuladende Dateien auswählen
  * Commit und Push
  
### Einbetten von Fotos
Geht so:

```{.default shortcodes="false"}
![](../images/banner.jpg){width='66%' fig-align='center'}
```

### Einbetten von Fotos über externen Anbieter
* Hochladen
* zum Beispiel über
  * [flickr](https://www.flickr.com/) - kein Beispiel
  * [albumizr](https://albumizr.com/) - Fotos hochladen und dann den angebotenen Text in die Datei einfügen. Beispiel:
  
```{.default shortcodes="false"}
<iframe loading="lazy" src="https://albumizr.com/a/nzJb" scrolling="no" frameborder="0" allowfullscreen width="100%" height="400"></iframe>
```
### Einbetten von Videos
* geht so:

``` {.default shortcodes="false"}
{{< video https://www.youtube.com/embed/wo9vZccmqwc >}}
```


## Angestrebtes Impressum
Dürfen wir ein Impressum wie z.B. [Freiburg](https://freiburg.healthforfuture.de/?page_id=214) machen? 

### Angaben gemäß § 5 Telemediengesetz
* Health for Future Dresden (freier Zusammenschluss von im Projekt Aktiven)
* Postalische Kontaktmöglichkeit: Sebastian Gerdes, Talstraße 7, 01099 Dresden
* Elektronische Kontaktmöglichkeit: dresden(at)healthforfuture(punkt)de

### Datenschutz
* Auf dieser Seite erfolgt kein Tracking und keine Werbung. Es werden keine Cookies gesetzt.
* Die Seite ist auf [Netlify](https://netlify.app/) gehosted. [Hier](https://www.netlify.com/privacy/) sind Informationen zum Datenschutz bei Netlify zu finden.



<details> 
<summary> 
Beispiele für Einzelpraxis/ große Gemeinschaftspraxis/ operative Tagesklinik 
<\summary>
Bei der unkompliziert möglichen Umstellung vom günstigsten Strom bei z.B. dem dresdner Grundversorger, der DREWAG, auf Ökostrom beim gleichen Anbieter sind das bei einer kleinen Hausarztpraxis mit einem Verbrauch von 1900 kWh/Jahr nicht einmal fünf Euro Mehrkosten. Für eine große Praxis mit 20 Mitarbeitern und 100 Praxisstunden/Woche (9325 kWh/Jahr)wären es Mehrkosten von 23 Euro und eine Praxis mit angeschlossener Tagesklinik (ca. 17000 kWh/Jahr) würde jährlich 40 Euro mehr zahlen bei Wechsel auf Strom aus erneuerbaren Energien.
Übrigens gehören die örtlichen Grundversorger oft zu den teuersten Stromanbietern. Laut einem Vergleich des Bundeswirtschaftsministeriums lag der durchschnittliche Strompreis 2018 in der Grundversorgung bei 31,47 Cent pro kWh. Der Preis aller von der Vergleichsplattform EcoTopTen empfohlenen und mit Grüner-Strom- oder ok-Power-Label zertifizierten Ökostrom-Tarife liegt unter diesem Preis – allerdings ohne Berücksichtigung monatlicher Grundgebühren. Somit könnte man bei einem Wechsel sogar Geld sparen!
<\details>