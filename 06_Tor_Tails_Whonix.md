## 🕵️ Advanced Anonymity & OpSec Guide

### Kapitel 6 – Tor, Tails & Whonix

*(Security Stages 1–3)*

> ⚠️ **Hinweis**
> Diese Systeme ermöglichen **maximale Anonymität**.
> Sie dienen der **Privatsphäre** und dem Schutz vor Überwachung –
> **nicht** für illegale Aktivitäten.

---

## 🟢 Stage 1 – Tor-Browser-Bundle

### 🌐 Was ist Tor?

* **Onion-Routing**: Daten werden über mehrere, weltweit verteilte **Tor-Knoten** verschlüsselt geleitet.
* Jeder Knoten kennt nur seinen **direkten Nachbarn**, nicht den gesamten Pfad.
* Am **Exit-Knoten** wird der Datenstrom entschlüsselt – daher **HTTPS** nutzen!

### ✅ Vorteile

* Sehr einfacher Einstieg in anonyme Kommunikation.
* Keine Installation zusätzlicher Komponenten nötig.

### 🔧 Nutzung

1. **Tor Browser** von der offiziellen Website laden:
   [https://www.torproject.org/](https://www.torproject.org/)
2. Installieren und starten.
3. Surfen wie mit Firefox, aber **über Tor**.

> 💡 Für Gelegenheitsnutzer ist der **Tor Browser** meist ausreichend.

---

## 🟠 Stage 2 – Tails (The Amnesic Incognito Live System)

### 💡 Was ist Tails?

* Ein **Live-Betriebssystem**, das sich von **USB-Stick oder DVD** starten lässt.
* Entwickelt, um **keinerlei Spuren** auf dem genutzten Computer zu hinterlassen.
* Inklusive vorkonfigurierter **Sicherheits- und Privacy-Tools**:

  * Webbrowser
  * E-Mail-Client
  * Instant-Messaging
  * Office-Paket
  * Audio-/Bildbearbeitung

### 📦 Vorteile

* Komplett unabhängiges Betriebssystem.
* Keine Installation auf dem Host-Rechner notwendig.
* Option für **Windows-XP-Tarnmodus** (für unauffällige Nutzung).

### 🔧 Installation auf USB-Stick

1. **Download**

   * Original-ISO von [https://tails.boum.org/index.de.html](https://tails.boum.org/index.de.html) herunterladen.
   * Download verifizieren (Firefox-Plugin kann erforderlich sein).
2. **Ersten USB-Stick vorbereiten**

   * Mit dem **Universal USB Installer** die Tails-ISO auf den Stick schreiben.
3. **Booten & Vorab-Version starten**

   * Rechner über den Stick starten (Boot-Menü, z. B. `F12`/`Esc`/`Del`).
4. **Zweiten USB-Stick klonen**

   * Innerhalb von Tails: `Anwendungen → Tails → Tails Installer → Install by Cloning`
   * Ziel: Zweiter Stick → „Install Tails“ → Warnmeldung bestätigen.

> ⚠️ **Tipp:**
> Für maximale Sicherheit kann Tails auch auf **DVD** gebrannt werden –
> Änderungen am System sind dann unmöglich.

---

## 🔴 Stage 3 – Whonix High-Security System

### 🖥️ Konzept

* **Debian-basierte Linux-Distribution**, die konsequent auf **Tor** setzt.
* Besteht aus **zwei virtuellen Maschinen**:

  1. **Gateway** – leitet alle Verbindungen über Tor.
  2. **Workstation** – isolierte Umgebung für tägliche Arbeit.

### ✅ Vorteile

* Sämtlicher Netzwerkverkehr wird **zwangsläufig durch Tor geleitet**.
* Updates erfolgen automatisch über Tor.
* Host-System bleibt isoliert.

### 🔧 Benötigte Software

* **VirtualBox** – Virtualisierungssoftware
  [https://www.virtualbox.org/wiki/Downloads](https://www.virtualbox.org/wiki/Downloads)
* **Whonix** – Download der Images (Gateway + Workstation)
  [https://www.whonix.org/wiki/Download](https://www.whonix.org/wiki/Download)
* Optional: Beliebiges Gastbetriebssystem (z. B. Windows 7) für die Workstation.

### 💡 Installation

1. **VirtualBox installieren**.
2. Whonix-Images (Gateway & Workstation) importieren:

   * `File → Import Appliance…` → `.ova`-Datei auswählen → `Import`.
3. **Starten**

   * Zuerst **Whonix-Gateway**, dann **Whonix-Workstation**.
4. **Erstkonfiguration**

   * Standard-Login: `user` / Passwort: `changeme`.
   * Nach dem ersten Start Updates einspielen.
   * Passwörter ändern (`passwd user`).

> 💡 Arbeiten erfolgt **nur** in der **Workstation**.
> Das Gateway muss immer aktiv sein, da es die Verbindung zum Tor-Netzwerk aufbaut.

---

## 🔐 Vergleich der Security Stages

| Stage | System      | Schwierigkeit   | Anonymität                   | Einsatzgebiet                       |
| ----- | ----------- | --------------- | ---------------------------- | ----------------------------------- |
| **1** | Tor-Browser | Einfach         | Hoch (bei richtiger Nutzung) | Gelegenheits-User                   |
| **2** | Tails OS    | Mittel          | Sehr hoch                    | Spurenfreies Arbeiten               |
| **3** | Whonix      | Fortgeschritten | Maximal                      | Dauerhafte High-Security-Umgebungen |

---

## ✅ Zusammenfassung

* **Tor-Browser**: Schnell und einfach → ideal für Einsteiger.
* **Tails**: Komplettes Live-System → keine Spuren auf dem Rechner.
* **Whonix**: Höchste Sicherheit → aber komplexer und ressourcenintensiver.

---
