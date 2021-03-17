
# DNS Einstellungen
## _Hier wird beschrieben, welche DNS Einstellungen zu treffen sind!_


## Welche Optionen hast du?

- Du besitzt keine Domain:
    - Du kannst dir selbst eine kaufen. Zum Beispiel hier: Namecheap.com, OVH.com oder Cloudflare.com
    - Du wendest dich per Mail an mich. 
- Du besitzt eine Domain
    - Du wendest dich per Mail an mich, oder noch besser
    - Du folgst der folgenden Anleitung!

 <br><br>

***Du wirst hier immer die drei Beispiele (Namecheap.com, OVH.com, Cloudflare.com) sehen!***

## Schritt 1:
Als aller erstes meldest du dich bei der Website an, bei der du deine Domain gekauft hast und navigierst zu den DNS Einstellungen.

## Schritt 2:
Hier legst du nun die folgenden fünf Einträge ohne Anführungszeichen an:

 - Einträge des Typen "A":
   - "@" auf "91.134.179.202"
   - "*" auf "91.134.179.202"
   - "www" auf "91.134.179.202"
-Einträge des Typen "MX":
   - "@" auf "host.laukandt.de" mit der Priorität 10
   - "@" auf "mail.laukandt.de" mit der Priorität 20
	
	![Namecheap](webhost/example/images/nc-dns.png)