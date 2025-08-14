# Quest VR Headset Setup Anleitung

## Zweck & Kontext
Diese Anleitung bietet die erforderlichen Schritte zur erstmaligen Einrichtung eines Quest VR-Headsets. 
WPS hat möglicherweise einige benötigte Konten als Teil ihres internen VR-Partnerprogramms erstellt. Fragen Sie WPS-Personal, wenn Sie unsicher sind, welche Konten Ihre Organisation benötigt.
Kontoerstellung durch WPS erfolgt, um reibungslosen VR-Betrieb zu erleichtern und unsere Fähigkeit zur technischen Unterstützung zu erhöhen. 
Konten, die ohne Hilfe von WPS-Personal erstellt wurden, können von WPS-Personal während technischer Support-Sitzungen nicht aufgerufen werden.

⚠️ **Meta**: Meta Hardware und Software (einschließlich MQDH) liegen außerhalb der Kontrolle von WPS. Meta-Updates können unerwartete Funktionalitätsänderungen in VR-Systemen verursachen. WPS überwacht Meta-Veröffentlichungen, um Benutzer über potenzielle Auswirkungen und Änderungen zu informieren.

## Voraussetzungen
- Eine WiFi-Internetverbindung
- E-Mail-Konto-Anmeldedaten, die mit Ihrem VR-Setup verbunden sind *(können von WPS bereitgestellt werden)*
- Smartphone mit 2FA-App-Funktionalität
- Smartphone mit installierter Meta Horizon Anwendung
- Erste Koordination mit WPS-Personal für erstmalige Anmeldung
- VR-Headsets

## Schneller Überblick (für erfahrene Benutzer)
1. Meta-Konto wird für Organisation erstellt *(kann von WPS bereitgestellt werden)*
2. Benutzer meldet sich in Meta Horizon Phone-App an
3. Developer-Modus wird für Headset aktiviert
4. Empfohlene Einstellungen werden auf Headset angewendet
5. WildXR und Auto Launch *(falls gewünscht)* werden auf Headset installiert
6. Headset wird bei WildXR-Website für Remote-Bereitstellung registriert
7. Videos werden heruntergeladen oder sideloadet, um WildXR-Leistung zu verbessern

## Detaillierte Schritte

### Meta-Kontoerstellung

- *Wenn WPS-Personal das Meta-Konto erstellt hat, das zur Registrierung von Headsets verwendet wird, kann dieser Schritt bereits abgeschlossen sein*

1. **Zu Meta navigieren**
   - Webbrowser öffnen und zu `meta.com` gehen
<div style="page-break-after: always;"></div>

2. **Anmeldung aufrufen**
   - **Account-Symbol** *(Personensilhouette)* oben rechts klicken
   - **"Sign up or log into a Meta account"** auswählen
   - **"Continue with email"** wählen

3. **Anmeldedaten eingeben**
   - **Continue with Email** klicken
   - E-Mail-Adresse eingeben, die mit Ihrem VR-Setup verbunden ist
   - **"Next"** klicken
   - **"Create new account"** wählen
   - Die angeforderten Details für Kontoerstellung nach Bedarf eingeben
   - *Beim Hinzufügen eines Geburtsdatums - WildXR wird für Alter 13+ empfohlen - ein Datum eingeben, das diese Anforderung erfüllt*
   - Ein Passwort für Ihr Konto wählen *(WPS-Personal hat keinen Zugang zu Ihrem Passwort)*
   - Ihre Kontodetails (E-Mail und Passwort) für zukünftige Nutzung sichern
   - **"Next"** klicken

4. **Anmelde-Persistenz verwalten (optional)**
   - Wählen, ob Anmeldedaten auf diesem Computer gespeichert werden sollen
   - *Das Speichern von Anmeldedaten speichert nur E-Mail- und Passwort-Informationen*
   - *Sicherheitsimplikationen gespeicherter Anmeldedaten auf gemeinsam genutzten Computern berücksichtigen*

5. **Kontodetails überprüfen** 
   - Die eingegebenen Kontodetails überprüfen
   - *Das Kontrollkästchen für Marketing-E-Mails deaktivieren*
   - **"Create account"** klicken

6. **Kontoerstellung bestätigen**
   - Das E-Mail-Konto öffnen, das mit Ihrem Meta-Konto verbunden ist
   - Bestätigungscode aus der aktuellen Meta-E-Mail kopieren
   - Bestätigungscode in das entsprechende Feld eingeben
   - **"Next"** klicken

7. **Konto-Dashboard aufrufen**
   - Sie kehren zur `meta.com` Hauptseite zurück
   - **Account-Symbol** erneut klicken, um auf Kontofunktionen zuzugreifen *(Symbol ist jetzt ein Kreis mit einem Buchstaben oder Logo)*
   - **"Accounts Center"** für Haupt-Dashboard auswählen
<div style="page-break-after: always;"></div>

### Zwei-Faktor-Authentifizierung

- *Jetzt ist ein guter Zeitpunkt, Zwei-Faktor-Authentifizierung einzurichten, da sie später benötigt wird*
- *Wenn Ihr Konto von WPS-Personal bereitgestellt wurde, kann dieser Schritt bereits abgeschlossen sein*

8. **Zu Sicherheitseinstellungen navigieren**
   - Im **Accounts Center** auf **"Password and security"** klicken
   - **"Two-factor authentication"** auswählen
   - Ihr Profil wählen
   - **"Authentication app"** auswählen und zu Schritt 9 weitergehen *(empfohlen)*
   - **"SMS or WhatsApp"** auswählen und zu Schritt 13 weitergehen

### 2FA über Authentication App

9. **Authenticator-App installieren (Empfohlen)**
   - Eine Authenticator-Anwendung ermöglicht Verwaltung durch mehrere Personen
   - Google Authenticator (empfohlen) oder Authy herunterladen
   - Verfügbar sowohl auf iOS als auch Android
   - Mehrere Mitarbeiter können denselben Authenticator für gemeinsames Konto verwenden
   - SMS- oder WhatsApp-Authentifizierung ist nur für eine Telefonnummer verfügbar

10. **Neues Gerät hinzufügen**
    - **"Add"**-Schaltfläche klicken
    - *QR-Code und Setup-Schlüssel erscheinen*
    - *Zu Ihrem Telefon für die nächsten Schritte wechseln*

11. **Authenticator-App konfigurieren**
    - Authenticator-App auf dem Telefon öffnen
    - Neues Konto hinzufügen *(+ Symbol)*
    - **"Scan QR code"** oder **"Enter setup key"** wählen
    - QR-Code von der Meta-Website scannen

12. **Setup abschließen**
    - Beschreibenden Namen für dieses Gerät eingeben *(z.B. WPSVR GAuth oder Alex's GAuth)*
    - 6-stelligen Code aus der Authenticator-App eingeben
    - **"Done"** klicken
    - *Gerät erscheint jetzt in der 2FA-Geräteliste*
<div style="page-break-after: always;"></div>

### 2FA über SMS oder WhatsApp

- *Nur eine Telefonnummer ist für 2FA über SMS oder WhatsApp erlaubt*
- *Dies wird die Fähigkeit zur Fehlerbehebung bestimmter Probleme einschränken, sollten sie auftreten*

13. **Telefonnummer hinzufügen**
    - Ländercode bei Bedarf ändern *(standardmäßig Vereinigte Staaten)*
    - Telefonnummer eingeben
    - **"Next"** klicken
    - Den 6-stelligen Code eingeben, der an das Gerät gesendet wurde
    - **"Done"** klicken

### Meta Horizon App-Bereitstellung

14. **Meta Horizon Phone-Anwendung öffnen**
    - **Continue with email** wählen
    - Die E-Mail eingeben, die zur Erstellung des Organisations-Meta-Kontos verwendet wurde *(Kann von WPS bereitgestellt werden)*
    - **"Next"** klicken
    - **"Enter password instead"** wählen *(einfacher als E-Mail-Code)*
    - Ihr Meta-Konto-Passwort eingeben *(kann von WPS bereitgestellt werden)*

15. **Konto über 2FA verifizieren *(kann erforderlich sein)***
    - 2FA-Methode aus Dropdown auswählen
    - **"Next"** klicken
    - Authenticator-Anwendung öffnen oder nach SMS/WhatsApp-Nachricht suchen
    - 6-stelligen Code eingeben
    - **"Next"** klicken

16. **Anmelde-Persistenz verwalten (optional)**
    - Wählen, ob Anmeldedaten auf diesem Computer gespeichert werden sollen
    - *Das Speichern von Anmeldedaten speichert nur E-Mail- und Passwort-Informationen*
    - *Sicherheitsimplikationen gespeicherter Anmeldedaten auf gemeinsam genutzten Computern berücksichtigen*
  
### Meta Horizon Konto einrichten

- *Das Meta Horizon Konto wird ausschließlich für Metas VR-Raum verwendet*
- *Einige Optionen sind für andere Meta Horizon Benutzer sichtbar*

17. **Meta Horizon Benutzername wählen**
    - *Dieser Benutzername ist für andere Meta Horizon Benutzer sichtbar*
    - Einen akzeptierten Benutzernamen eingeben *(ein grünes Häkchen zeigt an, dass der Benutzername gültig ist)*
    - **"Continue"** klicken
    - Sie werden zum Meta Horizon Dashboard geleitet

### Headset-Setup

18. **Headset einschalten**
    - Verpackungsmaterial vom Headset entfernen
    - Batterieschoner von Hand-Controllern entfernen
    - **Quest 2**: **Power-Taste** auf der rechten Seite drücken
    - **Quest 3 & Quest 3s**: **Power-Taste** auf der linken Seite drücken
    - VR-Headset aufsetzen

19. **Erste Einführung und WiFi-Verbindung**
    - Den Bildschirmaufforderungen im VR-Headset folgen
    - *Gelegentlich installieren Hand-Controller ein Update, das sie für kurze Zeit funktionsunfähig macht*
    - Ihr Headset mit Ihrer WiFi-Internetverbindung verbinden
    - *WPS empfiehlt, die WiFi-Details auf Ihrem Headset einzugeben*
    - *Falls Ihr WiFi-Netzwerk versteckt ist, zu Schritt #20 gehen*
    - Ihr Headset kann Firmware-Updates anwenden
    - Ihr Headset angeschlossen lassen, während Updates heruntergeladen werden
    - *Ihr Headset kann anzeigen, dass Sie das Setup in der Meta Horizon Phone-App fortsetzen können*
    - ⚠️ **WPS empfiehlt dies nicht und schlägt vor, zu warten, bis das Headset Ihren Kopplungscode anzeigt**

### Verstecktes WiFi-Netzwerk hinzufügen

20. **Verstecktes Netzwerk zu WiFi hinzufügen**
    - *Sie benötigen möglicherweise Hilfe von Ihrer Unternehmens-IT-Abteilung, wenn Sie ein robustes WiFi-Sicherheitsprogramm haben*
    - Im WiFi-Fenster nach unten zu **"+ New Network >"** scrollen
    - Klicken, um ein neues Netzwerk hinzuzufügen
    - **"Advanced"** klicken
    - Unter **"Hidden Network"** angezeigten Wert zu **"Yes"** ändern
    - Generell sind die Standardwerte für den Rest des Advanced-Menüs ausreichend
    - *Falls Sie weiterhin Probleme haben, sich mit einem versteckten WiFi-Netzwerk zu verbinden, müssen Sie möglicherweise Ihre Unternehmens-IT-Abteilung kontaktieren*
    - **"Confirm"** klicken
    - Falls Ihr WiFi-Netzwerk ein Passwort hat, verwendet es höchstwahrscheinlich **WPA/WPA2-Personal** als **"Security"**-Einstellung
    - Die restlichen Details Ihres WiFi-Netzwerks eingeben
    - **"Connect"** klicken, um WiFi-Setup abzuschließen und sich mit dem Netzwerk zu verbinden
<div style="page-break-after: always;"></div>

### Headset mit Meta Horizon Phone-App koppeln

21. **Zu Devices in Horizon App navigieren**
    - Ihre Meta Horizon Phone-App öffnen
    - Die Meta Horizon App zeigt den Konto-Avatar und ein Hamburger-Menü *(drei horizontale Balken)* auf der rechten Seite
    - Das Hamburger-Menü öffnen
    - Unter **Device Management** auf **Devices** klicken

22. **Headset mit Meta Horizon App koppeln**
    - Die **Pair New Headset** Option finden und darauf klicken
    - Das korrekte Modell des Meta-Headsets auswählen
    - *Sie werden möglicherweise aufgefordert, einen Avatar zu erstellen - dieser Schritt ist jetzt von Meta erforderlich*
    - *Dieser Avatar ist für andere Meta Horizon Benutzer sichtbar*
    - Einen Avatar erstellen und **"Continue"** klicken
    - Ihr Headset sollte einen fünfstelligen Code anzeigen
    - Den fünfstelligen Code eingeben, wenn dazu aufgefordert
    - **"Continue"** klicken, wenn der erfolgreiche Kopplungsbildschirm angezeigt wird

### **Bedingungen von Meta akzeptieren**

23. **Haftungsausschlüsse in Meta Horizon App akzeptieren**
    - **"Continue"** bei den Sicherheitsrichtlinien klicken
    - **"Don't Share"** oder **"Share"** bei der Anfrage zum Teilen zusätzlicher Daten klicken
    - **"Not now"** bei der Anfrage Enable hand and body tracking klicken
    - **"Skip"** bei dem Start 3-month trial Angebot klicken *(Dieser Bildschirm kann vorhanden sein oder nicht)*
    - **"Skip"** bei Add a payment method klicken
    - **"Close"** beim **You're all set!** Bildschirm klicken

### **Headset-Setup abschließen**

24. **Headset-Einführung abschließen**
    - VR-Headset für eine kurze Einführung in Ihr Headset von Meta aufsetzen
    - Bildschirmaufforderungen folgen
    - An Tutorials nach Wunsch teilnehmen *(Das Überspringen von Tutorials beeinflusst das Headset-Setup nicht)*
    - *Sie müssen das Headset während der Einführung aufbehalten*
    - Nach der Einführung wird Ihnen das Horizon-Dashboard gezeigt
<div style="page-break-after: always;"></div>

## Nächste Schritte

**Developer Mode aktivieren**
- Der **Developer Mode Setup** Anleitung folgen
- Developer-Modus wird benötigt, um einige empfohlene Einstellungen anzuwenden
- Developer-Modus wird benötigt, um die erforderliche Sicherheitsgrenze zu entfernen

**Empfohlene Headset-Einstellungen anwenden**
- Der **Recommended Headset Settings** Anleitung folgen

**Unbenötigte Software entfernen**
- Der **Library Management** Anleitung folgen

## Fehlerbehebung

**Kann nicht auf Meta-Konto zugreifen:**
- E-Mail-Adresse für Ihr VR-Setup überprüfen *(Falls von WPS bereitgestellt)*
- WPS für Passwort-Hilfe kontaktieren

**Bestätigungscode von Meta fehlt:**
- Bestätigungscodes können durch langsame oder intermittierende Internetverbindungen verzögert werden
- **Spam**-Ordner in Ihrem E-Mail-Browser überprüfen
- Sicherstellen, dass Sie im korrekten E-Mail-Konto schauen *(Konto kann von WPS bereitgestellt worden sein)*

**2FA-Geräte existieren bereits für Meta-Konto**
- Wenn Ihr Meta-Konto von WPS-Personal erstellt wurde, ist es mit 2-3 2FA-Geräten vorbelegt
- Eines dieser Geräte sollte dem von WPS bereitgestellten E-Mail-Konto entsprechen
- Andere 2FA-Geräte werden von WPS-Personal verwendet, um bei der Fehlerbehebung zu helfen, falls Probleme auftreten

**"Add"-Schaltfläche für 2FA ausgegraut:**
- Konto hat möglicherweise maximale Anzahl verknüpfter Geräte
- WPS kontaktieren, um ungenutzte Geräte zu entfernen
- Einige Kontotypen haben Gerätebegrenzungen
<div style="page-break-after: always;"></div>

**Kann Meta Horizon Anwendung nicht finden:**
- Die Meta Horizon Anwendung ist zum Download im Apple App Store oder Google Play Store verfügbar
- Falls Sie ein von WPS bereitgestelltes Telefon verwenden, sollte die App vorhanden sein - nach Horizon suchen
- Die Meta Horizon App ist möglicherweise nicht auf der ersten Seite Ihres Telefons platziert
- Die Telefonsuchfunktion verwenden, um Meta Horizon zu finden und an einen offensichtlichen Ort zu verschieben

**Kann sich nicht in Meta Horizon App anmelden**
- Sicherstellen, dass Sie dasselbe Konto verwenden, das in den Meta-Kontoerstellungsschritten verwendet wurde
- Sicherstellen, dass Sie "Enter Password instead" gewählt haben, wenn Sie versuchen, ein Passwort einzugeben
- Ihr Passwort doppelt überprüfen, es wird das Meta-Konto-Passwort sein, nicht das E-Mail-Konto-Passwort für Horizon-Anmeldung

**2FA schlägt für Meta Horizon App fehl**
- Sicherstellen, dass Sie das korrekte 2FA-Konto für Autorisierung verwenden
- Falls Sie SMS/WhatsApp für Autorisierung verwenden, ist nur eine Telefonnummer mit dem Konto verbunden
- 2FA-Codes sind durchschnittlich 30 Sekunden gültig, warten Sie, bis ein neuer Code generiert wird, und versuchen Sie sich anzumelden

**Meta erlaubt meinen gewünschten Benutzernamen nicht**
- Meta beschränkt das Format von Benutzernamen, um Eindeutigkeit zu gewährleisten
- Den Benutzernamen bearbeiten, um Unterstriche oder Zahlen einzuschließen
- Denken Sie daran, dass dieser Benutzername für andere Meta Horizon Benutzer sichtbar werden kann

**Headset erkennt Hand-Controller nicht**
- Beim ersten Hochfahren eines Headsets können Firmware-Updates auf Hand-Controller angewendet werden, die sie temporär funktionsunfähig machen
- 2-3 Minuten warten, bevor Sie Hand-Controller erneut verwenden
- Frische Batterien in die Hand-Controller einsetzen
- Sehr selten können andere Probleme mit Hand-Controllern auftreten - Eine Hilfssitzung mit WPS-Personal für zusätzliche Anleitung planen

**Headset kann sich nicht mit WiFi verbinden**
- Sicherstellen, dass Ihre IT-Abteilung nicht erkannten Geräten erlaubt, sich mit dem WiFi-Kanal Ihres Unternehmens zu verbinden
- Das VR-Gerät bei Ihrer IT-Abteilung registrieren, falls nötig
- Sicherstellen, dass Sie das korrekte WiFi-Netzwerk und Passwort in die entsprechenden Felder eingegeben haben
- Falls Ihr WiFi-Netzwerk versteckt ist, zu Schritt #20 gehen - *Sie benötigen möglicherweise Hilfe von Ihrer IT-Abteilung bei versteckten Netzwerken*

**Kann Devices-Menü in Horizon App nicht finden**
- Sicherstellen, dass Sie auf der Hauptseite der Meta Horizon App sind - *Sie sollten Ihren Benutzer-Avatar und Namen sehen*
- Horizon App schließen und Anwendung erneut öffnen, um die Hauptseite zu laden
- Das Hamburger-Menü auf der rechten Seite der Anwendung identifizieren - Symbol sind drei gestapelte horizontale Balken
- Das Hamburger-Menü öffnen und nach unten scrollen, um den **"Device management"** Bereich zu sehen
- Prüfen, ob ausstehende Updates für die Meta Horizon App oder Ihr Telefon-Betriebssystem vorhanden sind

**Gezwungen, einen Avatar zu erstellen**
- Meta zwingt Benutzer jetzt, einen Avatar für ihren Benutzer zu erstellen
- Falls Sie die meisten sozialen Medien deaktiviert oder blockiert haben, wird dieser Avatar für andere Benutzer minimal sichtbar sein
- Falls Sie Ihre Datenschutzeinstellungen überprüfen möchten, öffnen Sie das Hamburger-Menü und scrollen nach unten zu **"Privacy and security"**, um den **"Privacy settings"** Bereich zu öffnen

**5-stelliger Kopplungscode wird nicht akzeptiert**
- Es kann eine Weile dauern, bis die Headset-Kopplung abgeschlossen ist, abhängig von der Internetkonnektivität
- Sicherstellen, dass Ihr Telefon und Headset im gleichen WiFi-Netzwerk sind
- Den im Headset angezeigten Code und den in die Meta Horizon App eingegebenen Code doppelt überprüfen

## Wichtige Hinweise

⚠️ **Meta Horizon App**: Meta erfordert die Verwendung der Telefon-Anwendung **Meta Horizon** zur Einrichtung von Quest-Headsets.

⚠️ **Avatar-Erstellung**: Meta erfordert die Erstellung eines virtuellen Avatars. Dieser Avatar ist an einigen Stellen im VR-"Metaverse" sichtbar, abhängig von den Datenschutzeinstellungen.

⚠️ **Schwierigkeiten mit 2FA**: Wenn Meta nach einer 2FA-Methode fragt, können mehrere Optionen präsentiert werden. Nur eine Telefonnummer kann für SMS/WhatsApp-Benachrichtigungen zur Authentifizierung verwendet werden. Sicherstellen, dass Sie das korrekte Konto für 2FA auswählen. 2FA-Codes dauern generell 30 Sekunden, falls ein Code kurz vor dem Ablauf steht, auf einen neuen warten.

⚠️ **Internet-Netzwerke**: Falls Ihr Headset und Telefon nicht mit demselben WiFi-Netzwerk verbunden sind, ist es möglicherweise nicht möglich, Ihr Headset mit der App zu koppeln.