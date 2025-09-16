## 🕵️ Advanced Anonymity & OpSec Guide

### Kapitel 4 – Anonymisierung von Firefox

> ⚠️ **Hinweis**
> Dieses Kapitel beschreibt, wie du **Mozilla Firefox** mit Add-ons und versteckten Einstellungen
> zu einem **maximal privacy-freundlichen Browser** aufrüstest.

---

## Warum Firefox?

* **Open Source** → Quellcode überprüfbar, keine proprietären Hintertüren.
* Riesige **Community** → Viele Sicherheits-Add-ons und Anleitungen.
* Hohe **Flexibilität** → Anpassbar über `about:config`.

Download: [Mozilla Firefox – Alle Versionen](https://www.mozilla.org/en-US/firefox/all/)

---

## about\:config – Der Konfigurations-Editor

Mit `about:config` erhältst du Zugriff auf **versteckte Einstellungen** aus den Dateien `prefs.js` und `user.js`.

1. In die Adressleiste `about:config` eingeben.
2. Sicherheitswarnung bestätigen („Ich bin mir der Risiken bewusst“).
3. Nach gewünschtem Parameter suchen und per **Doppelklick** oder **Rechtsklick → Modify** anpassen.

> ⚠️ Änderungen nur vornehmen, wenn du deren Wirkung verstehst.
> Falsche Werte können den Browser oder Webseiten beschädigen.

---

## Empfohlene Konfigurationen

```ini
media.peerconnection.enabled = false       # Deaktiviert WebRTC (verhindert IP-Leaks)
geo.enabled = false                         # Standortermittlung abschalten
geo.wifi.uri = [leer lassen]                # Keine WLAN-basierte Standortbestimmung
network.http.use-cache = false              # Kein HTTP-Caching
network.http.keep-alive.timeout = 600
network.http.max-persistent-connections-per-proxy = 16
network.proxy.socks_remote_dns = true       # DNS-Anfragen durch Proxy leiten
network.cookie.lifetimePolicy = 2           # Cookies nur für aktuelle Session
network.http.sendRefererHeader = 0          # Keine Referrer-Daten senden
network.http.sendSecureXSiteReferrer = false
network.protocol-handler.external = false   # Keine externen Protokollaufrufe
network.protocol-handler.warn-external = true
network.http.pipelining = true
network.http.pipelining.maxrequests = 8
network.http.proxy.keep-alive = true
network.http.proxy.pipelining = true
network.prefetch-next = false               # Kein Vorabladen von Seiten
browser.cache.disk.enable = false
browser.cache.offline.enable = false
browser.sessionstore.privacy_level = 2      # Sitzungsdaten minimal speichern
browser.sessionhistory.max_entries = 2
browser.display.use_document_fonts = 0      # Keine Webfonts laden (Fingerprinting)
intl.charsetmenu.browser.cache = ISO-8859-9, windows-1252, windows-1251, ISO-8859-1, UTF-8
dom.storage.enabled = false                 # DOM Storage deaktivieren
extensions.blocklist.enabled = false
```

> 💡 **Tipp:**
> Werte zuerst in einer **Test-Installation** prüfen, bevor du sie auf deinem Hauptsystem nutzt.

---

## Empfohlene Add-ons

| Add-on               | Funktion                                 | Link                                                     |
| -------------------- | ---------------------------------------- | -------------------------------------------------------- |
| **NoScript**         | Blockiert JavaScript und aktive Inhalte  | [NoScript Add-on](https://addons.mozilla.org/)           |
| **HTTPS Everywhere** | Erzwingt HTTPS-Verbindungen              | [HTTPS Everywhere](https://www.eff.org/https-everywhere) |
| **Privacy Badger**   | Blockiert Tracker automatisch            | [Privacy Badger](https://privacybadger.org/)             |
| **RefControl**       | Blockiert oder fälscht den HTTP-Referrer | [RefControl](https://addons.mozilla.org/)                |
| **Secret Agent**     | Rotiert User-Agent-String                | [Secret Agent](https://addons.mozilla.org/)              |
| **Disable WebRTC**   | Verhindert IP-Leaks durch WebRTC         | [Disable WebRTC](https://addons.mozilla.org/)            |

---

## Suchmaschinen ohne Tracking

* [DuckDuckGo](https://duckduckgo.com/) – keine Speicherung von IP oder Suchhistorie.
* [StartPage](https://www.startpage.com/) – Google-Ergebnisse ohne Profiling.
* [eTools.ch](https://www.etools.ch/) – Schweizer Metasuchmaschine.

---

## Sitzungsverwaltung

* Firefox unter `Settings → Privacy` so konfigurieren,
  dass **alle Daten beim Schließen gelöscht** werden:

  * **Chronik löschen, wenn Firefox geschlossen wird**
  * **Cookies nur bis zum Schließen behalten**

---

## Zusammenfassung

1. Firefox installieren und **Add-ons** hinzufügen.
2. `about:config`-Werte anpassen, um Tracking zu minimieren.
3. Nur Suchmaschinen ohne Tracking nutzen.
4. Sitzungs- und Cookie-Löschung aktivieren.

---
