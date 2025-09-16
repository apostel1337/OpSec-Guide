#######################################################################################

Warum überhaupt verschlüsseln? Klare Sache, falls doch mal die Polizei vor der Türe steht werden sie sicher euren Rechner, alle Speichermedien usw beschlagnahmen. Schlecht wenn dann alle eure Geschäfte, Accounts, Daten auf dem Rechner gespeichert sind. Wenn die Platte oder bzw. ein Container gut verschlüsselt ist und das Passwort nicht leicht erraten werden kann kommt nicht mal die CIA an eure Daten ran, versprochen. Zum Verschlüssen benutzen wir Veracrypt.

VeraCrypt ist der offizielle Nachfolger von TrueCrypt, d.h. wer sich schon mit TrueCrypt auskennt wird sich sehr schnell auch in VeraCrypt einarbeiten können. TrueCrypt wurde anhand Sicherheitsmängel eingestellt, VeraCrypt hat diese beseitigt und bietet das Programm kostenlos für Windows, Linux und auch Mac an.

Man kann folgendes damit verschlüsseln:

- Einzene Ordner (Containerdatei erstellen)
- Komplette Partitionen
- Das ganze System
- Versteckte Container in einer verschlüsselten Partition/Container

Was ist ein Container? Man kann sich das so vorstellen wir im realen Leben, das man einen Überseecontainer öffnet, Sachen dort hereinbringt und den Container danach abschließt. Jetzt kommt nur noch derjenige an die Sachen der den richtigen Schlüssel hat. Genauso ist das mit einem VeraCrypt Container. Es wird eine Datei erstellt die xxxMB groß ist, die man öffnen kann, Daten reinkopiert und dann wieder vom PC trennt. Jetzt sieht man nur eine xxxMB große Datei, kann aber nichts damit anfangen.

Ich empfehle nicht unbedingt komplette Partitionen auf externen Datenträgern zu verschlüsseln, denn wenn man diese an das Betriebssystem hängt kommt bei Windows z.B. direkt der Hinweis den Datenträger zu formatieren weil Windows mit dem Dateisystem nichts anfangen kann, ein falscher Klick und die Daten sind im Nirvana. Also lieber eine Containerdatei erstellen.

# Container erstellen

Als erstes starten wir VeraCrypt als Administrator. Das hat den Hintergrund weil ich bei TrueCrypt damals öfters mal Probleme bekam, vielleicht ist es mit VeraCrypt jetzt anders, aber das weiß ich nicht. Folgendes war damals passiert, ich startete TrueCrypt ganz normal, ließ einen 930GB Container erstellen, damit war der PC 8-12 Stunden beschäftigt, am Ende kam dann eine Fehlermeldung weil das Programm keine Administrator Rechte bekam, da war die Arbeit der ganzen Stunden dahin. Startete ich aber direkt als Administrator lief das Programm bis zum Ende ganz normal durch.

- Volumen und auf Neues Volumen erstellen
- Containerdatei erstellen auswählen
- Standard VeryCrypt Volume auswählen
- Speicherort für den Verschlüsselten Container angeben

Jetzt geht es darum den Verschlüsselungsalgorithmus auszuwählen. Hier solltet ihr IMMER eine Kombination wählen. AES - Blowfish z.B. Der Hash Algorithmuss sollte SHA-512 sein.

- Größe des Containers angeben

Jenachdem wieviel Daten ihr speichern wollt reicht oft schon ein kleiner Container mit 500Mb oder 1GB. Diesen könnt ihr dann z.b. einfach auf einen USB-Stick kopieren und eure Daten sicher und verschlüsselt mitnehmen. Der Container kann dann an jedem Rechner auf dem VeraCrypt installiert ist entschlüsselt und verwendet werden.

- Passwort für den Container vergeben

Im nächsten Fenster haben wir die Auswahl nach einem Dateisystem. NTFS ist ratsam wenn ihr Dateien über 4GB speichern wollt, FAT kann das nicht.

Jetzt einfach mit dem Mauszeiger im Fenster wild hin und her fahren. Wenn man meint man hat es lange genug gemacht geht man auf Formatieren. Je nach Größe des Containers und Leistung deines Rechners kann das etwas dauern.

Es kommt eine Meldung dass das Volume erstellt wurde. Ein Klick auf "Weiter" und wir sind fertig.

Bevor du wichtige Daten in den Container legst teste bitte ob alles funktioniert und du verstanden hast wie man den Container benutzt.

# Container öffnen

- Veracrypt starten
- Freien Laufwerksbuchstaben wählen
- Containerdatei auswählen
- Einbinden klicken
- Passwort eingeben
- Der Container ist nun unter dem Laufwerksbuchstaben verfügbar


#######################################################################################