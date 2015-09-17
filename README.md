# BdP Newsletter Template für MailChimp

## Vorraussetzungen
Es wird ein MailChimp Account benötigt. Dieser kann auf www.mailchimp.com kostenfrei angelegt werden.

## Installation
1. Lade die aktuelle Version des Templates unter [Github Releases](https://github.com/pfadfinden/newsletter/releases) als `.zip` Datei herunter.
2. Erstelle in MailChimp unter Template > Create Template ein neues Template. Importiere entweder den HTML Code aus der Datei base_boxed_basic_2column_query.html (Paste in code) oder lade die zip-Datei direkt hoch (Import HTML).
3. Ersetze den automatischen Insert-Tag \*|LIST:COMPANY|\*  durch den Anzeigenamen, sodass dieser einzeilig dargestellt wird. (Preview benutzen!).
4. Ersetze den automatischen Insert-Tag \*|LIST:ADDRESS|\* durch die postalische Adresse in der Form Strasse Hausnummer, PLZ Ort, DE
5. Speichere das Template. Nun kann es unter Campaigns > Create Campaign genutzt werden.

## Update
Das Update des Extension erfolgt durch überschreiben des HTML-Codes der Datei base_boxed_basic_2column_query.html (Paste in code)aus dem aktuellen Release (https://github.com/pfadfinden/newsletter/releases)

## Bekannte Probleme
Hier werden Probleme bei der Darstellung des Newsletters aufgeführt, die systembedingt nicht gelöst werden können.

### Gmail Webclient
* Überschriften werden unter den Bildern statt auf den Bildern dargestellt.

### Gmail Android Client
* Überschriften werden unter den Bildern statt auf den Bildern dargestellt.

### Darstellung in Apple Mail

### Darstellung in Roundcube Web Mail

### Darstellung in Android K-9 Mail
* Hintergrundbilder werden im dunklen Theme nicht angezeigt.

### Darstellung in Outlook

### Darstellung in Thunderbird
* Elemente werden nach einem Fenster Resize versetzt angezeigt. Abhilfe: E-Mail Anzeige neuladen.

## Hinweise zur Benutzung von Mailchimp

## Fragen & Antworten
#### Warum werden einige Dateien über CDN Links geladen?
CDN steht für Content Delivery Network. Es handelt sich hierbei um einen Verbund von Servern, die speziell für die Auslieferung von statischen Dateien optimiert sind. Durch Einsatz des CDN und die Wiederverwendung der selben Resourcen durch Bund und Länder wird die Darstellung des Newsletters beschleunigt. Als Standard CDN wird cdn.pfadfinden.de verwendet.



