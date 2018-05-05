#nlshPhpStandard#

----------

Mal schnell ein paar Zeilen Code zu schreiben ist einfach.

Diesen aber später noch flüssig lesen können und verstehen ist wesentlich schwieriger.

Darum sollte man sich einen Standard schaffen und **immer** danach programmieren!

Aus diesem Grund nutze ich den [PHP CodeSniffer](http://pear.php.net/package/PHP_CodeSniffer/download "PHP CodeSniffler").

Um überhaupt in PHP programmieren zu können, benötigt man natürlich eine PHP- Umgebung. Ich persönlich benutze unter einem Windows- Betriebssystem [xampp](https://www.apachefriends.org/de/index.html "xampp"). Dies ist selbst für einen Anfänger schnell und ohne Grundkenntnisse installierbar.

Also, erstens [xampp](https://www.apachefriends.org/de/index.html "xampp") installieren!

Danach benötigt man natürlich den [PHP CodeSniffler](http://pear.php.net/package/PHP_CodeSniffer/download "PHP CodeSniffler").

Diesen bitte in der aktuell angebotenen Version mit der unter **Easy Install** angegebenen Zeile in der Eingabeaufforderung (Startbutton-> Alle Programme -> Zubehör -> Eingabeaufforderung, oder einfach Eingabe **CMD** im Suchrequester) installieren.

**Bitte die angezeigten PEARL- Warnungen oder Hinweise nicht ignorieren, sondern Folge leisten!**

Danach befinden sich im Verzeichnis  `C:\xampp\php\pear\PHP\CodeSniffer\src\Standards` ( in der Version 2.x im Verzeichnis `C:\xampp\php\pear\PHP\CodeSniffer\Standards`) die einzelnen Definitionen für Standards, vorgelistet nach bestehenden Standards.

Um Euren eigenen definierten Standard nutzen zu können legt im o.g. Verzeichnis einen Ordner mit dem Namen Eures Standards an und erstellt dort einen Ordner Namens **Sniffs**. In diesem Ordner kommen dann Eure selbstgebastelten oder angepassten Sniffs. Außerdem müsst Ihr im Wurzelverzeichnis Eures Standards- Verzeichnisses eine Datei Namens `ruleset.xml` anlegen.

Mit `phpcs -i` könnt Ihr Euch die installierten Konfiguration ansehen.

Mit `phpcs --standard=NameEuresStandards (eventuellPfadvomCmsFensterZurDatei/)zuTestendePhpDatei` könnt Ihr loslegen.

Viel Spaß

Nils



