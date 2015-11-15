# BdP Newsletter Template für MailChimp

version: 1.0.1

## Voraussetzungen
Es wird ein MailChimp Account benötigt. Dieser kann auf [mailchimp.com](//mailchimp.com/) kostenfrei angelegt werden.

## Installation
1. Lade die aktuelle Version des Templates unter [Github Releases](https://github.com/pfadfinden/newsletter/releases) als `.zip` Datei herunter.
2. Erstelle in MailChimp unter Template > Create Template ein neues Template. Importiere den HTML Code aus der Datei /mailchimp/newsletter_buena_mailchimp.html (Paste in code).
3. Ersetze Stamm ????? im Header und 2x im Footer durch deinen Stamm oder Landesverband.
4. Ersetze den automatischen Insert-Tag \*|LIST:ADDRESS|\* durch die postalische Adresse in der Form: Strasse Hausnummer, PLZ Ort, DE
5. Speichere das Template. Nun kann es unter Campaigns > Create Campaign genutzt werden.

## Update
Das Update des Extension erfolgt durch überschreiben des HTML-Codes der Datei /mailchimp/newsletter_buena_mailchimp.html (Paste in code) aus dem aktuellen Release (https://github.com/pfadfinden/newsletter/releases)

## Hinweise zur Benutzung von Mailchimp

### Spambekämpfung
Der Großteil des weltweiten E-Mail Aufkommens ist Spam. Um den Spam zu verringeren wird versucht, diesen schon zu blockieren, bevor die Mails vom Mailserver angenommen werden. Deshalb wird überprüft, ob der Mailserver, der die E-Mails verschickt, diese auch verschicken darf. Mailchimp versendet die Newsletter von den Mailchimp-Servern und nicht von dem zu eurer Domain gehörigen Server. Mittels SPF und DKIM erteilt ihr den Mailchimp-Servern die Berechtigung Mails für eure Domain zu versenden.

Damit eure Newsletter nicht im Spamordner landen solltet ihr folgende zwei Einstellungen bei eurer Domain erstellen. Dazu müsst ihr zwei Einträge bei eurem DNS-Provider hinzufügen.

##### TXT(SPF) Record

    v=spf1 a mx include:servers.mcsv.net ~all


##### DKIM (CNAME Eintrag)

Ersetze example.com durch eure Domain.

    k1._domainkey.example.com CNAME dkim.mcsv.net

Nach ca. 24 Stunden sollten diese DNS-Änderungen im ganzen Internet verfügbar sein. Danach sollet ihr nur noch eure Domain in [Mailchimp authentifiziren](http://kb.mailchimp.com/delivery/deliverability-research/set-up-mailchimp-authentication).


