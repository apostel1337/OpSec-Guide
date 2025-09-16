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
user_pref("app.normandy.enabled", false); // Deaktiviert die Normandy-Funktion von Firefox für Benutzerstudien und Umfragen.
user_pref("app.shield.optoutstudies.enabled", false); // Deaktiviert die Teilnahme an Firefox Shield-Studien.
user_pref("browser.cache.disk.enable", false); // Deaktiviert das Zwischenspeichern von Webseiten auf der Festplatte.
user_pref("browser.cache.disk_cache_ssl", false); // Deaktiviert das Zwischenspeichern von SSL (HTTPS)-Inhalten auf der lokalen Festplatte.
user_pref("browser.cache.offline.enable", false); // Deaktiviert das Offline-Zwischenspeichern von Webseiten.
user_pref("browser.fixup.alternate.enabled", false); // Deaktiviert die Funktion von Firefox, Korrekturen für falsch eingegebene URLs vorzuschlagen.
user_pref("browser.newtabpage.enabled", false); // Deaktiviert die neue Registerkarte (New Tab Page) in Firefox.
user_pref("browser.messaging-system.whatsNewPanel.enabled", false); // Deaktiviert das "Was gibt es Neues"-Panel in Firefox.
user_pref("browser.newtabpage.activity-stream.feeds.snippets", false); // Deaktiviert Snippets auf der neuen Registerkarte.
user_pref("browser.newtabpage.activity-stream.feeds.topsites", false); // Deaktiviert Top-Websites auf der neuen Registerkarte.
user_pref("browser.newtabpage.activity-stream.feeds.system.topsites", false); // Deaktiviert System-Top-Websites auf der neuen Registerkarte.
user_pref("browser.newtabpage.activity-stream.showSponsored", false); // Deaktiviert gesponserten Inhalt auf der neuen Registerkarte.
user_pref("browser.newtabpage.activity-stream.showSponsoredTopSites", false); // Deaktiviert gesponserte Top-Websites auf der neuen Registerkarte.
user_pref("browser.newtabpage.activity-stream.asrouter.userprefs.cfr.addons", false); // Deaktiviert die Benutzerpräferenzen für die Empfehlungen von Add-Ons auf der neuen Registerkarte.
user_pref("browser.newtabpage.activity-stream.asrouter.userprefs.cfr.features", false); // Deaktiviert die Benutzerpräferenzen für die Empfehlungen von Funktionen auf der neuen Registerkarte.
user_pref("browser.pagethumbnails.capturing_disabled", true); // Deaktiviert das Erfassen von Seitenminiaturen für die Miniaturansicht.
user_pref("browser.ping-centre.telemetry", false); // Deaktiviert die Telemetrie für Ping Center.
user_pref("browser.region.update.enabled", false); // Deaktiviert die Regionenaktualisierung.
user_pref("browser.region.network.url", ""); // Setzt die Netzwerk-URL für die Region auf eine leere Zeichenfolge.
user_pref("browser.search.update", false); // Deaktiviert die Aktualisierung der Suchmaschinen.
user_pref("browser.search.suggest.enabled", false); // Deaktiviert die automatische Vervollständigung von Suchanfragen.
user_pref("browser.sessionstore.privacy_level", 2); // Setzt den Datenschutzlevel für die Sitzungswiederherstellung auf 2, um keine zusätzlichen Sitzungsdaten zu speichern.
user_pref("browser.startup.homepage_override.mstone", "ignore"); // Setzt die Homepage-Überschreibung auf "ignore".
user_pref("browser.startup.page", 0); // Setzt die Startseite auf eine leere Seite.
user_pref("com.webaudio.enabled", false); // Bestimmte Angriffe und Tracking-Methoden können die Web Audio API nutzen, um Informationen über den Benutzer zu sammeln.
user_pref("privacy.resistFingerprinting", false); // Muss deaktiviert bleiben, wenn FPP (privacy.fingerprintingProtection) aktiv ist, um Konflikte zu vermeiden.
user_pref("privacy.resistFingerprinting.autoDeclineNoUserInputCanvasPrompts", false);  // Zugriff auf Canvas-Inhalte werden abgelehnt, wenn keine Benutzerinteraktion vorliegt. 


user_pref("browser.topsites.contile.enabled", false); // Deaktiviert die Top-Sites-Kacheln in der neuen Tab-Seite.
user_pref("browser.uitour.enabled", false); // Deaktiviert die User-Tour-Funktion.
user_pref("browser.uitour.url", ""); // Setzt die URL für die User-Tour auf eine leere Zeichenfolge.
user_pref("browser.urlbar.trimURLs", false); // Deaktiviert das Kürzen von URLs in der Adressleiste.
user_pref("browser.urlbar.groupLabels.enabled", false); // Deaktiviert die Gruppenbeschriftungen in der Adressleiste.
user_pref("browser.urlbar.suggest.openpage", false); // Deaktiviert die automatische Vervollständigung von URL-Vorschlägen beim Eintippen.
user_pref("browser.urlbar.suggest.searches", false); // Deaktiviert die automatische Vervollständigung von Suchanfragen in der Adressleiste.
user_pref("browser.urlbar.suggest.topsites", false); // Deaktiviert die automatische Vervollständigung von Top-Sites in der Adressleiste.
user_pref("browser.vpn_promo.enabled", false); // Deaktiviert die VPN-Promotions in Firefox.


/* Healthreport und Telemetriedaten für Mozilla **/
user_pref("datareporting.healthreport.uploadEnabled", false); // Deaktiviert das Hochladen von Healthreport-Daten an Mozilla.
user_pref("datareporting.policy.dataSubmissionEnabled", false); // Deaktiviert die Datenübermittlung an Mozilla.
user_pref("toolkit.telemetry.archive.enabled", false); // Deaktiviert die Archivierung von Telemetriedaten.
user_pref("extensions.getAddons.cache.enabled", false); // Deaktiviert den Cache für Add-on-Updates.
user_pref("dom.security.https_first", true); // Aktiviert HTTPS-First, um sichere Verbindungen zu bevorzugen.
user_pref("dom.vibrator.max_vibrate_ms", 0); // Setzt die maximale Vibrationsdauer auf 0 Millisekunden (deaktiviert Vibration).
user_pref("extensions.htmlaboutaddons.recommendations.enabled", false); // Deaktiviert Add-on-Empfehlungen auf der "about:addons"-Seite.
user_pref("extensions.ui.lastCategory", "addons://list/extension"); // Setzt die zuletzt geöffnete Kategorie in den Add-ons auf "Erweiterungen".
user_pref("extensions.pocket.enabled", false); // Deaktiviert die Pocket-Integration.
user_pref("extensions.systemAddon.update.enabled", false); // Deaktiviert Updates für System-Add-ons.
user_pref("extensions.webextensions.restrictedDomains", ""); // Leert die Liste der eingeschränkten Domains für WebExtensions.
user_pref("layout.css.font-visibility.standard", 1); // Setzt die Sichtbarkeit von Schriftarten auf Standard.
user_pref("browser.tabs.crashReporting.sendReport", false); // Deaktiviert das Senden von Absturzberichten (Firefox 44+).
user_pref("browser.crashReports.unsubmittedCheck.enabled", false); // Deaktiviert die Überprüfung auf nicht eingereichte Absturzberichte.
user_pref("browser.crashReports.unsubmittedCheck.autoSubmit2", false); // Deaktiviert das automatische Senden von nicht eingereichten Absturzberichten.



/** Die internen Adressen aus dem LAN müssen somit nicht publiziert werden. Mit folgenden Optionen kann man es abschalten: **/
user_pref("media.peerconnection.ice.default_address_only", true); // Setzt die Verwendung von Standard-Adressen für WebRTC ein.
user_pref("media.peerconnection.ice.no_host", true); // Verhindert das Senden von Hostnamen in WebRTC.
user_pref("media.peerconnection.enabled", false); // Deaktiviert WebRTC.
user_pref("network.captive-portal-service.enabled", false); // Deaktiviert den Captive Portal Service.
user_pref("network.connectivity-service.enabled", false); // Deaktiviert den Connectivity Service.
user_pref("network.cookie.cookieBehavior", 5); // Setzt das Cookie-Verhalten auf "Nur von der besuchten Seite akzeptieren".
user_pref("network.cookie.lifetimePolicy", 2); // Setzt die Cookie-Lebensdauer auf "Nach Sitzungsende löschen".
user_pref("network.IDN_show_punycode", true); // Zeigt Punycode in internationalisierten Domainnamen an.
user_pref("network.manage-offline-status", false); // Deaktiviert das Verwalten des Offline-Status.
user_pref("permissions.isolateBy.userContext", true); // Isoliert Berechtigungen nach Benutzerkontext.
user_pref("places.history.enabled", false); // Deaktiviert die Speicherung von Browserverlauf.
user_pref("privacy.cpd.offlineApps", true); // Löscht Offline-Webseitendaten beim Beenden des Browsers.
user_pref("privacy.cpd.passwords", true); // Löscht gespeicherte Passwörter beim Beenden des Browsers.
user_pref("privacy.cpd.siteSettings", true); // Löscht Website-Einstellungen beim Beenden des Browsers.
user_pref("privacy.donottrackheader.enabled", false); // Deaktiviert den Do Not Track-Header.
user_pref("privacy.firstparty.isolate", true); // Isoliert viele verschiedene Arten von identifizierenden Daten, um das Tracking über verschiedene Domains hinweg zu verhindern.
user_pref("privacy.firstparty.isolate.block_post_message", false); // Blockiert keine Post-Nachrichten für isolierte Erstanbieter.
user_pref("privacy.history.custom", true); // Aktiviert die individuelle Konfiguration des Browserverlaufs.
user_pref("privacy.query_stripping.enabled", true); // Aktiviert das Entfernen von Suchanfragen aus der URL.
user_pref("privacy.sanitize.sanitizeOnShutdown", true); // Löscht private Daten beim Beenden des Browsers.
user_pref("privacy.userContext.enabled", true); // Aktiviert den Benutzerkontext-Modus.
user_pref("privacy.userContext.ui.enabled", true); // Aktiviert die Benutzeroberfläche für den Benutzerkontext-Modus.
user_pref("privacy.userContext.longPressBehavior", 2); // Setzt das Verhalten für längeres Drücken im Benutzerkontext-Modus auf "Standard".
user_pref("security.insecure_connection_icon.enabled", true); // Aktiviert das Symbol für unsichere Verbindungen.
user_pref("security.insecure_connection_icon.pbmode.enabled", true); // Aktiviert das Symbol für unsichere Verbindungen im privaten Browsing-Modus.
user_pref("security.insecure_connection_text.enabled", true); // Aktiviert den Text für unsichere Verbindungen.
user_pref("security.insecure_connection_text.pbmode.enabled", true); // Aktiviert den Text für unsichere Verbindungen im privaten Browsing-Modus.
user_pref("security.mixed_content.upgrade_display_content", true); // Aktualisiert gemischte Inhalte in Anzeigen.
user_pref("services.settings.server", "https://s.%.c.invalid/v1"); // Setzt den Server für Diensteinstellungen.
user_pref("signon.autofillForms", false); // Deaktiviert das automatische Ausfüllen von Formularen.
user_pref("signon.formlessCapture.enabled", false); // Deaktiviert die Erfassung von Anmeldeinformationen ohne Formulare.
user_pref("xpinstall.signatures.required", false); // Erfordert keine digitalen Signaturen für Add-ons.




/*  Um diese Datenübertragung an Mozilla ebenfalls zu deaktivieren, muss man unter "about:config" folgende Variablen neu anlegen:   */
user_pref("toolkit.coverage.endpoint.base", ""); // Setzt die Basis-URL für die Codeabdeckung auf leer.
user_pref("toolkit.coverage.opt-out", true); // Opt-out aus der Codeabdeckung.
user_pref("toolkit.telemetry.coverage.opt-out", true); // Opt-out aus der Codeabdeckung für Telemetriedaten.
user_pref("toolkit.telemetry.hybridContent.enabled", false); // Deaktiviert Telemetrie für hybride Inhalte.
user_pref("toolkit.telemetry.bhrPing.enabled", false); // Deaktiviert Telemetrie für BHR-Ping.
user_pref("toolkit.telemetry.firstShutdownPing.enabled", false); // Deaktiviert Telemetrie für den ersten Shutdown-Ping.
user_pref("toolkit.telemetry.newProfilePing.enabled", false); // Deaktiviert Telemetrie für den Ping eines neuen Profils.
user_pref("toolkit.telemetry.shutdownPingSender.enabled", false); // Deaktiviert den Sender für Shutdown-Pings.
user_pref("toolkit.telemetry.updatePing.enabled", false); // Deaktiviert Telemetrie für Update-Pings.
user_pref("toolkit.telemetry.unified", false); // Deaktiviert einheitliche Telemetrie.
user_pref("ui.use_standins_for_native_colors", true); // Verwendet Platzhalter für natürliche Farben.
user_pref("webgl.enable-debug-renderer-info", false); // Deaktiviert die Anzeige von Debug-Renderer-Informationen für WebGL, um das Fingerprinting der Grafikkarte zu vermeiden.
user_pref("security.ssl.require_safe_negotiation", true); // Erfordert sichere Verhandlungen für SSL.
user_pref("security.ssl.treat_unsafe_negotiation_as_broken", true); // Behandelt unsichere Verhandlungen als fehlerhaft.



user_pref("privacy.trackingprotection.fingerprinting.enabled", true); // Aktiviert den Schutz vor Fingerprinting.
user_pref("privacy.trackingprotection.cryptomining.enabled", true); // Blockiert Cryptomining.
user_pref("browser.send_pings", false); // Deaktiviert das Senden von Pings, um das Tracking von Klicks zu verhindern.
user_pref("beacon.enabled", false); // Deaktiviert das Beacon API.
user_pref("webgl.disabled", true); // Deaktiviert WebGL, um das Fingerprinting Ihres Geräts zu verhindern.
user_pref("geo.enabled", false); // Deaktiviert die GEO-Ortung.
user_pref("webgl.disable-extensions", true); // Deaktiviert WebGL-Erweiterungen, um das Fingerprinting zu verhindern.
user_pref("webgl.min_capability_mode", true); // Deaktiviert WebGL im Mindestfunktionsmodus, um das Fingerprinting zu verhindern.
user_pref("app.update.service.enabled", false); // Deaktiviert Hintergrundupdates.
user_pref("privacy.trackingprotection.enabled", false); // Deaktiviert den Tracking-Schutz.
user_pref("privacy.trackingprotection.pbmode.enabled", false); // Deaktiviert den Tracking-Schutz im privaten Browsing-Modus.
user_pref("network.http.sendRefererHeader", 2); // Deaktiviert das Senden des Referers in den Header.
user_pref("privacy.clearOnShutdown.cache", true); // Löscht den Cache beim Schließen des Browsers.
user_pref("privacy.clearOnShutdown.downloads", true); // Löscht die Download-Historie beim Schließen des Browsers.
user_pref("privacy.clearOnShutdown.history", true); // Löscht die Browser-Historie beim Schließen des Browsers.
user_pref("privacy.clearOnShutdown.sessions", true); // Löscht die Sitzungsdaten beim Schließen des Browsers.


user_pref("browser.display.use_document_fonts", 1); // Erlaubt die Darstellung von serverseitig bereitgestellten Schriften (Fonts).
user_pref("browser.formfill.enable", false); // Deaktiviert das automatische Ausfüllen von Formularen.
user_pref("browser.safebrowsing.downloads.remote.url", " "); // Leert die URL für sicheres Browsen bei Downloads.
user_pref("browser.safebrowsing.downloads.enabled", false); // Deaktiviert sicheres Browsen bei Downloads.
user_pref("browser.safebrowsing.phishing.enabled", false); // Deaktiviert den Schutz vor Phishing-Seiten.
user_pref("browser.safebrowsing.malware.enabled", false); // Deaktiviert den Schutz vor Malware.
user_pref("browser.safebrowsing.downloads.remote.enabled", false); // Deaktiviert sicheres Browsen bei Remote-Downloads.
user_pref("browser.safebrowsing.downloads.remote.block_dangerous", false); // Deaktiviert das Blockieren gefährlicher Remote-Downloads.
user_pref("browser.safebrowsing.downloads.remote.block_dangerous_host", false); // Deaktiviert das Blockieren gefährlicher Remote-Hosts.
user_pref("browser.safebrowsing.downloads.remote.block_potentially_unwanted", false); // Deaktiviert das Blockieren potenziell unerwünschter Remote-Downloads.
user_pref("browser.safebrowsing.downloads.remote.block_uncommon", false); // Deaktiviert das Blockieren ungewöhnlicher Remote-Downloads.
user_pref("browser.safebrowsing.blockedURIs.enabled", false); // Deaktiviert das Blockieren von URIs durch sicheres Browsen.
user_pref("browser.safebrowsing.provider.google.gethashURL", ""); // Leert die Google-URL für sicheres Browsen.
user_pref("browser.safebrowsing.provider.google.updateURL", ""); // Leert die Google-Update-URL für sicheres Browsen.
user_pref("browser.safebrowsing.provider.google4.gethashURL", ""); // Leert die Google4-URL für sicheres Browsen.
user_pref("browser.safebrowsing.provider.google4.updateURL", ""); // Leert die Google4-Update-URL für sicheres Browsen.
user_pref("browser.safebrowsing.provider.mozilla.gethashURL", ""); // Leert die Mozilla-URL für sicheres Browsen.
user_pref("browser.safebrowsing.provider.mozilla.updateURL", ""); // Leert die Mozilla-Update-URL für sicheres Browsen.
user_pref("browser.urlbar.speculativeConnect.enabled", false); // Deaktiviert das Vorabladen von URLs in der Adressleiste.
user_pref("dom.security.https_only_mode", false); // Deaktiviert den HTTPS-Only-Modus.
user_pref("dom.security.https_only_mode_send_http_background_request", false); // Deaktiviert Hintergrund-HTTP-Anfragen im HTTPS-Only-Modus.
user_pref("extensions.blocklist.enabled", false); // Deaktiviert die Blockliste für Erweiterungen.
user_pref("extensions.formautofill.addresses.enabled", false); // Deaktiviert das automatische Ausfüllen von Adressen in Formularen.
user_pref("extensions.formautofill.creditCards.enabled", false); // Deaktiviert das automatische Ausfüllen von Kreditkartendaten in Formularen.
user_pref("extensions.formautofill.heuristics.enabled", false); // Deaktiviert die Heuristik für das automatische Ausfüllen von Formularen.
user_pref("extensions.screenshots.disabled", true); // Deaktiviert die Screenshots-Funktion.
user_pref("font.blacklist.underline_offset", ""); // Leert die Liste der unterdrückten Schriftarten.
user_pref("media.eme.enabled", false); // Deaktiviert die automatische Wiedergabe von DRM-gesteuerten HTML5-Inhalten.
user_pref("media.gmp-gmpopenh264.enabled", false); // Deaktiviert das OpenH264-Plugin für die Wiedergabe von H.264-Video.
user_pref("media.navigator.enabled", false); // Deaktiviert die Erfassung von Mikrofon- und Kamerainformationen durch Websites.
user_pref("media.navigator.video.enabled", true); // Aktiviert die Video-Funktion für die Erfassung von Mikrofon- und Kamerainformationen.
user_pref("media.gmp-gmpopenh264.autoupdate", false); // Deaktiviert die automatische Aktualisierung des OpenH264-Plugins.
user_pref("media.gmp-gmpopenh264.provider.enabled", false); // Deaktiviert den OpenH264-Provider.
user_pref("media.gmp-gmpopenh264.visible", false); // Deaktiviert die Anzeige des OpenH264-Plugins.
user_pref("media.gmp-manager.url", "data:text/plain,"); // Leert die URL des GMP-Managers.
user_pref("media.gmp-manager.url.override", "data:text/plain,"); // Leert die überschriebene URL des GMP-Managers.
user_pref("media.video_stats.enabled", false); // Deaktiviert die Erfassung von Video-Statistiken.
user_pref("network.dns.disablePrefetch", true); // Deaktiviert das DNS-Prefetching.
user_pref("network.predictor.enabled", false); // Deaktiviert den Netzwerk-Prädiktor.
user_pref("network.prefetch-next", false); // Deaktiviert das Vorabrufen von Seiten.
user_pref("network.http.altsvc.enabled", false); // Deaktiviert den HTTP-Alternative Services.
user_pref("network.http.altsvc.oe", false); // Deaktiviert den OE (Opportunistic Encryption) für HTTP-Alternative Services.
user_pref("network.http.referer.XOriginPolicy", 2); // Setzt die Referer-Politik auf "2" (nur beim Navigieren auf dieselbe Domain wird der Referer übertragen).
user_pref("pdfjs.enableScripting", false); // Deaktiviert das Ausführen von Skripten in PDF.js.
user_pref("plugin.default.state", 0); // Deaktiviert alle Plugins standardmäßig.
user_pref("security.cert_pinning.enforcement_level", 2); // Setzt das Zertifikats-Pinning auf Stufe 2 (strenges Pinning).
user_pref("security.certerrors.mitm.auto_enable_enterprise_roots", false); // Deaktiviert die automatische Aktivierung von Enterprise-Root-Zertifikaten bei Man-in-the-Middle-Angriffen.
user_pref("security.family_safety.mode", 0); // Deaktiviert den Family Safety-Modus.
user_pref("ui.systemUsesDarkTheme", 0); // Verwendet das helle Thema (Light Theme) im System.
user_pref("webgl.disable-fail-if-major-performance-caveat", true); // Deaktiviert WebGL, wenn ein großer Leistungsnachteil vorliegt.



// Bitte beachten Sie, dass diese Einstellungen optional sind und je nach Ihren Anforderungen aktiviert oder deaktiviert werden können.
user_pref("browser.chrome.site_icons", true); // Aktiviert die Anzeige von Website-Symbolen in der Adressleiste.
user_pref("browser.eme.ui.enabled", false); // Deaktiviert das Benutzeroberflächen-Element für EME (Encrypted Media Extensions).
user_pref("browser.sessionstore.max_tabs_undo", 0); // Begrenzt die Anzahl der rückgängig gemachten Tabs auf 0.
user_pref("browser.sessionstore.max_windows_undo", 0); // Begrenzt die Anzahl der rückgängig gemachten Fenster auf 0.
user_pref("dom.event.clipboardevents.enabled", false); // Deaktiviert die Ereignisse zur Zwischenablage und verhindert, dass Websites Daten darüber sammeln, was Sie von einer Webseite kopieren, einfügen oder ausschneiden können.
user_pref("dom.push.connection.enabled", false); // Deaktiviert die Push-Verbindung.
user_pref("dom.push.enabled", false); // Deaktiviert Push-Benachrichtigungen.
user_pref("dom.push.serverURL", ""); // Setzt die URL des Push-Servers auf leer.
user_pref("gfx.direct2d.disabled", true); // Deaktiviert Direct2D-Grafikbeschleunigung.
user_pref("gfx.downloadable_fonts.enabled", true); // Aktiviert herunterladbare Schriftarten.
user_pref("gfx.font_rendering.opentype_svg.enabled", false); // Deaktiviert das Rendern von OpenType-SVG-Schriftarten.
user_pref("gfx.font_rendering.graphite.enabled", false); // Deaktiviert Graphite-Schriftarten.
user_pref("identity.fxaccounts.enabled", false); // Deaktiviert Firefox-Konten-Integration.

user_pref("layout.css.font-loading-api.enabled", false); // Deaktiviert das CSS Font Loading API.
user_pref("media.autoplay.default", 5); // Ändert das Standard-Autoplay-Verhalten auf "Blockieren".
user_pref("media.autoplay.blocking_policy", 2); // Setzt die Autoplay-Blockierungsrichtlinie auf "Blockieren".
user_pref("media.hardware-video-decoding.enabled", false); // Deaktiviert die hardwarebeschleunigte Video-Decodierung.
user_pref("privacy.clearOnShutdown.offlineApps", true); // Löscht Offline-App-Daten beim Beenden des Browsers.
user_pref("privacy.clearOnShutdown.siteSettings", true); // Löscht Site-Einstellungen beim Beenden des Browsers.
user_pref("pdfjs.disabled", false); // Aktiviert den integrierten PDF-Betrachter.
user_pref("signon.rememberSignons", false); // Deaktiviert das Merken von Anmeldedaten für Websites.
user_pref("svg.disabled", false); // Aktiviert das Rendern von SVG-Grafiken.


user_pref("privacy.clearOnShutdown.cookies", true); // Löscht Cookies beim Schließen des Browsers.

user_pref("privacy.fingerprintingProtection", true); // Aktiviert den integrierten Schutz gegen Fingerprinting in Firefox (FPP), wodurch zusätzliche Add-ons wie CanvasBlocker nicht mehr erforderlich sind
user_pref("media.peerconnection.turn.disable", true); // stellt die Deaktivierung von TURN-Servern sicher, dass die Verbindung nicht über einen TURN-Server geleitet wird.

user_pref("network.http.referer.spoofSource", true); // Täuscht die Quelle des Referers vor.
user_pref("network.http.referer.XOriginTrimmingPolicy", 2); // Nur der Ursprung der URL wird im Referer-Header angezeigt
user_pref("layers.acceleration.disabled", true); // Deaktiviert die Hardwarebeschleunigung, um potenzielle Sicherheitsrisiken durch GPU-bezogene Sicherheitslücken zu vermeiden.
user_pref("dom.serviceWorkers.enabled", false); // Da Service Worker persistent im Hintergrund laufen, können sie potenziell für Tracking-Zwecke verwendet werden.
user_pref("dom.battery.enabled", false); // Die Battery API kann theoretisch auch zur Fingerprint-Erstellung beitragen.
user_pref("browser.cache.offline.storage.enable", false); // Deaktiviert die lokale Speicherung.
user_pref("layout.css.visited_links_enabled", false); // Seiten können abfragen, ob bestimmte Links auf "besucht" gesetzt sind und somit Rückschlüsse darauf ziehen, welche Seiten du bereits besucht hast.
user_pref("privacy.resistFingerprinting.letterboxing", true); // Fügt Balken hinzu, um die Fenstergröße zu standardisieren

user_pref("network.cookie.thirdparty.sessionOnly", true); // Drittanbieter-Cookies nur für die aktuelle Sitzung in isolierten Tabs.
user_pref("network.trr.mode", 5); // Setzt DNS-über-HTTPS (DoH) als Standardmodus


// URLs für Updates entfernen
user_pref("app.update.url.details", "");
user_pref("app.update.url.manual", "");


user_pref("geo.wifi.uri", "http://127.0.0.1"); // Leitet Standortanfragen auf die lokale Adresse um, verhindert das Senden an Geodienste.
user_pref("toolkit.telemetry.server", ""); // Deaktiviert URL für Telemetrie-Datenübertragung.
user_pref("breakpad.reportURL", ""); // Deaktiviert das Senden von Absturzberichten.

user_pref("browser.urlbar.filter.javascript", true); // Verhindert die Anzeige von JavaScript in URLs (Sicherheitsmaßnahme).

// Flash-bezogene Einstellungen
user_pref("dom.ipc.plugins.flash.subprocess.crashreporter.enabled", false); // Deaktiviert Plugin-Absturzberichte.
user_pref("dom.ipc.plugins.reportCrashURL", false); // Verhindert das Senden von Absturz-URLs.

user_pref("browser.cache.memory.enable", false); // Deaktiviert den Memory-Cache (reduziert Tracking, aber Leistungseinbußen möglich).

// OCSP und Zertifikatsüberprüfung
user_pref("security.OCSP.require", false); // Erfordert keine OCSP-Überprüfung (Trade-off zwischen Sicherheit und Privatsphäre).
user_pref("security.OCSP.enabled", 0); // Deaktiviert OCSP komplett (privater, aber weniger sicher).

user_pref("security.cert_pinning.enforcement_level", 2); // Aktiviert striktes Pinning (sicherer, aber inkompatibel mit einigen AV-Programmen).

// API- und WebRTC-Funktionen
user_pref("media.getusermedia.screensharing.enabled", false); // Deaktiviert Bildschirmfreigabe.
user_pref("dom.gamepad.enabled", false); // Deaktiviert Gamepad-API (Fingerprinting-Schutz).
user_pref("dom.netinfo.enabled", false); // Verhindert Weitergabe von Netzwerkinformationen.
user_pref("dom.enable_user_timing", false); // Deaktiviert User Timing API (Fingerprinting-Schutz).
user_pref("dom.enable_resource_timing", true); // Ermöglicht Timing-API, nötig für Cloudflare-Challenges. Sonst auf false lassen.  info link https://2captcha.com/demo/cloudflare-turnstile-challenge
user_pref("dom.vibrator.enabled", false); // Deaktiviert die Vibration-API.

user_pref("browser.download.useDownloadDir", false); // Fragt vor jedem Download nach Speicherort.
user_pref("device.sensors.enabled", false); // Deaktiviert Zugriff auf Gerätesensoren (Fingerprinting-Schutz).

// Proxy-DNS
user_pref("network.proxy.socks_remote_dns", true); // Lässt DNS-Anfragen über den Proxy laufen, verhindert DNS-Leaks.

// Deaktiviert automatische Updates für Add-ons und Such-Plugins
user_pref("extensions.update.enabled", false); // Add-on-Updates deaktivieren.
user_pref("services.sync.prefs.sync.extensions.update.enabled", false); // Deaktiviert Synchronisation von Add-on-Update-Einstellungen.
user_pref("services.sync.prefs.sync.browser.search.update", false); // Deaktiviert Synchronisation von Such-Plugin-Updates.

// Sync-Dienste für Add-ons deaktivieren
user_pref("services.sync.engine.addons", false); // Synchronisation von Add-ons deaktivieren.
user_pref("services.sync.engine.extensions", false); // Synchronisation von Erweiterungen deaktivieren.

user_pref("dom.private-attribution.submission.enabled", false); // Deaktiviert die Übermittlung von privaten Attributionsdaten, um Tracking durch Firefox zu verhindern.

// Bitte beachten Sie, dass diese Einstellungen die JavaScript-Performance beeinflussen können, aber die Sicherheit erhöhen. Sie können sie nach Ihren Anforderungen aktivieren oder deaktivieren.
user_pref("javascript.options.baselinejit", true); // Deaktiviert zwar den Baseline JIT-Compiler, führt jedoch zu Lag-Problemen und bleibt daher aktiviert.
user_pref("javascript.options.ion", false); // Deaktiviert den Ion JIT-Compiler.
user_pref("javascript.options.native_regexp", false); // Deaktiviert die nativen RegExp-Optimierungen.
```

> 💡 **Tipp:**
> Werte zuerst in einer **Test-Installation** prüfen, bevor du sie auf deinem Hauptsystem nutzt.
> **Credits:** [xqi](https://github.com/xqi1337/FireFox-Cfg/)
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
