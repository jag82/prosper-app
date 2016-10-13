1) Grunt nach Änderungen bzw. während Änderungen laufen lassen, dammit tenplates auch tatsächlich aktualisiert werden.

in /var/www/client als root /node_modules/grunt/bin/grunt ausführen


2) CSS am besten in styles/critical.css machen

Das ist zwar das minimal-CSS, was als allererstes geladen wird, aber dann müsst ihr euch ertsmal keine Gedanken darüber machen, was wo hingehört; 
alles, was hier drin landet, wird immer geladen.


3) API: API-Url wird in js/lib/ic-module.js festgelegt. Für InfoCompass sieht das so aus (Zeile 22):

icApiProvider.setBase('http://213.187.84.22:3000')


4) Pfade für API-Calls stehen in js/lib/ic-api.js

5) Texte werden über die Api bezogen (api-url.../locale), dort kommen auch die Übersetzungen her


