# imcm-mitschrift
 
Das ist die README.md-Datei. med steht für Markdown. Markdown ist eine im Internet weit verbreitete Auszeichnungssprache (*Markup-Language*)
 
- HTML (Hypertext Markup Language)
- XML (Extensible Markup Language)
- YAML, YML (Yet Another Markup Language)
 
## Playlist zur Funktionsweise des Internets
 
### Teil 1 - What is the Internet?
 
- wurde in den 1970er-Jahren erfunden
- Motivation: schaffung eines dezentralen Netzwerks das auch noch nach einem Atomschlag noch funktioniert (Kontext des Kalten Krieges)
- Funktionsweise: Paketvermittlung (*Packet Switching*) - jedes Datenpaket sucht sich eine eigene Route durch das Netzwerk
- Internet: das Netz der Netze - besteht aus vielen kleinen Netzen unterschiedlicher Internetanbietern (*Internet Service Provider - ISP*, z.B.: A1, Magenta, Salzburg AG, ...)
 
### Teil 2 - The Internet: Wires, Cables & Wifi
 
- Informationen werden im Internet als Bits übertrage.
- Bits haben zwei Werte: 0 oder 1.
- 8 Bits ergeben 1 Byte. Mit einem Byte kann man 256 verschiedene Werte speichern (2^8).
 
- Bits können über verschiedene Übertragungsmedien zwischen Computern versendt werden.
- Die Anzahl der Übertragenen Bits pro Sekunde wird als Bandbreite bezeichnet - z.b.: 300MBit/s -> 300 Millionen Bit können pro Sekunde über diese Leitung laufen.
- Die zwei Hauptübertrager sind :
 
1. Kupfer / Elektrizität
    - billig
    - einfache Verarbeitung
    - weit verbreitet
    - hohe Verluste über lange Distanzen (hunderte Meter)
 
 
2. Glasfaser / Licht
    - teuer
    - schwierige Verarbeitung
    - schnelle Übertragung
    - verlustfrei
    - geeignet für Ozeankabel
 
3. Funk / Radiowellen
    - hoher Komfort, Internet überall
    - hohe Verluste über Distanzen
 
### Teil 3 - The Internet: IP-Adressen ß DNS
 
    - protokolle sind die Regel der Kommunikation
    - eines der wichtigsten Protokolle im Internet ist das Internet Protocoll (IP)
    - jedes Gerät im Internet hat zumindest eine (eindeutige) IP-Adresse, viele Geräte haben aber eine externe IP (ähnlich wie die      Raumnummer)
    - das Domain name system (DNS) übersetzt menschenlesbare Domainnamen (z.B.: www.google.com) in IP Adressen
    - DNS server führen Tabellen mit Domainnamen und den entsprechenden IP-Adressen
 
### Teil 4 - The Internet: Packets, Routing and Reliability
 - Daten, die über das Internet versendet werden, werden in Pakete aufgeteilt
 - Pakete sind in der Regel rund 1500 Byte groß (= 1.5KB). das heißt, ein 10 MB großes Foto würde in etwa 6667 Pakete aufgeteilt werden (10MB = 10.000 KB = 10.000.000 Byte / 1500 Byte = 6667 Pakete)
 - Pakete können unterschiedliche Routen durch das Internet nehmen. Die Routenplanung erfolgt durch spezielle Computer-sogenannte Router. Router entscheiden,welchen Weg ein Paket durch das Internet nimmt. Die Entscheidung basiert auf verschiedenen Faktoren, wie z.B. der aktuellen Auslastung der Verbindung und der Entfernung zum Ziel.
 - jedes Paket enthält die Ip-Adresse über die Quelle und des Ziels sowie die Reihenfolge der Pakete (damit sie am Ziel wieder korrekt zusammengesetzt werden können)
 - am Ziel wird die Vollständigkeit der Pakete durch das *Transmission Control Protocol (TCP)* überprüft. Wenn Pakete verloren gehen, fordert TCP die erneute Übertragung an.
 - TCP und IP bilden gemeinsam die Basis für die Funktionsweise des Internets - man spricht auch vom TCP/IP-Modell.
 
 ### Teil 5 - The Internet: HTTP and HTML
 
 - das *Hypertext Transfer Protocol* (HTTP) ist das Protokoll, das für die Übertragung von Webseiten verwendet wird.
 - der Ablauf ist immer derselbe:
 1. der Web-Client (Browser) schickt eine HTTP - Anfrage (*Request*) an den Web-Server
2. der Web-Server übernimmt die Anfrage, bearbeitet sie und schickt eine HTTP - Antwort (*Response*) zurück an den Web-Client. Dabei versieht er die Antwort mit einem [HTTP-Statuscode](https://de.wikipedia.org/wiki/HTTP-Statuscode). Diese sind in verschiedene Klassen eingeteilt.
 
>[! NOTE]
> #### HTTP-Statuscodes-Klassen
>
> - **1xx** - die Anfrage dauert noch an
> - **2xx** - die Anfrage war erfolgreich
> - **3xx** - die Anfrage wurde umgeleitet
> - **4xx** - Clientfehler (z.B. 404 - Seite nicht gefunden)
> - **5xx** - Serverfehler (z.B. 500 - interner Serverfehler)
 
- Daten (Webseiten, Bilder, Videos, usw.) werden mittels GET-Anfragen angefordert
- User-Input (Texteingaben, Dateiuploads, ...) werden mittels POST-Anfragen verschlüsselt übermittelt
- Get- und Post-Anfragen sind sogenannte **HTTP-Methoden**. Es gibt noch weitere Methoden, die wir erst später lernen.
- HTTP-Anfragen und Antworten können auch **Cookies** enthalten. Das sind kleine Textdateien, die aus Schlüssel-Wert-Paaren (*key-value-pairs*) bestehen. Ist ein Cookie einmal gesetzt, wird es mit jeder Anfrage mitgesendet. So kann der Webserver einzelne User wiedererkennen bzw. identifizieren.
 
### Teil 8 - The Internet: How Search Works
 
- Suchcmaschinen-Bots (*Crawler*) durchstreifen ständig das WWW und katologisieren Websites. Der so enstehende Katalog wird auch **Index** genannt.
- wenn wir einen Suchbegriff  bei Google (oder einer anderen *Search Engine*) eingeben, wird nicht das WWW durchsucht, sondern lediglich der zuvor erstellte Index.
- Suchergebnisse werden auf Basis eines (geheimen)Algorithmus geranked - Ergenisse, die weiter oben stehen, werden öfter angeklickt
- Einfluss auf das Ranking haben u.a.:
  - im Text vorkommende Suchbegriffe (*Keywords*)
  - Links, die auf meine Seite zeigen (*Backlinks*)
- die Suchergebnisse werden an die Benutzer*innen angepasst! D.h. nicht jede/r sieht die gleichen Informationen, selbst wenn sie idente Suchanfragen durchführen!
- [Startpage](https://www.startpage.com/) ist eine datensparsame Suchmaschine, die ihren Benutzer*innen die Verwendung von Google ohne Tracking oder Personalisierung erlaubt.



