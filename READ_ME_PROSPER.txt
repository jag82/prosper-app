1) Grunt nach Änderungen bzw. während Änderungen laufen lassen, damit templates auch tatsächlich aktualisiert werden.

in /var/www/client als root /node_modules/grunt/bin/grunt ausführen. (Läuft dann einfach nebenher und wartet auf Änderungen)


2) CSS am besten in styles/critical.css machen

Das ist zwar das minimal-CSS, was als allererstes geladen wird, aber dann müsst ihr euch ertsmal keine Gedanken darüber machen, was wo hingehört; 
alles, was hier drin landet, wird immer geladen.


3) API: API-Url wird in js/lib/ic-module.js festgelegt. Für InfoCompass sieht das so aus (Zeile 22):

icApiProvider.setBase('http://213.187.84.22:3000')


4) Pfade für API-Calls stehen in js/lib/ic-api.js

5) Texte werden über die Api bezogen (api-url.../locale), dort kommen auch die Übersetzungen her.

6) Farben und Icons stehen in styles/typography_and_colors.css

7) Die Homepage mit den Kacheln liegt in /pages/main.html. Beispielkacheln für Zielgruppen gibt es dort, allerdings: auskommentiert.


