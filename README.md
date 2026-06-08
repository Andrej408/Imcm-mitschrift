# Imcm mitschrift

Das ist die READMe.md-datei. md steht für Markdown.
Markdown ist eine Internet weit verbreitete Auszeichnungsprache (*Markup-Language*).
Andere bekannte Auszeichnungssprachen sind:

- hypertext Markup Language (HTML)
- extensible Markup Language (XML)
- yet Another markup Language (YAML, YML)

## Playlist zur Funktionsweise des Internets

### Teil 1- what is the Internet?

- wurde in den 1970er - Jahren erfunden
- Motivation: Schaffung eines dezentralen Netzwerks, das auch nach einem Atomschlag noch funktioniert (Kontext des Kalten krieges)
- Funktionsweise: Paketvermittlung (*Packet Switching*) - jedes Datenpaket sucht sich eine eigene route durch das Netzwerk
- Internet: das Netz der Netze besteht aus vielen kleinen Netzen unterschiedlicher Internetanbieter (*Internet Service Provider -  ISP*, z.B. A1, Magenta, Salzburg AG, ...)

### Teil 2 - The Internet : Wires, Cables & Wifi

informationen werden im Interent als Bits Übertragen.
Bits haben zwei Werte : 0 oder 1.  8 Bits ergeben 1 Byte . Mit einem Byte kann man 256 verschiedene Werte speichern (2^8 = 2*2*2*2*2*2*2*2).

Bits können über verschiedene Übertragungsmedien zwischen Computern versendet werden.
 Die Anzahl der übertragenen Bits pro Sekunde wird als Bandbreite bezeichnet - z.B.: 300Mbit/s -> 300 Millionen Bit können pro Sekunde über diese Leitung laufen.
Übertragungsmedien können sein:

1. Kupfer / Elektrizität
 -  billig 
 - einfach in der Bearbeitung
 - weit verbreitet 
 - hohe Verluste über lange Distanzen (hunderte Meter)

2. Glasfaser / Licht
- schnelle Übertragung 
- verlustfrei
- geeignet für Ozeankabel
- teuer und schwierig in der Verarbeitung

3. Funk / Radiowellen
- hoher Komfort, Internet überall
- hohe Verluste über Distanzen
  
  
  ### Teil 3 - The Internet: IP-Addresses & DNS

  - Protokolle sind die Regeln der Kommunikation
  - eines der wichtigsten Protokolle im Internet ist das Internet protocol (IP) 
  - jedes Gerät im Internet hat zumindest eine (eindeutige) IP-Adresse, viele Geräte haben aber eine externe IP ( ähnlich wie die Hausnummer ) und eine Interne IP ( ähnlich wie die Raumnummer )
  - das Domain Name System (DNS) übersetzt menschenlesbare Domainnamen (z.B.: www.google.com) in IP-Adressen
  - DNS-Server führen Tabellen mit Domainnamen und den entsprechenden IP-Adressen


  ### Teil 4 - the Internet: Packets, Routing and Reliability

  - Daten die über da Internet versendet werden , werden in Packete aufgestellt
  - Pakete sind in der Regel rund 1500 Byte groß (=1.5 KB). Das heißt ein 10MB großes Foto wurde in etwa 6667 Pakete aufgeteillt werden ( = 10 000KB = 10 000 000 Byte / 1500 Byte = 6667 Pakete )
  - Pakete können unterschiedliche Routen durch das Internet nehmen. Die Routenplanung erfolgt durch spezielle Computer - sogennante Router .Router  entscheiden welchen Weg ein Paket durch das Internet nimmt. Die entscheidung basiert auf verschiedenen Faktoren, wie z.B. der aktuellen Auslastung der Verbindungen und der Entfernung zum Ziel.
  - jedes paket enthält die IP-Adressen der Quelle und des Ziels sowie die Reihenfolge der Pakete ( damit sie am Ziel wieder korrekt zusammengesetzt werden können ) 
  - am Ziel wird die vollständigkeit der Pakete durch das *Tarnsmission Control Protocol* (TCP) überprüft. Wenn Pakete beschädigt oder verloren gehen, 
  - TCP und IP bilden gemeinsam die Basis für die Funktionsweise des Internets - man spricht auch vom TCP/IP Modell

 ### Teil 5 - The Internet: HTTP und HTML


 - das *Hypertext Transfer protocol* ( HTTP) ist das Protocol, das für die Übertragung von Webseiten verwendet wird 
 - der Ablauf ist immer derselbe: 
 1. der Web-Client (Browser) schickt eine HTTP-Anfrage (*Request*) an den web-Server 
 2. der Web-Server übernimmt die Anfrage, bearbeitet sie und schickt eine HTTP-Antwort (*response*) zurück an den Web-Client. Dabei versieht er die Antwort mit einem [HTTP-Statuscode](https://de.wikepedia.org/wiki/HTTP-Statuscode). Diese sind in verschiedene Klassen eingestellt

 
 > #### HTTP-Statuscode-Klassen
 >
 > - **1xx** - die Anfrage dauert noch an 
 > - **2xx** - die Anfrage war erfolgreich 
 > - **3xx** - weiter oder Umleitung 
 > - **4xx** - Clientfehler (z.B. 404 - Not Found)
 > - **5xx** - Serverfehler
 - Daten ( Websiten, Bilder, Videos) werden mit der GET-Anfrage angefordert 
 -  User-Input ( Texteingaben, Dateinuploads, ...) werden mittels 
 POST-Anfragen verschlüsselt übermittelt
 - GET und POST sind sogennante **HTTP-Methoden**. Es gibt noch weitere Methoden, die wir erst später lernen. 
 - HTTP-Anfragen und Antworten könne auch **Cookies** enthalten. Das sind kleine Textdatein, die aus Schlüssel-Wert-Paaren
 (*key-volue-pairs*) bestehen. Ist ein Cookie einmal gesetzt, wird es mit jeder Anfrage mitgesendet. So kann der Webserver einzelne User wiederkennen bzw.Identifizieren.

### Teil 8 - The Internet: How Search Works

- Suchmaschienen Bots (*Crawler*) durchstreichen ständig das WWW und katalogisieren Websites . Der entstehende Katalog wird auch **Index** gennant.
- wenn wir einen Suchbegriff bei Google (oder einer anderen *Search Engine*)eingeben, wird Nicht das WWW durchsucht, sondern lediglich der zuvor erstellte Index
- Suchergebnisse werden auf basis eines (geheimen) Algorithmus geranked - Ergebnisse die weiter oben stehen, werden öfter angeklickt 
- Einfluss auf das Ranking haben u.a.:
   - im Text vorkommende Suchbegriffe (*Keywords*) 
   - Links, die auf meine Seite zeigen (*BackLinks*)
- die Suchergebnisse werden an die Benutzer angepasst D.H. , nicht jeder sieht die gleichen Informationen, selbst  wenn sie idente Suchanfragen durchführen.



 





















