# Developer Mode Setup Anleitung

## Zweck & Kontext
Diese Anleitung bietet die erforderlichen Schritte zur Autorisierung eines Meta-Kontos und der mit diesem Konto verbundenen Headsets mit Entwickler-Berechtigungen. 
Entwickler-Berechtigungen sind erforderlich, um bestimmte Funktionen zu aktivieren, die zur Lösung von Verbindungsproblemen, Verwaltung von Geräteeinstellungen oder Fehlerbehebung bei VR-Anwendungen benötigt werden.

⚠️ **Meta**: Meta Hardware und Software (einschließlich MQDH) liegen außerhalb der Kontrolle von WPS. Meta-Updates können unerwartete Funktionalitätsänderungen in VR-Systemen verursachen. WPS überwacht Meta-Veröffentlichungen, um Benutzer über potenzielle Auswirkungen und Änderungen zu informieren.

## Voraussetzungen
- Eine Internetverbindung
- E-Mail-Konto-Anmeldedaten, die mit Ihrem VR-Setup verbunden sind *(können von WPS bereitgestellt werden)*
- Meta-Konto-Passwort *(kann von WPS bereitgestellt werden)*
- Smartphone mit 2FA-App-Funktionalität
- Smartphone mit installierter Meta Horizon Anwendung
- Erste Koordination mit WPS-Personal für erstmalige Anmeldung
- VR-Headsets

## Schneller Überblick (für erfahrene Benutzer)
1. Meta-Konto der Organisation wird zur WPS Developer-Gruppe hinzugefügt
2. Developer Mode für jedes Gerät in der Meta Horizon App aktiviert
3. Developer Mode in jedem Headset über Advanced Settings aktiviert

## Detaillierte Schritte

### Erste Entwickler-Autorisierung

1. **WPS-Personal bitten, das Meta-Konto Ihrer Organisation zur WPS Developer-Gruppe hinzuzufügen**
   - *Wenn WPS-Personal das Meta-Konto erstellt hat, das zur Registrierung der Headsets verwendet wird, kann dieser Schritt bereits abgeschlossen sein*
   - *Die folgenden Schritte werden am besten während eines Videoanrufs durchgeführt*
   - WPS-Personal die Meta-Konto-Informationen (**E-Mail-Adresse** oder **Benutzername**) senden und Developer-Zugang anfordern
   - WPS-Personal wird das Konto einladen, der Organisation als Entwickler beizutreten
   - E-Mail auf Einladung zum Meta Quest Developer Dashboard von Meta Horizons überprüfen
<div style="page-break-after: always;"></div>

2. **Einladung zur WPS Developer-Gruppe annehmen**
   - Einladungs-E-Mail öffnen
   - **"View Invitation"** klicken - ein Web-Link wird geöffnet - *(Wir empfehlen Chrome oder Firefox Browser für diesen Schritt)*

3. **Anmeldedaten eingeben**
   - **Continue with Email** klicken
   - E-Mail-Adresse eingeben, die mit Ihrem VR-Setup verbunden ist
   - **"Next"** klicken
   - **"Enter password instead"** wählen *(einfacher als E-Mail-Code)*
   - Ihr Meta-Konto-Passwort eingeben *(kann von WPS bereitgestellt werden)*
   - **"Log in"** klicken

4. **Zwei-Faktor-Authentifizierung (kann erforderlich sein)**
   - *Wenn Sie die Zwei-Faktor-Authentifizierung (2FA) für Ihr Meta-Konto noch nicht aktiviert haben, müssen Sie das jetzt tun*
   - *Siehe Meta Account Access and Security Setup Guide für Details zur Aktivierung von 2FA*
   - *Wenn Ihr Konto von WPS-Personal erstellt wurde, müssen Sie den Zugang koordinieren*

5. **Einladung annehmen und Autorisierung überprüfen** 
   - Einladung auf der Meta-Website annehmen
   - *Ein "accept invitation" Kontrollkästchen sollte auf der Webseite sichtbar sein*
   - Mit WPS-Personal bestätigen, dass die Einladung angenommen wurde und Developer-Berechtigungen autorisiert wurden

### Headset mit Meta Horizon Phone-Anwendung verbinden

6. **VR-Headset einschalten**
   - *Die folgenden Schritte setzen voraus, dass das VR-Headset initial eingerichtet wurde*
   - *Wenn dies nicht der Fall ist - siehe **VR Headset Initial Setup Guide** für erforderliche Schritte*
   - VR-Headset mit Internet verbinden
   - *Es ist am besten, nur ein Headset gleichzeitig eingeschaltet zu haben*

7. **Device Options öffnen**
   - Meta Horizon Phone-Anwendung öffnen
   - *Das für das VR-Headset verwendete Konto muss dasselbe sein wie für das Meta Horizon Konto*
   - Die Meta Horizon App zeigt den Konto-Avatar und ein Hamburger-Menü *(drei horizontale Balken)* auf der rechten Seite.
   - Das Hamburger-Menü öffnen
   - Unter **Device Management** auf **Devices** klicken
<div style="page-break-after: always;"></div>

8. **Mit Gerät verbinden**
   - *Sie sehen möglicherweise mehrere aufgelistete Geräte* 
   - Ein Gerät sollte einen grünen Kreis zeigen und als **"Nearby"** aufgelistet sein
   - Auf das **Nearby** Gerät klicken
   - Ein neuer Bildschirm zeigt Gerätedetails und vier **Manage your device** Optionen

9. **Developer Mode aktivieren**
    - Auf **Headset Settings** klicken - *(kann durch Manage profiles Benachrichtigung verdeckt sein)*
    - Sie sollten eine Anzahl von Optionen unter **Headset settings** sehen
    - Auf **Developer Mode** klicken
    - Den **Developer Mode** Schalter aktivieren

### Developer-Einstellungen auf VR-Headset aktivieren

- *Sie werden das VR-Headset für die nächsten Schritte tragen*
- *Für detaillierte Anweisungen zum Zugriff auf das Settings-Menü siehe - **Recommended Headset Settings***

10. **Advanced Settings Menü öffnen**
    - Das **Quick Settings** Menü öffnen, indem Sie auf die Zeit/WiFi/Batterie-Anzeige klicken
    - **Settings** oben rechts klicken
    - Links nach unten scrollen, um **Advanced Settings** zu finden
    - Auf die **Advanced Setting** Option klicken

11. **Developer Mode aktivieren**
    - Nach unten scrollen, um den **Developer** Bereich zu finden
    - **Enable Developer Settings** aktivieren
    - Eine zusätzliche Liste von Optionen sollte erscheinen
    - **Enable MTP Notification** aktivieren
    - **Physical Link Features** deaktivieren
    - **Link Auto-Connect** deaktivieren

## Fehlerbehebung

**Keine Einladungs-E-Mail von WPS erhalten**
- Mit WPS-Personal vor dem Senden einer Folge-E-Mail koordinieren
- Die an WPS-Personal gesendete E-Mail-Adresse überprüfen
- Ihren Spam-Ordner überprüfen

**Kann sich nicht in Meta-Konto einloggen**
- Die korrekte E-Mail für das Meta-Konto überprüfen
- Beim Einloggen E-Mail-Code statt Passwort verwenden, um Konto-Übereinstimmung zu bestätigen
- Sicherstellen, dass das Passwort für das Konto korrekt ist
- Wenn das Meta-Konto von WPS erstellt wurde, weitere Fehlerbehebung mit Personal koordinieren
<div style="page-break-after: always;"></div>

**Zwei-Faktor-Authentifizierung Probleme**
- Wenn das Konto von WPS erstellt wurde, 2FA-Zugang koordinieren oder erhalten *(normalerweise Google Authenticator)*
- Sicherstellen, dass Sie die korrekte Methode für 2FA wählen *(falls mehrere Optionen existieren)*
- WPS-Personal kann nicht bei 2FA per Telefon oder SMS helfen

**Kann Einladung zum Beitritt zur Organisation nicht annehmen**
- Sicherstellen, dass das Meta-Konto mit der E-Mail-Adresse auf der Einladung übereinstimmt
- Versuchen, die Einladung mit Chrome oder Firefox Browsern anzunehmen - *(Safari hat in der Vergangenheit Probleme verursacht)*

**Kann Gerät in Meta Horizon App nicht finden**
- Sicherstellen, dass sowohl VR-Headset als auch Telefon dieselbe Internetquelle verwenden
- Überprüfen, dass VR-Headset und Telefon mit demselben Meta-Konto angemeldet sind
- Sowohl Headset als auch Meta Horizon App neu starten
- Um mögliche Verwirrung zu reduzieren, sicherstellen, dass nur ein VR-Headset eingeschaltet ist

**Mehrere Geräte zeigen als **Nearby** in Meta Horizon App**
- Andere nahegelegene Geräte ausschalten, um das Setup zu vereinfachen
- Seriennummern abgleichen *(Seriennummer befindet sich am linken Bügel des Headsets)*
- *Seriennummer befindet sich innen am linken Bügel - Quest 3*
- *Seriennummer befindet sich außen am linken Bügel, unter der Kopfband-Abdeckung - Quest 2*

**Developer Mode nicht verfügbar in Meta Horizon App**
- Sicherstellen, dass das Meta-Konto zur WPS-Organisation als Entwickler hinzugefügt wurde
- Aus Meta Horizon App ausloggen und wieder einloggen
- Überprüfen, dass das korrekte Meta-Konto in der Meta Horizon App verwendet wird

**Developer Mode Schalter bleibt nicht aktiviert in Meta Horizon App**
- Überprüfen, dass das Meta-Konto zur WPS-Organisation als Entwickler hinzugefügt wurde
- Sicherstellen, dass das korrekte Meta-Konto in der Meta Horizon App verwendet wird
- VR-Headset auf Warndialog oder Aktionsnachrichten überprüfen

**Developer Settings nicht in Advanced Settings auf Headset sichtbar**
- Überprüfen, dass das Headset Developer Mode in der Meta Horizon App aktiviert hat
- VR-Headset neu starten
- Headset auf ausstehende Updates überprüfen - *(alle ausstehenden Updates anwenden)*
<div style="page-break-after: always;"></div>

## Wichtige Hinweise

⚠️ **WPS Organisation Einladung**: Koordination dieses Schritts ist vor allen weiteren Developer-Konto-Einstellungen erforderlich

⚠️ **Konto-Konsistenz**: Meta-Konten müssen zwischen der Meta Horizon Anwendung und dem VR-Headset übereinstimmen.