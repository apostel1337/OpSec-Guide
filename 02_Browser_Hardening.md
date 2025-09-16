#######################################################################################


### Clearnet vs Darknet

Die einen nur wollen sicher ihr Gras zum Eigenkonsum im Darknet bestellen, die anderen möchten unerkannt Waren und Dienstleistungen im Clearnet carden. Um dich richtig zu schützen solltest du vorher wissen was genau du vor hast. Im Darknet kannst du dich recht leicht mit TOR und ein paar anderen Tools gut schützen, im Clearnet sieht die Sache schon anders aus. Dort kann oft kein TOR verwendet werden da die Webseiten und Anbieter Verbindungen erkennen die von TOR-Exitnodes kommen und diese sofort blockieren.

DHL z.B. sperrt Packstationen meistens nach dem ersten Login von einem TOR-Node da hier automatisch von einem Missbrauch ausgegangen wird (was in 99% der Fälle auch so ist). Will man also im Clearnet arbeiten braucht man eine sichere Verbindung die aber zugleich nicht geblacklisted ist und auch anderweitig keine Aufmerksamkeit aufsich zieht bzw. nicht die Möglichkeiten einschränkt.

Du wirst also mit einem TOR-Browser keinen Erfolg beim Carding haben und mit nur einem sauberen VPN nicht ins Darknet kommen.


### Open Source vs Closed Source

Bei Freier Software wie Linux handelt es sich um Programme, deren Quelltext einsehbar ist und unter bestimmten Lizenzbedingungen verändert und weitergegeben werden darf. Dadurch entsteht die Möglichkeit, den Programmcode zu untersuchen und potentielle Hintertüren zu entdecken. Beim Gegenteil, der proprietären Software, wie z.B. Windows, ist der Quelltext nicht einsehbar, wird aber auf Anfrage von einigen Herstellern zur Verfügung gestellt. Man kann daher nicht 100% sicher sagen was diese Programme im Hintergrund machen. Eine platzierte Spionagesoftware kann daher leicht unerkannt bleiben.

Grundsätzlich ist keine Software vor Infiltrierung durch Dritte geschützt. Bei grossen Projekten wie zum Beispiel dem Linux-Kernel muss der Programmcode durch eine oder sogar mehrere Personen geprüft und freigegeben werden. Erst danach wird er dann veröffentlicht. Dieser Prozess des vorherigen Prüfens heißt Peer Review.

In der Vergangenheit kam es auch im Umfeld Freier Software zu größeren Sicherheitsproblemen, wie zum Beispiel der Heartbleed-Sicherheitslücke, die es Angreifern erlaubte, verschlüsselte HTTPS-Verbindungen abzuhören. Eine Verfügbarkeit des Quelltextes alleine garantiert somit also keine generelle Sicherheit, sie ist aber eine wichtige Voraussetzung, um die Sicherheit von Software zu erhöhen. Daher also das Fazit: Linux ist sicherer als Windows.

Beim Surfen im Internet hinterlässt man eine Vielzahl von Datenspuren, die von Dienst-Anbietern und Ermittlungsbehörden genutzt werden können. In erster Linie dienen sie zur Ermittlung von Vorlieben, um auf den Anwender zugeschnittene Werbung oder Suchergebnisse anzeigen zu können. Gerade bei der Online-Suche kann das schnell zu einer sogenannten Filter Bubble führen. Isst man beispielsweise gerne Asiatisch und hat in der Vergangenheit bei Google nach asiatischen Restaurants gesucht, besteht eine sehr hohe Wahrscheinlichkeit, dass man in Zukunft in erster Linie asiatische Varianten von Restaurants als Suchergebnis erhält.

Das mag zunächst harmlos klingen, in der Praxis kann das aber bedeuten das uns z.B. die DHL-Webseite anhand der vorher geöffneten Packstation Accounts wiedererkennt und unsere Aktivitäten eindeutig zuzuordnen sind. Oder GMX erkennt das wir heute schon 10 Mailadressen angelegt haben und kann diese Adressen miteinander in Verbindung bringen. Das wollen wir natürlich alles vermeiden.


### Tracker

Seit einigen Jahren gibt es die Möglichkeit, einem Webseiten-Betreiber mitzuteilen, dass man nicht verfolgt werden möchte. Im Firefox aktiviert man diese Einstellung, indem man in den „Settings“ unter dem Punkt „Privacy“ die Option „Tell sites that I dont want to be tracked“ wählt. Da es aber bisher weder in Europa noch in den USA einen verbindlichen rechtlichen Rahmen für die Funktion gibt, respektieren nur wenige Seitenbetreiber diese Einstellung.

Im Falle von Betrug gelten diese Richtlinien ohnehin nicht. Die Anti-Fraud-Systeme der einzelnen Webseiten sind sogar extra darauf ausgelegt möglichst viele und möglichst genaue Daten über uns zu sammeln. Auch die Polizei wird versuchen möglichst viele Informationen zu bekommen um uns zu identifizieren.

Tracker nutzen auf Webseiten eingebundene Elemente, um zu verfolgen, welche Webseiten besucht worden sind. Einen wirksamen Schutz gegen Tracker bietet das Addon Privacy Badger. Er verhindert die Datenübermittlung der Tracker und schaltet somit ihre Funktion aus. Diese Erweiterung wird von der Electronic Frottier Foundation (EFF) entwickelt. Die EFF setzt sich für Grundrechte im Informationszeitalter ein. Die Erweiterung benötigt nach der Installation keine besondere Konfiguration.


### Cookies

Grundsätzlich kann man sagen, dass Cookies weder schlecht noch gefährlich sind. Das sind kleine Dateien, die das Verhalten der Nutzer auf dem eigenen Computer speichern und mit bestimmten Websites interagieren. Sie dienen beispielsweise dazu, eine Sitzung aufrechtzuerhalten. Beim Aufruf einer Webseite kann ein „Cookie“ für die spätere Nutzung gesetzt werden. Beim nächsten Zugriff auf diese Webseite schickt der Browser automatisch den Cookie mit. Der Anbieter kann mit Hilfe des Cookies den Nutzer eindeutig zuordnen. Das wollen wir natürlich nicht, daher schalten wir diese Funktion ab.

Ein besonderer Fall sind Third Party Cookies. Dabei handelt es sich um reguläre Cookies, die aber nicht direkt zur aufgerufenen Webseite gehören. Es wird zum Beispiel ein Facebook-Like-Button in eine Webseite eingebunden. Der Button wird direkt von Facebook geladen und muss nicht angeklickt werden, um den Cookie zu setzen. Der Prozess passiert im Hintergrund.

Wenn man Third-Party-Cookies deaktiviert, werden keine Cookies mehr für Webseiten gesetzt, die nicht direkt aufgerufen worden sind. Die Option zum Deaktivieren von Third-Party-Cookies ist im Firefox etwas versteckt. In den „Privacy“-Einstellungen stellt man zunächst von „Firefox will Remember History“ auf „Use Custom Settings for History“ um. Danach kann man den Punkt „Accept third-party cookies“ auf „Never“ stellen. Firefox bietet ausserdem die Option, alle Cookies beim Beenden des Browsers zu löschen, was wir auch immer tun sollten.


### Adobe Flash

Der Adobe Flash Player hat keine besonders ruhmreiche Vergangenheit, was Sicherheit anbelangt. Der Flash-Player ist durch seine hohe Verbreitung umso verlockender für Angriffe auf die Privatsphäre. Daher sollte man grundsätzlich darauf verzichtet. Viele Dienstanbieter wie YouTube haben auf HTML5-Technologie zum Abspielen von Video- und Audiodateien umgestellt. Apple hat bereit schon 2010, noch unter Steve Jobs Führung, auf Flash in allen seinen Produkten verzichtet. Google hat den hauseigenen Flash-Player Peppermint im Mai 2015 testweise aus Chrome deaktiviert. Mit dem HTML5-basierten Flash-Player Shumway des Mozilla-Projektes ist es möglich, rudimentäre Flash-Inhalte ohne den Adobe Flash Player abspielen zu können. Im Normalfall braucht man Flash auf dem „Arbeitsrechner“ nicht.

Falls man trotzdem noch nicht auf den Adobe Flash Player verzichten kann, sollte man den lokalen Cache deaktivieren. Die Flash-Einstellungen kann man vornehmen, indem man mit der rechten Maustaste auf einen Flash-Inhalt klickt und „Global Settings“ wählt. Unter „Storage“ kann man dann „Block all sites from storing information on this computer“ wählen, um die Cachefunktion abzuschalten.


### NoScript

Das Firefox-Addon NoScript bietet die Möglichkeit, für jede Webseite einzustellen, ob aktive Elemente (sogenannte Skripte) ausgeführt werden sollen. Dabei wird der Ansatz verfolgt, dass standardmäßig alle Skripte verboten sind und pro Webseite freigeschaltet werden müssen. Das ist eine sehr hilfreiche Technik Tracking durch Java zu unterbinden.

Nach der Installation des Add-ons findet man ein entsprechendes Symbol neben der Adressleiste. Sollten auf einer Seite Skripts blockiert worden sein, öffnet sich zusätzlich eine Benachrichtigung im unteren Bereich des Browserfensters. Über einen Klick auf das Symbol öffnet sich eine Liste aller auf der gerade geöffneten Webseite eingebundener Skripte. Angegeben wird jeweils der Name der Webseite, von der versucht wird das Skripte zu beziehen. Besucht man zum Beispiel die Webseite der DHL, wird in der Liste nicht nur „dhl.de“ aufgeführt, sondern auch eine Vielzahl weiterer Webseiten wie zum Beispiel Google, von denen weitere Skripte bezogen werden. In den meisten Fällen kommen diese Skripte von Werbeanbietern oder Analyseseiten und werden zur Identifikation und zum Tracking genutzt.

Einige Darstellungs-Funktionen von Websites sind manchmal per Javascript umgesetzt – z.B Google Captures. Man sollte mit dem Plugin also aufmerksam umgehen. Sollte eine Webseite nicht mehr wie gewünscht dargestellt werden, kann man schrittweise Skripte von fremden Webseiten temporär zulassen, bis der Inhalt wieder korrekt dargestellt wird. Nachdem man so herausgefunden haben, welche Skripte freigeschaltet werden müssen, kann man diese permanent zulassen. Einstellungen bei NoScript gelten immer global. Es ist nicht möglich den Zugriff auf z. B. „googleapis.com“ für eine Webseite zuzulassen, für eine andere aber zu sperren.


### WebRTC

Mit WebRTC kann die lokale IP Adresse des Rechners im LAN und die öffentliche IP Adresse ermittelt werden, wie eine Demonstration von D. Roesler zeigt. Auch VPN-Verbindungen können damit ausgetrickst werden. Außerdem kann das Vorhandensein von Kamera und Mikrofon als Feature im Browser Fingerprint genutzt werden.

Mit dem Plugin Disable WerRTC kann die Übermittlung der Daten abgeschaltet werden.


### Fake User-Agent

Bei jedem Aufruf einer Webseite wird der Name und die Version des Browsers an den Webseitenbetreiber übermittelt, der sogenannte User-Agent-String. Die Informationen umfassen die Geräteart und -typ (PC, Tablet, Smartphone), die verwendete Bildschirmauflösung und das benutzte Betriebssystem sowie auch der auf dem System installierten Schriften, die zum Beispiel mit Hilfe von JavaScript ausgelesen werden können. Anhand dieser Daten kann ein Benutzer schon sehr genau identifiziert und zu mindestens 90% wiedererkannt werden.

Eine mögliche Gegenmaßnahme ist es, den User-Agent-String bei jedem Aufruf einer Webseite zu wechseln. Zu diesem Zweck eignet sich die Erweiterung Secret Agent. Nach der Installation desselbigen kann in den Einstellungen des Add-ons eine Liste der zu verwendenden User-Agent-Strings festgelegt werden. Die Standardliste enthält viele exotische Browser, was dazu führt, dass einige Webseiten nicht mehr korrekt dargestellt werden. Daher empfiehlt es sich, diese Liste zu bereinigen und nur moderne Browser-Varianten zu verwenden. Dazu öffnet man in den Plug-in-Einstellungen das Tab „User Agents“ und bearbeitet den Inhalt der Box „Stealth Mode“.

Der Stealth Mode kann daraufhin im Tab „Entropy“ über den Punkt „Enable Secret Agent’s Stealth Mode“ aktiviert werden. Hier lässt sich auch festlegen, in welchem zeitlichen Abstand der User-Agent-String rotiert werden soll. Alle weiteren Einstellungen des Add-ons können auf den Standardwerten belassen werden. Sollte es Probleme mit der Darstellung einer bestimmten Webseite geben, kann diese in der Host-Whitelist eintragen werden. Etwas störend wirkt die Secret Agent Toolbar. Sie kann bei Bedarf über „View -> Toolbars -> Secret Agent Toolbar“ ausgeblendet werden.


### Referrer

Beim Aufruf eines Links auf einer Webseite wird der Zielseite automatisch über einen sogenannten Referrer im HTTP-Header mitgeteilt, von welcher Seite die Anfrage kam. Hat man z. B. auf Google nach dem Wort „Packstation“ gesucht und klickt auf einen Treffer von DHL, dann bekommt DHL die Information, dass man zuvor auf Google war und dort nach dem Wort „Packstation“ gesucht hat.

Diese Funktion kann für Webseitenbetreiber sehr sinnvoll sein, um Webseiten strukturell besser aufzubauen. Denn damit kann auch ermittelt werden, wie Links am häufigsten aufgerufen werden. Auf der anderen Seite verraten Referrer, welche Suchworte eingegeben wurden, um auf eine Seite zu gelangen.

Da sich ein generelles Deaktivieren negativ auf den Surfkomfort auswirken kann, empfiehlt sich das Zulassen von Referrern innerhalb einer Seite und das Deaktivieren von Referrern beim Wechsel auf eine andere Seite. Leider bietet Firefox selbst diese Einstellmöglichkeit nicht an. Dazu eignet sich die Erweiterung RefControl.

Nach der Installation des Add-ons und dem Neustart des Browsers findet man im „Tools“-Menü einen Eintrag zur Konfiguration der RefControl-Optionen. Dort müssen keine einzelnen Seiten hinzugefügt werden. Stattdessen klickt man neben „Default for sites not listed“ auf „Edit“ und stellt dort „Block“ als Standardaktion ein. Durch das Setzen des Hakens bei „3rd Party requests only“ stellt man sicher, dass die Einstellung nur für den Aufruf neuer Seiten gilt.


### Modus des Browsers

Firefox sollte immer so eingestellt werden dass nach dem Schließen alle Daten über die aktuelle Session gelöscht werden. Unter Settings → Datenschutzeinstellungen können entsprechende Einstellungen gesetzt werden. Haken setzen bei „Die Chronik löschen, wenn Firefox geschlossen wird“ und Cookies nur behalten bis Firefox geschlossen wird. So werden nach dem Schließen immer alle Daten gelöscht und es baut sich keine History auf.


### Suchmaschine

Die Anbieter Google und Bing haben sich bei der Suche im Internet stark durchgesetzt. Damit wissen sie viel über die Vorlieben und das Surfverhalten eines Benutzers. Es gibt alternative Anbieter, die zusichern, keine personenbezogenen Daten zu speichern und weiter zu verarbeiten. Dazu gehören die Suchmaschine DuckDuckGo oder die Schweizer Metasuchmaschine eTools.ch.

StartPage ist eine Suchmaschine, die im Hintergrund auf Google zugreift. Sie ist vollständig lokalisierbar. Es kommt keine personalisierte Suche zum Einsatz, wodurch die Gefahr einer «Filter Bubble» verringert wird.


### HTTPS benutzen

Beim Zugriff auf Webseiten über HTTP werden alle Informationen unverschlüsselt übertragen und können leicht von Dritten analysiert werden. Besonders eine Übertragung von Passwörtern über HTTP ist sehr kritisch.
Um HTTPS für möglichst viele Seiten zu forcieren, bietet sich das Firefox-Add-on HTTPS everywhere der Electronic Frontier Foundation an. Nachdem dessen Installation erfolgt ist und der Browser neu gestartet wurde, findet man neben der Adressleiste ein neues Symbol, über das sich die Erweiterung steuern lässt. Ob die aktuelle Verbindung per HTTPS verschlüsselt ist, kann man anhand des Schlosssymbol in der Adressleiste erkennen.


### VPN

Beim Surfen im Internet kann ein Nutzer eindeutig einem Rechner und einer IP-Adresse zugeordnet werden. Falls möglich, empfiehlt sich immer die Nutzung eines offenen, anonymen WLAN-Zugangs (z. B. in einem Café).

Ein VPN ist dagegen Pflicht. Der VPN ändert deine IP und verschleiert somit deine reale IP-Adresse. Dazu kommt dass eine VPN-Verbindung immer ein verschlüsselter Tunnel ist, somit kann auch der Betreiber und alle Knotenpunkte über die deine Verbindung geht nichts mitlesen sondern sehen nur den verschlüsselten Tunnel. Bei der Nutzung von Tor ist ein VPN zu empfehlen um den Tor-Traffic im VPN-Tunnel zu verstecken. So wird eine Analyse von Online-Zeiten usw. unterbunden.

Traffic den man nicht sehen kann kann man auch nicht abhören. Also sollte bei einem VPN immer auf starke Verschlüsselung und sicheren Schlüsseltausch achten. Ist der VPN einmal sicher aufgebaut gibt es keine Möglichkeit den Traffic im inneren abzuhören oder zu manipulieren. Stellt der VPN-Client eine Manipulation am Tunnel fest wird der Tunnel abgebrochen und erneut eine sichere Verbindung aufgebaut.

Passende VPN Angebote findest du in unseren Listings.


### Tor-Netzwerk

Beim sogenannten Onion-Routing werden die Verbindungen über die einzelnen Tor-Knoten, die auf Rechnern in der ganzen Welt laufen, geleitet. Man kann Tor als Client nutzen oder auch selbst einen Knoten anbieten, über den dann andere Teilnehmer anonym surfen können. Die Verbindung zwischen den Knoten wird verschlüsselt. Die einzelnen Teilnehmer haben dabei keinen Einblick in die übermittelten Daten. Am Endpunkt, also am Übergang zum angefragten Zielserver, muss die Verbindung wieder entschlüsselt werden. Dieser Knoten hat Zugriff auf die übertragenen Daten. Es ist also auch hier sehr zu empfehlen, nur verschlüsselte Verbindungen aufzubauen.

Die einfachste Möglichkeit Tor zu nutzen, ist der vom Projekt bereitgestellte Tor-Browser. Dabei handelt es sich um eine modifizierte Firefox-Version, die alle für Tor notwendigen Komponenten bereits enthält.

Alternativ dazu kann man auch eine spezialisierte Linux-Distribution wie zum Beispiel Tails nutzen, die einfach auf einen USB-Stick gespielt und von dort aus gestartet und genutzt werden kann. Tails bietet ausserdem noch einen Windows-Tarnmodus an, in dem sich das System gegenüber Servern im Internet wie ein Windows-Rechner verhält.
Tails eignet sich sehr gut für den Einsatz auf fremden PCs, da es ein abgeschlossenes System ist, das auf dem damit gestarteten Rechner keinerlei Spuren hinterlässt.


#######################################################################################