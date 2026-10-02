# Fördjupning mot VG krav

## Moment A: Avancerad Nätverksanalys & Trafikflöden (Mål 3)

![Bild med datatrafikflöde](dataflow.png)

### Bild förklaring

Bilden förklarar hur datatrafiken åker när en dator (som är konfiguerad med Googles DNS server på 8.8.8.8) ska in på hemsida.<br>
Den visar hur käll- och destinations IP-adresser ändras när man kommer till ändpunkter och information ska skickas tillbaka.<br>
Den visar hur man använder olika (logiska) portar för att använda olika tjänster (53 för DNS, 80 för HTTP och 443 för HTTPS)

### Bilden visar inte MAC-adresser

Bilden visar däremot inte MAC-adresser. MAC-adresser är adresser till specifika nätverks-interfaces. En dator brukar bara ha en, men en router kan ha många.<br>
När man skickar information i ett nätverk så använder man destinations-MAC-adressen som next-hop address; den ändras för varje interface som den åker emellan, till skillnad til IP-adresser som alltid är samma tills informationen ska till ett annat håll.

### TCP/IP modellen

MAC-adresser ligger på Länk-lagret (eller Network Access-lagret) på TCP/IP modellen<br>
IP-adresser ligger på Internet-lagret på TCP/IP modellen<br>
Port nummer ligger på Transport-lagret på TCP/IP modellen<br>