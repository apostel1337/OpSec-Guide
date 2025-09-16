| Security STAGE 1
#######################################################################################

Mit wenigen Klicks surfen wir anonym über Tor im Netz – ganz gleich, ob unter Windows, Linux oder OS X. Der Tor-Browser ist die einfachste und schnellste Lösung anonym ins Internet zu kommen.
Der Einstieg in das Anonymisierungs-Netzwerk Tor ist schnell geschafft und nicht komplizierter als eine Firefox-Installation. Das kostenlose Tor-Browser-Bundle bringt alles mit, was wir brauchen: den Tor-Client, der eine Verbindung zum Netzwerk herstellt sowie eine vollständig vorkonfigurierte Firefox-Version namens Tor Browser. Damit wir auch tatsächlich anonym surfen und nicht an eine manipulierte Version des Bundles geraten, sollten man nur direkt beim Tor Project herunterladen.
Der Tor-Browser ist für Gelegenheits-User gut geeignet und auch völlig ausreichend.


#######################################################################################
#  Tails auf USB-Stick | Security STAGE 2
#######################################################################################

Tails ist ein Live-Betriebssystem, das darauf ausgerichtet ist unsere Privatsphäre und Anonymität zu bewahren. Es hilft uns dabei, das Internet so gut wie überall und von jedem Computer aus anonym zu nutzen, ohne dabei Spuren zu hinterlassen, sofern wir dies nicht ausdrücklich wünschen.

Tails beinhaltet verschiedene Programme, die im Hinblick auf die Sicherheit vorkonfiguriert wurden: einen Webbrowser, einen Instant-Messaging-Client, ein E-Mail-Programm, ein Office-Paket, einen Bild- und Audioeditor usw.

### Tails USB-Stick erstellen

Die Installation von Tails lässt sich auch als Laie im IT-Bereich bewerkstelligen. Sie können Tails über Windows, Mac Os X, DEBIAN/UBUNTU oder LINUX (Red Hat, FEDORA,...) installieren. Natürlich handeln sie eigenverantwortlich.

Für die Installation benötigen wir folgendes:

- Einen Computer mit Internetzugang
- Zwei USB-Sticks mit mindestens 4GB Speicher
- Einen weiteren Computer, Smartphone oder Drucker, für die weiteren Schritte der Installation
- Ca. zwei Stunden Zeit
Zwei USB-Sticks sind nötig, weil man zunächst eine Vorab-Version von Tails auf dem einem Stick installieren muss und erst im nächsten Schritt über diesen ersten Stick die finale Version von Tails auf den zweiten Stick installiert.
Eine sehr ausführliche Installationsanleitung finden sie auf der unten verlinkten Herstellerwebseite. Ich gebe an dieser Stelle nur einen kurzen Überblick über den Installationsvorgang.

# Download von Tails
Als erstes muss die Installationsdatei von der Herstellerwebseite geladen werden. Achte darauf, dass es sich auch wirklich um die originale Webseite handelt.
→ https://tails.boum.org/index.de.html

Nach ein paar Angaben über ihr verwendetes Betriebssystem und die bevorzugte Installationsweise (du kannst Tails auch von einer bereits bestehenden Tails-Installation aus installieren), starte den Download der Installationsdatei. Dabei kann es notwendig sein, im Vorfeld ein Firefox-Plugin zu installieren, das den Download der Tails-ISO verifiziert.

# Tails auf dem USB-Stick installieren

Im nächsten Schritt müssen wir ein Programm (Universal USB Installer) laden, das es erlaubt, die eben geladene Tails-ISO auf dem ersten USB-Stick zu installieren. Diesen Stick können wir jetzt schon mit dem Computer verbinden.

Nach dem Download des USB-Installers starten wir diesen durch einen Doppelklick. Eventuell wirst du von deinem Betriebssystem noch nach einer Bestätigung gefragt, ob du dieses Programm wirklich starten willst. Bestätige dies und lese im Anschluss die Lizenzvereinbarung des USB-Installers durch und bestätige diese.

Nun müssen wir in einem Dropdown-Menü die Linux-Destribution Tails auswählen (ist ziemlich weit unten im Menü), als Quelle das zuvor geladene ISO-Image und als Ziel den ersten USB-Stick. Außerdem müssen wir bei „Format“ ein Häkchen setzen, durch das wir bestätigen, dass der USB-Stick formatiert werden darf (ACHTUNG! Alle Daten auf dem Stick werden dabei gelöscht.)

Nun müssen wir nur noch die Installation von Tails bestätigen und im Anschluss den Universal USB-Installer schließen. Auf dem ersten USB-Stick befindet sich jetzt die Vorab-Version von Tails.
Jetzt müssen wir den Computer über den USB-Stick neu starten. Im Vorfeld sollten sie diese Webseite auf einem anderen Gerät (Computer, Tablet, Handy,...) aufrufen, bzw. die weiteren Schritte der Installation ausdrucken oder notieren.

Je nach Hersteller des Computers kann es nötig sein, den Computer in einem anderen Modus (Boot-Menu) zu starten, über den man dem Computer vorgeben muss, über den USB-Stick zu starten. Wenn wir die Tastenkombination dafür nicht kennen, können wir versuchen folgende Tasten während des Startvorgangs zu betätigen: Esc, F12, F10, F9, F8 oder F2. Bei meinem PC sind es zum Beispiel Del oder F2. Damit kommt man in das Boot-Menu und zur Möglichkeit, über den USB-Stick zu starten. Daneben lässt sich die Reihenfolge von den zu bootenden Laufwerken verändern und speichern. Man kann z.B. USB → HDD → CD einstellen, wenn immer als erstes versucht werden soll, über den Stick zu starten, falls ein USB-Stick am Computer angeschlossen ist. Ist keiner angeschlossen, so startet das System über die Festplatte.

Wenn sie es geschafft haben, das System über den USB-Stick zu starten, erscheint ein kleines Auswahlfenster. Hier bestätigen sie mit der Return-Taste den ersten Punkt (Live). Im Anschluss wählen sie noch die bevorzugte Sprache aus. Wir haben nun die Vorabversion von Tails erfolgreich installiert.

# Tails auf zweitem USB-Stick installieren

Im Anschluss müssen wir die endgültige Version von Tails auf dem zweiten USB-Stick installieren. Dazu schließen wir den zweiten Stick am Computer an, gehen in Tails auf Anwendungen → Tails → Tails Installer und wählen Install by Cloning aus.

Wähle den zweiten USB-Stick als Target Device und klicke auf Install Tails, um die Installation auf dem zweiten Stick zu starten. Es folgt eine Warnmeldung, dass alle Daten auf dem zweiten Stick gelöscht werden. Bestätige diese, wenn wir damit einverstanden sind. Die endgültige Version von Tails wird jetzt auf dem zweiten USB-Stick installiert.

Nach der erfolgreichen Installation können wir den Computer runter fahren und den ersten Stick entfernen. Starte nun den Computer von dem zweiten USB-Stick, so wie wir es bereits erfolgreich mit dem ersten Stick gemacht haben.

# Tails auf USB-Stick oder Speicherkarte oder sogar DVD?

Wer Tails auf einem USB-Stick oder einer Speicherkarte nutzt, hat den Vorteil, dass Daten direkt auf dem Datenträger (Stick oder Karte) gespeichert werden können. Dafür hat es den Nachteil, dass das System über Schadsoftware geändert werden kann. Wer ein absolut sicheres System wünscht, sollte Tails auf einer DVD installieren. Dadurch wird erreicht, dass das System nicht mehr geändert werden kann. Wer Daten über Tails speichern möchte, kann immer noch einen Datenträger über das System auswählen, und die Daten darauf speichern, was aber doch sehr umständlich sein kann.

Wir können die Benutzeroberfläche von Tails so einstellen, dass sie der von Windows XP ähnelt. Dazu müssen wir in Tails unter „System → Einstellungen → Erscheinungsbild“ die Windows XP Benutzeroberfläche auswählen und bestätigen. Das machst die Nutzung für viele User einfacher.


#######################################################################################
#  Hochsicheres Whonix System | Security STAGE 3
#######################################################################################

Whonix ist eine Debian-basierende Linux-Distribution, die auf Privatsphäre, Sicherheit und Anonymität im Internet Wert legt. Um dies zu erreichen, setzt Whonix insbesondere auf die Nutzung des Tor-Netzwerks.

Das Betriebssystem besteht aus zwei virtuellen Maschinen, einer Workstation und einem Gateway für das Tor-Netzwerk. Jegliche Netzwerkkommunikation wird durch das Tor-Netzwerk geleitet. Updates werden via Tor mit dem Debian apt-get-Paketmanager eingespielt. VirtualBox, Qubes OS und KVM werden als Virtualisierungssoftware unterstützt. Die Desktop-Umgebung ist KDE. Installer werden für Windows, Linux, macOS und Qubes OS angeboten.

Wir richten zusammen das Whonix Grundsystem ein, so dass wir zukünftig von Anfang anonym online unterwegs sind. Dazu nutzen wir einerseits die kostenlose Software VirtualBox. Andererseits aber auch das kostenlose Betriebssystem Whonix sowie ein VPN.


### Benötigte Software

Hier die Software in einer Liste, die du benötigst, um garantiert anonym surfen zu können:
- VirtualBox: Die kostenlose Virtualisierungssoftware ist ungemein leistungsstark und für nahezu jedes Betriebssystem erhältlich. Lade die aktuellste Version hier herunter und installiere VirtualBox anschließend.

- Whonix: Ein Linux-Derivat, das extra dafür geschaffen ist, um anonym surfen zu können. Grundsätzlich besteht Whonix aus zwei Komponenten. Wir benötigen allerdings lediglich das sogenannte „Gateway“. Lade das Image für VirtualBox herunter.

Du benötigst außerdem ein beliebiges weiteres Betriebssystem das Disk-Image. Im Idealfall sollte es eine ISO von Windows 7 oder höher sein. Windows wird nach wie vor von den meisten Anwendern genutzt und gilt als recht einfach zu bedienen. Es hat zwar gewisse Schwächen. Allerdings verfügt es auch über die höchste Kompatibilität. So oder so lässt sich damit vor allem das Grundsystem besonders einfach einrichten.


### Installation

Bevor man Whonix benutzt ist es sinnvoll zu verstehen wie Whonix überhaupt funktioniert. Whonix besteht aus zwei Teilen. Der erste Teil ist das Gateway welches ein TOR-Relay zur Verfügung stellt. Der zweite Teil ist die Workstation, also die Maschine auf der wir später arbeiten können.

Beide Teile laufen nur als VM (Virtuelle Maschine) auf einem Host. Der Host kann sowohl Windows, Linux oder ein OSX sein. Um VM laufen lassen zu können benötigt der Host das Programm "Virtual Box".

-> https://www.virtualbox.org/wiki/Downloads

Dazu laden wir uns noch die beiden Whonix VMs runter. Je nachdem welches Host-System ihr habt, beide VMs downloaden. Sowohl das Gateway als auch die Workstation.

-> https://www.whonix.org/wiki/Download

Nachdem ihr Virtual Box installiert habt könnt ihr die beiden Whonix VMs importieren. Virtual Box öffnen und folgendes tun:

- Klick File > Import Appliance…
- Klick “Choose” und wähle die Whonix-Gateway.ova File.
- Klick next und dann “Import” ohne Einstellungen zu ändern.
- Warten bis der Import komplett ist.
- Diese Schritte für die Whonix-Workstation.ova File wiederholen.
- Jetzt kann man Whonix-Gateway und Whonix-Workstation starten.

Der default Username ist: user
Der default Passwort ist: changeme

Beim ersten Start müsst ihr durch einen kurzen Setup-Prozess der aber selbstklärend und einfach ist. Danach sollte Whonix nach Updates suchen und diese ggf. installieren.

Passwörter sollten nach der Installation geändert werden. Ganz einfach ein Terminal öffnen und folgendes eingeben. "passwd user", dann ein neues Passwort vergeben.

Gearbeitet wird NUR in der Whonix Workstation. Das Gateway MUSS immer laufen da die Workstation sonst keine Verbindung zum TOR-Netzwerk aufbauen kann.


#######################################################################################