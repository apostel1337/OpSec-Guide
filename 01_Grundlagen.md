## 🕵️ Advanced Anonymity & OpSec Guide

### Kapitel 1 – Vorwort & Grundlagen

> ⚠️ **Hinweis**
> Dieser Guide dient ausschließlich zu **Bildungs- und Datenschutz-Zwecken**.
> Ziel ist es, die eigene **Privatsphäre zu schützen** und **Überwachung zu vermeiden** –
> **keine Anleitung für illegale Aktivitäten**.

---

## Vorwort

Starke Anonymität soll besonders **Risikogruppen** Schutz gegen Repressionen bieten.
Es gibt viele Gründe, warum Menschen Repressionen fürchten:

* **Minderheiten** befürchten Verfolgung durch Mehrheiten.
* **Regelbrecher** oder Aktivisten müssen mit staatlichen Maßnahmen rechnen.

Anonymität im Internet bedeutet, in einer **großen Gruppe mit identischen Merkmalen** unterzutauchen,
damit Einzelne nicht anhand von IP-Adresse, Browsertyp oder Fingerprints identifiziert werden können.

**Vorteil:**
Starke Anonymisierung macht **Tracking** und **Profilbildung** unmöglich.

> 💡 Seit den Enthüllungen von **Edward Snowden** wissen wir:
>
> * Wir sind nicht paranoid – **Überwachung ist Realität**.
> * Jeder wird überwacht – **jetzt und überall**.

---

## 🏁 Grundlagen

### Clearnet vs. Darknet

* **Darknet (Tor)**

  * Leicht zu schützen: TOR-Browser + zusätzliche Tools.
  * Ideal für anonyme Kommunikation oder den Zugriff auf schwer zensierbare Inhalte.
* **Clearnet (normales Internet)**

  * Schwieriger zu anonymisieren:
    Viele Webseiten blockieren TOR-Exitnodes oder erkennen VPNs.
  * Beispiel: **DHL Packstation** sperrt Zugänge nach erstem TOR-Login.

> **Praxis-Tipp**
>
> * Für Darknet → **Tor**
> * Für Clearnet → **sauberes VPN**, unauffällige Verbindung, kein TOR.

---

### Open Source vs. Closed Source

* **Freie Software (Linux, Firefox …)**

  * Quellcode einsehbar → Hintertüren können entdeckt werden.
  * Peer Review: Code wird von mehreren Entwicklern geprüft.
  * **ABER:** Offenheit ≠ absolute Sicherheit (z. B. Heartbleed-Bug).
* **Proprietäre Software (Windows, macOS …)**

  * Quellcode nicht einsehbar → unklare Hintergrundprozesse.

> **Fazit**:
> Linux bietet **mehr Transparenz** und ist im Regelfall **sicherer** als Windows.

---

### Tracker

Viele Webseiten binden Tracker ein, die das Surfverhalten aufzeichnen.

* **Do-Not-Track**: In Firefox unter `Settings → Privacy` aktivierbar,
  aber rechtlich nicht bindend – kaum Seiten respektieren es.
* **Empfohlenes Add-on**:

  * **Privacy Badger** (EFF) → blockiert Tracker automatisch.

---

### Cookies

* **Was sind Cookies?**
  Kleine Dateien, die Surfverhalten und Sitzungen speichern.
* **Problematisch:**

  * **Third-Party-Cookies** (z. B. über eingebettete Facebook-Buttons).
* **Firefox-Einstellungen:**

  1. `Settings → Privacy → Use Custom Settings for History`
  2. `Accept third-party cookies → Never`
  3. **Alle Cookies beim Beenden löschen** aktivieren.

---

### Adobe Flash

* Historisch viele Sicherheitslücken.
* Heute dank **HTML5** überflüssig → **deaktivieren** oder deinstallieren.

---

### NoScript

* Add-on für Firefox, blockiert **JavaScript** und andere aktive Inhalte.
* Standard: Alle Skripte blockiert → nur manuelles Freigeben pro Seite.

---

### WebRTC

* Kann **lokale IP-Adresse** und **öffentliche IP** trotz VPN/Tor preisgeben.
* **Lösung:** Add-on `Disable WebRTC`.

---

### Fake User-Agent

* Jeder Webseitenaufruf übermittelt Browser- & Systeminformationen (**Fingerprinting**).
* **Gegenmaßnahme:** Add-on `Secret Agent` → rotiert User-Agent-Strings.

---

### Referrer

* Überträgt die **Herkunfts-URL** bei jedem Linkklick.
* **Add-on:** `RefControl` → erlaubt gezieltes Blockieren.

---

### Modus des Browsers

* Firefox so einstellen, dass **alle Daten beim Schließen gelöscht** werden:

  * `Settings → Privacy → Clear history when Firefox closes`
  * Cookies nur bis zum Schließen behalten.

---

### Suchmaschinen

Alternative Suchdienste ohne Tracking:

* [DuckDuckGo](https://duckduckgo.com/)
* [StartPage](https://www.startpage.com/)
* [eTools.ch](https://www.etools.ch/)

---

### HTTPS benutzen

* HTTP = unverschlüsselt → leicht abhörbar.
* **Add-on:** [`HTTPS Everywhere`](https://www.eff.org/https-everywhere)
  → erzwingt sichere Verbindungen.

---

### VPN

* Pflicht für echte Anonymität:

  * **IP-Wechsel** + **verschlüsselter Tunnel**.
  * Verhindert Traffic-Analyse.
* **Wichtig:** Starke Verschlüsselung & sichere Schlüssel.

---

### Tor-Netzwerk

* **Onion-Routing**: Mehrere verschlüsselte Knoten weltweit.
* Einfachste Nutzung: [Tor Browser](https://www.torproject.org/).
* Alternative: [Tails OS](https://tails.boum.org/) für spurenloses Arbeiten.

---

### Fazit

Diese Grundlagen bilden die **Basis jeder Anonymitäts-Strategie**.
Alle weiteren Kapitel bauen auf diesen Schutzmaßnahmen auf.

---
