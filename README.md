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

Danach befinden sich im Verzeichnis  `C:\xampp\php\pear\PHP\CodeSniffer\Standards` die einzelnen Definitionen für Standards, vorgelistet nach bestehenden Standards.

Um Euren eigenen definierten Standard nutzen zu können legt im o.g. Verzeichnis einen Ordner mit dem Namen Eures Standards an und erstellt dort einen Ordner Namens **Sniffs**. In diesem Ordner kommen dann Eure selbstgebastelten oder angepassten Sniffs. Außerdem müsst Ihr im Wurzelverzeichnis Eures Standards- Verzeichnisses eine Datei Namens `ruleset.xml` anlegen.

Ich persönlich nutze die Standards von [TYPO3](https://typo3.org/ "TYPO3")

Holt euch dafür unter [https://github.com/typo3-ci/TYPO3SniffPool/releases/](https://github.com/typo3-ci/TYPO3SniffPool/releases/ "https://github.com/typo3-ci/TYPO3SniffPool/releases/") das Release 1.0.1 als .zip- Datei und kopiert daraus den Ordner **TYPO3SniffPool-x.x.x** in das o.g. Verzeichnis.
**Kürzt den Ordner- Namen um die Angabe der Versions- Nummer!**

Holt euch dann unter [https://github.com/typo3-ci/TYPO3CMS/releases](https://github.com/typo3-ci/TYPO3CMS/releases "https://github.com/typo3-ci/TYPO3CMS/releases") aus dem Release 6.2.1 die `ruleset.xml` und kopiert diese in Euer Wurzelverzeichnis Eures Standards. Dieses könnt Ihr jetzt nach Belieben anpassen und eigene Standards hinzufügen, bzw. angepasste Sniffs aufrufen.

Mit `phpcs --config-show` könnt Ihr Euch die Konfiguration ansehen.

Mit `phpcs --confic-set standard NameEuresStandards` könnt Ihr Euren Standard als vordefiniert bestimmen.

Habt Ihr Euren Standard vorkonfiguriert könnt Ihr mit `phpcs (eventuellPfadvomCmsFensterZurDatei/)zuTestendePhpDatei` loslegen.

Viel Spaß

Nils



