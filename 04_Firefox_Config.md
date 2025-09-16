#######################################################################################

Mozilla Firefox ist der Webbrowser der Mozilla Foundation und kann durch viele von der Community entwickelte Add-ons und Anpassungen in der Konfiguration zu einem sicheren und privacy-freundlichen Browser aufgewertet werden. Er ist kostenfrei nutzbar und steht auf der Downloadseite für Windows und MacOS bereit.
→ https://www.mozilla.org/en-US/firefox/all/


### Firefox about:config

Der Konfigurations-Editor listet alle möglichen Firefox Settings die aus den Dateien prefs.js und user.js gelesen werden können. Zusätzlich werden hier die Default-Einstellungen angezeigt. Viele dieser Einstellungen können nur so geändert werden und sind nicht über die üblichen Menüs erreichbar. Mit der Eingabe von "about:config" in der Adressleiste des Firefox kann die Settings-Page aufgerufen werden. Es erscheint eine Warnung die fragt ob man wirklich weiß was man tut. In diesen Settings sollten nur Einstellungen geändert werden deren Auswirkung man sich auch bewusst ist. Andernfalls können schnell weitere Sicherheitslücken entstehen.

Um einen bestehenden Wert zu ändern musst du einen rechtsklick auf die entsprechende Einstellung machen und dann "Modify" klicken. Alternativ kannst du auch einen Doppelklick machen. Dann kannst du den neuen Wert in das sich öffnende Fenster eintragen. Um nach bestimmten Einstellungen zu suchen kannst du einfach die Suchleiste ganz oben verwenden.

# Nützliche Firefox Mods

media.peerconnection.enabled  =  false
geo.enabled = false
geo.wifi.uri = [leave blank]
network.http.accept.default = text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8
network.http.use-cache = false
network.http.keep-alive.timeout = 600
network.http.max-persistent-connections-per-proxy = 16
network.proxy.socks_remote_dns = true
network.cookie.lifetimePolicy = 2
network.http.sendRefererHeader = 0
network.http.sendSecureXSiteReferrer = false
network.protocol-handler.external = false [set the default and all the subsettings to false]
network.protocol-handler.warn-external = true [set the default and all the subsettings to true]
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


#######################################################################################