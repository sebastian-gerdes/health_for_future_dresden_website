# Website for "Health for Future Dresden"
This is the github repository for the [quarto](https://quarto.org/)-based website of the Health for Future Group Dresden, a group belonging to the [Friday for Future](https://en.wikipedia.org/wiki/School_Strike_for_Climate) movement.

Currently, the website is still under construction.

The site is deployed via netlify [here](https://h4f-dresden.netlify.app/). Once it is fit for publication it will hopefully be published at the corresponding subdomain of Health for Future Germany ([Link](http://dresden.healthforfuture.de/)).

Feel free to give feedback and contact me if you want to fork this site (should not be a problem).


## Installation
* Benötigte Software (evtl. kann RStudio quarto und git gleich mitinstallieren)
  - RStudio mit Paketen
  - quarto
  - git
* Github Zugang
* Githubzugang in RStudio einrichten
* Projekt erstellen

## Zu beachten
* Keine Zugangsnamen und Passwörter im Text speichen, da die Daten möglicherweise von außen gelesen werden können

## Beim Start 
* Falls jemand anderes in der Zwischenzeit etwas an der Webseite geändert hat diese Änderungen in die eigene lokale Kopie integrieren:  `git pull` auf der Konsole eingeben oder im entsprechenden Menü klicken

## Neuen Post erstellen
* Datei `code_snippets.qmd` öffnen
* `create_post(post_title = 'Das ist ein Test')` ausführen
* Datei mit Starttext wird automatisch geöffnet

## Seite editieren
* Seite für Datei öffnen
* Seite editieren, dabei nach Belieben Vorschau über die Schaltfläche 'Render' nutzen (oder auf `Render on Save` umstellen und dann speichern)
* Wenn Post fertig ist:
  * Registerreiter Git öffnen
  * Hochzuladende Dateien auswählen
  * Commit und Push
  
## Einbetten von Fotos
Geht so:

```{.default shortcodes="false"}
![](../images/banner.jpg){width='66%' fig-align='center'}
```

Sieht dann so aus:

![](../images/banner.jpg){width='66%' fig-align='center'}

## Einbetten von Fotos über externen Anbieter
* Hochladen
* zum Beispiel über
  * [flickr](https://www.flickr.com/) - kein Beispiel
  * [albumizr](https://albumizr.com/) - Fotos hochladen und dann den angebotenen Text in die Datei einfügen. Beispiel:
  
```{.default shortcodes="false"}
<iframe loading="lazy" src="https://albumizr.com/a/nzJb" scrolling="no" frameborder="0" allowfullscreen width="100%" height="400"></iframe>
```
Das sieht dann so aus:
<iframe loading="lazy" src="https://albumizr.com/a/nzJb" scrolling="no" frameborder="0" allowfullscreen width="100%" height="400"></iframe>

## Einbetten von Videos
* geht so:

``` {.default shortcodes="false"}
{{< video https://www.youtube.com/embed/wo9vZccmqwc >}}
```
... und sieht dann so aus:
{{< video https://www.youtube.com/embed/wo9vZccmqwc >}}


