## 🕵️ Advanced Anonymity & OpSec Guide

### Kapitel 5 – Festplattenverschlüsselung

> 💡 **Warum verschlüsseln?**
> Falls Polizei, Behörden oder Dritte dein Gerät beschlagnahmen,
> können sie ohne starken Schlüssel **nicht auf deine Daten zugreifen**.
> Selbst Organisationen wie die **CIA** kommen bei starker Verschlüsselung nicht weiter.

---

## 🔑 Empfohlene Software: VeraCrypt

* Offizieller Nachfolger von **TrueCrypt**
* Kostenlos für **Windows, Linux und macOS**
* Verbesserte Sicherheit gegenüber TrueCrypt

**Website:** [https://www.veracrypt.fr/](https://www.veracrypt.fr/)

---

## 📦 Was kann verschlüsselt werden?

* **Einzelne Ordner** (Container-Datei)
* **Komplette Partitionen**
* **Gesamtes System**
* **Versteckte Container** in verschlüsselten Partitionen

---

## 🧰 Container-Prinzip

Ein Container ist wie ein **digitaler Tresor**:

* Es wird eine Datei erstellt (z. B. 500 MB oder 1 GB groß).
* Diese Datei kann wie ein virtuelles Laufwerk eingebunden werden.
* Nur mit dem **richtigen Passwort** lässt sich der Inhalt öffnen.

> ⚠️ **Tipp:**
> Container sind oft sicherer als komplette Partitionen.
> Windows erkennt verschlüsselte Partitionen als „unformatiert“ und könnte
> versehentlich eine Formatierung anbieten.

---

## 🔒 Container erstellen (Schritt-für-Schritt)

1. **VeraCrypt als Administrator starten**

   * Verhindert Fehler beim Erstellen großer Container.
2. **Neues Volume erstellen**

   * „Containerdatei erstellen“ auswählen.
   * „Standard VeraCrypt Volume“ wählen.
3. **Speicherort angeben**

   * Dateiname & Speicherpfad des Containers festlegen.
4. **Verschlüsselungsalgorithmus auswählen**

   * Kombinationen wie **AES + Blowfish** empfohlen.
   * **Hash-Algorithmus:** SHA-512.
5. **Größe des Containers festlegen**

   * Beispiel: 500 MB für USB-Stick, 1 GB für größere Daten.
6. **Passwort vergeben**

   * Starkes Passwort verwenden (lang, komplex).
7. **Dateisystem wählen**

   * NTFS für Dateien >4 GB.
8. **Container formatieren**

   * Mausbewegungen erzeugen Zufallsdaten für den Schlüssel.

Nach Abschluss erscheint die Meldung:

> „Das Volume wurde erfolgreich erstellt.“

---

## 📂 Container einbinden (Mounten)

1. VeraCrypt starten.
2. **Freien Laufwerksbuchstaben** auswählen.
3. **Containerdatei auswählen**.
4. **Einbinden** klicken.
5. Passwort eingeben.
6. Container erscheint als neues Laufwerk und kann wie ein Ordner genutzt werden.

---

## 🛡️ Best Practices

* **Starke Passwörter** (lang + Sonderzeichen).
* Keine Hinweise auf das Passwort speichern.
* Regelmäßige **Backups** verschlüsselter Container.
* Container nach Nutzung **immer aushängen**.

---

## ✅ Zusammenfassung

* VeraCrypt bietet **militärische Sicherheit** bei einfacher Bedienung.
* Containerdateien sind ideal für **USB-Sticks** oder portable Datenträger.
* Kombination aus **starkem Passwort** + **verstecktem Volume** = maximale Sicherheit.

---
