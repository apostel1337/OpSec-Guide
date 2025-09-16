## 🕵️ Advanced Anonymity & OpSec Guide

### Kapitel 2 – Browser Hardening & Online-Schutz

Dieses Kapitel zeigt, wie man den **Webbrowser** absichert, um Tracking, Fingerprinting und Datenabfluss zu verhindern.

---

## 🌍 Firefox Add-ons & Einstellungen

### 🔧 NoScript

* Blockiert **JavaScript** und andere aktive Elemente.
* Standardmäßig sind **alle Skripte verboten**.
* Freischaltung pro Webseite möglich.
* Nützlich gegen **Tracking per Java**.

> ⚠️ **Achtung:**
> Manche Websites (z. B. Google Captchas) benötigen JavaScript.
> Bei Darstellungsproblemen schrittweise Skripte temporär zulassen.

---

### 🔒 HTTPS Everywhere

* Erzwingt verschlüsselte **HTTPS-Verbindungen**, wenn verfügbar.
* Entwickelt von der **Electronic Frontier Foundation (EFF)**.
* Aktiviert sich nach Installation automatisch.

---

### 🕵️ Privacy Badger

* Blockiert **Tracker** und verhindert Übermittlung von Daten an Dritte.
* Ebenfalls ein Projekt der **EFF**.
* Keine komplizierte Konfiguration notwendig.

---

### 🍪 Cookies

* Cookies speichern **Nutzersitzungen** und erlauben eindeutige Zuordnung.

**Empfohlene Firefox-Einstellungen**

1. `Settings → Privacy → Use Custom Settings for History`
2. `Accept third-party cookies → Never`
3. **Alle Cookies beim Beenden löschen** aktivieren.

> 💡 Third-Party-Cookies stammen von eingebetteten Fremdseiten (z. B. Facebook-Like-Button)
> und setzen Cookies auch ohne aktives Anklicken.

---

### 🌐 WebRTC

* Kann trotz VPN/Tor die **lokale IP-Adresse** preisgeben.
* **Add-on:** [Disable WebRTC](https://addons.mozilla.org/) deaktiviert die Übermittlung.

---

### 🕵️‍♂️ Fake User-Agent

* Webseiten lesen den **User-Agent-String** (Browsername, Version, Betriebssystem, Schriftarten).
* Dient dem **Fingerprinting** und ermöglicht Wiedererkennung.

**Empfohlene Maßnahme:**

* Add-on [`Secret Agent`](https://addons.mozilla.org/) → rotiert den User-Agent automatisch.
* „Stealth Mode“ aktivieren und Zeitintervall für Rotation festlegen.

---

### ↩️ Referrer

* Übermittelt beim Klicken auf Links die **Herkunfts-URL** an die Zielseite.

**Add-on:** [RefControl](https://addons.mozilla.org/)

* Standardaktion: „Block“
* Optional nur für **3rd Party requests** aktivieren.

---

## ⚡ Adobe Flash

* Historisch **zahlreiche Sicherheitslücken**.
* Heutzutage durch **HTML5** ersetzt → **deinstallieren oder deaktivieren**.

> 💡 Falls Flash zwingend benötigt wird:
>
> * Lokalen Cache deaktivieren
> * `Global Settings → Storage → Block all sites from storing information`

---

## 🔧 Firefox `about:config` Hardening

Viele wichtige Sicherheitsoptionen sind nur über `about:config` erreichbar.
In der Adresszeile `about:config` eingeben und mit **Vorsicht** ändern.

**Empfohlene Werte**:

```ini
media.peerconnection.enabled = false
geo.enabled = false
geo.wifi.uri = [leer lassen]
network.http.use-cache = false
network.http.keep-alive.timeout = 600
network.http.max-persistent-connections-per-proxy = 16
network.proxy.socks_remote_dns = true
network.cookie.lifetimePolicy = 2
network.http.sendRefererHeader = 0
network.http.sendSecureXSiteReferrer = false
network.protocol-handler.external = false
network.protocol-handler.warn-external = true
network.http.pipelining = true
network.http.pipelining.maxrequests = 8
network.http.proxy.keep-alive = true
network.http.proxy.pipelining = true
network.prefetch-next = false
browser.cache.disk.enable = false
browser.cache.offline.enable = false
browser.sessionstore.privacy_level = 2
browser.sessionhistory.max_entries = 2
browser.display.use_document_fonts = 0
intl.charsetmenu.browser.cache = ISO-8859-9, windows-1252, windows-1251, ISO-8859-1, UTF-8
dom.storage.enabled = false
extensions.blocklist.enabled = false
```

> ⚠️ **Hinweis:**
> Änderungen nur vornehmen, wenn du deren Wirkung verstehst.
> Falsche Werte können die Browserfunktionalität einschränken.

---

## 🔍 Suchmaschinen ohne Tracking

* [DuckDuckGo](https://duckduckgo.com/) – speichert keine IPs oder Nutzerprofile.
* [StartPage](https://www.startpage.com/) – Google-Ergebnisse ohne personalisierte Suche.
* [eTools.ch](https://www.etools.ch/) – Schweizer Metasuchmaschine.

---

## 🔐 VPN (als Ergänzung)

* Ein **VPN** ist Pflicht für echte Anonymität.
* Vorteile:

  * Versteckt die **reale IP-Adresse**.
  * Erstellt einen **verschlüsselten Tunnel**, den weder ISP noch Knotenpunkte mitlesen können.
* Wichtig: Starke **Verschlüsselung** und **sicherer Schlüsseltausch**.

---

## ✅ Zusammenfassung Browser Hardening

1. **VPN + Firefox** als Basis.
2. Add-ons: `NoScript`, `HTTPS Everywhere`, `Privacy Badger`, `RefControl`, `Secret Agent`.
3. `about:config` anpassen, Cookies & WebRTC deaktivieren.
4. Suchmaschinen wie DuckDuckGo oder StartPage nutzen.

---
