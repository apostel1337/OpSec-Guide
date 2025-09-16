## 🕵️ Advanced Anonymity & OpSec Guide

### Kapitel 3 – Microsoft Windows ist immer unsicher

> ⚠️ **Hinweis**
> Dieses Kapitel beschreibt Datenschutz- und Sicherheitsprobleme von **Microsoft Windows**.
> Ziel ist **Aufklärung**, nicht Panikmache.
> Wer maximale Privatsphäre will, sollte die Risiken kennen und alternative Systeme in Betracht ziehen.

---

## 🖥️ Einführung

Mit **Windows 8.0** begann Microsoft, bei PCs ähnliche Tracking-Mechanismen einzuführen,
wie man sie von Smartphones kennt.
Seitdem hat sich die **Datensammlung** mit jeder Version (8.1, 10, 11) weiter verstärkt.

---

## 📊 Beispiele für Datensammlung

| Bereich                     | Gesammelte Daten                                                 | Anmerkung                       |
| --------------------------- | ---------------------------------------------------------------- | ------------------------------- |
| **Nutzungsprofil**          | Surfverhalten, App-Aktivitäten, persönliche Interessen           | für personalisierte Werbung     |
| **Standortdaten**           | GPS, WLAN-Umgebung, IP-Standort                                  | möglichst genaue Bestimmung     |
| **Kontakte**                | Adressbücher, Freundeslisten                                     | bei Nutzung von Microsoft-Tools |
| **Kommunikation**           | Inhalte von E-Mails, Instant Messages, Voice/Video (z. B. Skype) | laut Privacy Policy             |
| **Systemdaten**             | Installierte Anwendungen (über Windows Defender)                 |                                 |
| **Eingabeverhalten**        | Tastaturanschläge (Keystroke Biometrics)                         | zur Musteranalyse               |
| **Geräte-ID**               | „Unique Advertising ID“ für jedes Benutzerkonto                  | von Drittanbietern nutzbar      |
| **BitLocker Recovery Keys** | Automatische Sicherung in der Microsoft Cloud                    | auch für Behörden zugänglich    |

---

## 🔎 Besondere Kritikpunkte

### Windows 8 / 8.1

* Einführung von **Device-based Tracking**.
* Einrichtung eines **Online-Kontos** wird aggressiv beworben („Dark Pattern“).
* Nur durch falsche Angaben gelang es, ein reines **lokales Konto** zu erstellen.

### Windows 10

* Weiterer Ausbau der Datensammlung:

  * Generiert für jeden Account eine **Advertising ID**.
  * Neue Privacy Policy (2018):

    > „We will access, disclose and preserve personal data, including your content… when we have a good faith belief…“

* **Cortana**:

  * Standardmäßig aktiv – quasi eine „Abhörzentrale“ im Wohnzimmer.
  * Ab Anniversary Update (2016) kaum noch vollständig abschaltbar.

* **BitLocker**:

  * Automatisch generierte **Recovery Keys** werden in die Cloud hochgeladen,
    sofern man dies nicht manuell verhindert.

### Windows & Geheimdienste

* Die eindeutige UUID, die bei Kommunikation mit Microsoft-Servern übermittelt wird,
  dient laut Berichten als Selektor für NSA/GCHQ (**Tailored Access Operations**).

---

## 🛡️ Gegenmaßnahmen (nur teilweise wirksam)

* **Lokales Benutzerkonto** statt Microsoft-Konto verwenden.
* In den **Datenschutzeinstellungen** sämtliche Telemetrie deaktivieren.
  ➜ Allerdings lassen sich viele Dienste **nicht vollständig abschalten**.
* Bei BitLocker:

  1. Erst verschlüsseln (mit Key-Upload),
  2. dann **Entschlüsselung** durchführen,
  3. erneut verschlüsseln → erst beim zweiten Mal kann man den Key lokal speichern.

> ⚠️ **Hinweis**
> Diese Maßnahmen reduzieren, aber **eliminieren nicht** die Datensammlung.

---

## ⚠️ Bewertung durch Behörden

* **BSI (Bundesamt für Sicherheit in der Informationstechnik)**
  warnte bereits 2013 vor Windows 8 in Kombination mit **TPM 2.0**.

  * Risiko: Verlust der Kontrolle über Hard- und Software.
  * Einstufung als **inakzeptables Sicherheitsrisiko** für Behörden und kritische Infrastrukturen.

---

## ✅ Fazit

* Windows ist für **starke Anonymität** **nicht geeignet**.
* Wer auf Windows angewiesen ist:

  * **Ältere Versionen** (z. B. Windows XP oder 7) bieten weniger Telemetrie,
    sind jedoch sicherheitstechnisch veraltet.
* Für maximale Privatsphäre → **Linux-Distributionen** wie **Debian**, **Tails** oder **Qubes OS**.

---
