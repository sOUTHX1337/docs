
# DNS Einstellungen
## _Hier wird beschrieben, welche DNS Einstellungen zu treffen sind!_


## Welche Optionen hast du?

- Du besitzt keine Domain:
    - Du kannst dir selbst eine kaufen. Zum Beispiel hier: [Namecheap.com][nc], [OVH.com][ovh] oder [Cloudflare.com][cf]
    - Du wendest dich per Mail an mich. 
- Du besitzt eine Domain
    - Du wendest dich per Mail an mich, oder noch besser
    - Du folgst der folgenden Anleitung!



## Schritt 1:
Als aller erstes meldest du dich bei der Website an, bei der du deine Domain gekauft hast und navigierst zu den DNS Einstellungen.

Anleitung für [Cloudflare][cf-dns]
Anleitung für [OVH][ovh-dns]
Anleitung für [Namecheap][nc-dns]

## Schritt 2:
Hier legst du nun die folgenden vier Einträge ohne Anführungszeichen an:

 - Einträge des Typen "A":
   - "@" auf "91.134.179.202"
   - "www" auf "91.134.179.202"
 - Einträge des Typen "MX":
   - "@" auf "mx1.go-reach.me" mit der Priorität 10
   - "@" auf "mx2.go-reach.me" mit der Priorität 20
 - Sonstige Einträge ("ovhdnstest.tk" durch eigene Domain ersetzen!):
   - _dmarc.ovhdnstest.tk.	1	IN	TXT	"v=DMARC1; p=none; rua=mailto:info@ovhdnstest.tk"
   - ovhdnstest.tk.	1	IN	TXT	"v=spf1 ip4:54.38.93.51 ip4:91.134.179.202 ip6:2001:41d0:403:1f33:: include:ovhdnstest.tk ~all"
	
[nc]: https://namecheap.com
[ovh]: https://ohv.com
[cf]: https://cloudflare.com
[cf-dns]: https://support.cloudflare.com/hc/de/articles/360019093151-Verwaltung-von-DNS-Eintr%C3%A4gen-in-Cloudflare
[ovh-dns]: https://docs.ovh.com/de/domains/webhosting_bearbeiten_der_dns_zone/
[nc-dns]: https://www.namecheap.com/support/knowledgebase/article.aspx/434/2237/how-do-i-set-up-host-records-for-a-domain/
