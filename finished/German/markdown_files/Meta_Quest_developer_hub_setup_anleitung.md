# Meta Quest Developer Hub Setup Anleitung

## Zweck & Kontext
Diese Anleitung richtet das Meta Quest Developer Hub (MQDH) auf Ihrem Computer ein, das als Grundlage für erweiterte VR-Headset-Verwaltung dient. MQDH ermöglicht es Ihnen, benutzerdefinierte Anwendungen wie WPS Auto Launch zu installieren, Entwicklereinstellungen zu verwalten und erweiterte Fehlerbehebung durchzuführen. Dies ist ein einmaliger Setup-Prozess, der die Entwicklungsumgebung schafft, die für WildXR-Deployments benötigt wird.

⚠️ **Meta**: Meta Hardware und Software (einschließlich MQDH) liegen außerhalb der Kontrolle von WPS. Meta-Updates können unerwartete Funktionalitätsänderungen in VR-Systemen verursachen. WPS überwacht Meta-Veröffentlichungen, um Benutzer über potenzielle Auswirkungen und Änderungen zu informieren.

## Voraussetzungen
- Windows oder Mac Computer mit Internetzugang
- Meta-Konto-Anmeldedaten für Ihr VR-Setup (einschließlich 2FA-Zugang)
- Administratorrechte zur Installation von Software auf Ihrem Computer
- Meta Quest Headset mit aktiviertem Developer-Modus
- USB-Kabel, das mit Ihrem Quest-Headset kompatibel ist
- Headset und Computer mit demselben WiFi-Netzwerk verbunden

## Schneller Überblick (für erfahrene Benutzer)
1. MQDH von der Meta-Entwicklerseite herunterladen und installieren
2. MQDH starten und mit Meta-Konto authentifizieren
3. Erste Einrichtung abschließen und Entwicklerbedingungen akzeptieren
4. Headset verbinden und USB-Debugging-Autorisierung einrichten
5. Vollständige Funktionalität mit verbundener Headset-Verwaltung überprüfen

## Detaillierte Schritte
*Nur das Windows-Betriebssystem wird in den folgenden Schritten abgedeckt.*
*Eine Apple iOS-Version von MQDH ist über den unten stehenden Link verfügbar*

### MQDH herunterladen und installieren

1. **Zu Meta Developer Downloads navigieren**
   - Webbrowser öffnen und zur Meta-Entwicklerseite gehen
   - **Windows**: https://developers.meta.com/horizon/downloads/package/oculus-developer-hub-win/ besuchen
   - **Mac**: https://developers.meta.com/horizon/downloads/package/oculus-developer-hub-mac/ besuchen
<div style="page-break-after: always;"></div>

2. **MQDH-Paket herunterladen**
   - "Download"-Schaltfläche in der oberen rechten Ecke klicken
   - Lizenzbedingungen akzeptieren, wenn dazu aufgefordert
   - Download-Speicherort wählen und "Save" klicken
   - Datei wird als "Meta-Quest-Developer-Hub.zip" heruntergeladen

3. **MQDH extrahieren und installieren**
   - Zum Speicherort der heruntergeladenen Zip-Datei navigieren
   - Rechtsklick auf "Meta-Quest-Developer-Hub.zip"
   - "Extract All" auswählen und Ziel wählen (Standardspeicherort funktioniert gut)
   - "Extract" klicken, um Dateien zu entpacken
   - Extrahierten Ordner öffnen und "Meta-Quest-Developer-Hub.exe" lokalisieren
   - Auf die ausführbare Datei doppelklicken, um Installation zu beginnen

4. **Installationsprozess abschließen**
   - Anweisungen des Installationsassistenten folgen
   - Standard-Installationsort akzeptieren, es sei denn, spezifische Anforderungen bestehen
   - Wenn Installation abgeschlossen ist, "Run MQDH" Kontrollkästchen ankreuzen
   - "Finish" klicken, um Installation abzuschließen und Anwendung zu starten

### Erste MQDH-Authentifizierung

5. **MQDH-Setup beginnen**
   - Anwendung öffnet sich zum Willkommensbildschirm
   - "Continue" unten rechts klicken
   - "Log in with a Meta account" Option auswählen
   - System öffnet Browserfenster für Authentifizierung

6. **Mit Meta-Konto authentifizieren**
   - Browser leitet zur Meta-Anmeldeseite weiter
   - "Continue with email" Option wählen
   - E-Mail-Adresse eingeben, die mit Ihrem VR-Setup verbunden ist *(kann von WPS bereitgestellt werden)*
   - "Next" klicken, um fortzufahren

7. **Passwort-Authentifizierung abschließen**
   - "Enter password instead" auswählen *(einfacher als E-Mail-Code)*
   - Ihr Meta-Konto-Passwort eingeben *(kann von WPS bereitgestellt werden)*
   - "Log in" klicken, um zu authentifizieren
<div style="page-break-after: always;"></div>

8. **2FA-Überprüfung durchführen**
   - System zeigt 2FA-Methoden-Dropdown an
   - Methode auswählen, die von WPS-Personal spezifiziert wird
   - "Next" klicken, um fortzufahren
   - 6-stelligen Authentifizierungscode eingeben, wenn dazu aufgefordert
   - "Next" klicken, um 2FA-Überprüfung abzuschließen

9. **Anmelde-Persistenz verwalten (optional)**
   - Wählen, ob Anmeldedaten auf diesem Computer gespeichert werden sollen
   - *Das Speichern von Anmeldedaten speichert nur E-Mail- und Passwort-Informationen*
   - *2FA-Überprüfung wird weiterhin für zukünftige Anmeldesitzungen erforderlich sein*
   - *Sicherheitsimplikationen gespeicherter Anmeldedaten auf gemeinsam genutzten Computern berücksichtigen*

### MQDH-Setup abschließen

10. **Entwicklerbedingungen akzeptieren**
    - MQDH zeigt Terms and Documents Bildschirm an
    - Entwicklervereinbarungsbedingungen überprüfen
    - "Continue" klicken, um zu akzeptieren und fortzufahren

11. **ADB-Pfad-Warnung behandeln (falls angezeigt)**
    - System kann Warnung über mehrere ADB-Pfade anzeigen
    - Diese Warnung ist typischerweise sicher zu ignorieren
    - "Cancel" klicken oder Warnung schließen, ohne ADB-Einstellungen zu ändern
    - MQDH wird geeignete Standardwerte für Ihr System verwenden

12. **Erfolgreiche Installation überprüfen**
    - MQDH-Hauptschnittstelle sollte jetzt sichtbar sein
    - Linke Seitenleiste zeigt Geräteverwaltungssymbole
    - Obere Symbolleiste zeigt Kontoinformationen an
    - Anwendung ist bereit für Headset-Verbindungen und App-Verwaltung

### Ihr Headset verbinden und USB-Debugging einrichten

13. **Physische Verbindung herstellen**
    - VR-Headset vollständig einschalten
    - USB-Kabel zwischen Headset und Computer mit MQDH verbinden
    - Sicherstellen, dass Kabelverbindung an beiden Enden sicher ist
    - Headset sollte während des gesamten Verbindungsprozesses eingeschaltet bleiben
<div style="page-break-after: always;"></div>

14. **Auf automatische Geräteerkennung prüfen**
    - In MQDH auf das Headset-Symbol in der linken Seitenleiste klicken
    - Nach Ihrem Gerät suchen, das als "Active" im Devices-Bereich aufgelistet ist
    - Wenn Gerät als Active angezeigt wird, direkt zu Schritt 18 für USB-Debugging gehen
    - Wenn Gerät nicht angezeigt wird oder als inaktiv angezeigt wird, mit Geräte-Setup fortfahren

15. **Neues Geräte-Setup einleiten (falls nötig)**
    - Dropdown-Menü in der oberen rechten Ecke von MQDH klicken
    - "Set Up New Device" aus den Menüoptionen auswählen
    - Sie müssen möglicherweise nach unten scrollen, um diese Option zu finden
    - "Next" klicken, um Gerätekonfigurationsassistent zu beginnen

16. **Geräteverbindung konfigurieren**
    - Ihr spezifisches Headset-Modell aus verfügbaren Optionen auswählen
    - MQDH scannt nach kompatiblen Geräten in Ihrem Netzwerk
    - Ihr Headset aus der "Choose Device" Liste wählen, wenn es erscheint
    - "Next" klicken, um mit Kontoverifizierung fortzufahren

17. **Geräte-Setup abschließen**
    - Bestätigen, dass korrektes Meta-Konto auf der Account-Seite angezeigt wird
    - "Next" klicken, um zur Netzwerkkonfiguration zu gelangen
    - Geeignetes WiFi-Netzwerk für Ihre Deployment-Umgebung auswählen
    - "Next" klicken, um mit Developer-Modus-Überprüfung fortzufahren
    - "Enable Developer Mode" Schalter aktivieren, falls nicht bereits aktiv
    - "Next" klicken, um erstes Geräte-Setup abzuschließen

18. **USB-Debugging-Zugang autorisieren**
    - VR-Headset aufsetzen, um Systemaufforderungen zu sehen
    - Nach "Allow USB debugging?" Dialogfeld suchen
    - Dieser Dialog autorisiert Ihren Computer, Anwendungen zu installieren und auf Systemfunktionen zuzugreifen
    - Sie müssen möglicherweise in der virtuellen Umgebung umherschauen, um den Dialog zu finden

19. **Permanente Debugging-Berechtigungen gewähren**
    - "Always allow from this computer" Schaltfläche im Dialog klicken
    - Diese Schaltfläche kann am unteren Rand des Dialogfensters teilweise verdeckt sein
    - Die "Always allow" Option verhindert wiederholte Autorisierungsanfragen
    - Headset nach Bestätigung der Autorisierung abnehmen
<div style="page-break-after: always;"></div>

20. **Setup-Überprüfung abschließen**
    - Zu MQDH auf Ihrem Computer zurückkehren
    - "Finish" klicken, wenn Geräte-Setup-Assistent noch geöffnet ist
    - Ihr Headset sollte jetzt als "Active" in der Geräteliste erscheinen
    - USB-Debugging ist jetzt dauerhaft für dieses Computer-Headset-Paar autorisiert

## Developer Hub Komponenten verstehen

**Warum MQDH essentiell ist:**
Meta Quest Developer Hub dient als Brücke zwischen Ihrem Computer und VR-Headsets für erweiterte Verwaltungsaufgaben. Während der grundlegende Headset-Betrieb über die Standard-Meta-App funktioniert, schaltet MQDH Entwicklerfähigkeiten frei, die für benutzerdefinierte Anwendungsbereitstellung wie WPS Auto Launch essentiell sind. Stellen Sie es sich vor wie den Unterschied zwischen der Verwendung eines Smartphones als Verbraucher versus Entwicklerzugang zu haben, um benutzerdefinierte Apps zu installieren und Systemverhalten zu ändern.

**ADB-Integration:**
MQDH integriert sich mit Android Debug Bridge (ADB), dem zugrundeliegenden Kommunikationsprotokoll für die Verwaltung Android-basierter Geräte. Meta Quest Headsets laufen auf einem modifizierten Android-System, daher bietet ADB die technische Grundlage für die Installation benutzerdefinierter Anwendungen, den Zugriff auf Systemeinstellungen und die Durchführung erweiterter Fehlerbehebung. Die ADB-Warnung, die Sie während des Setups sehen könnten, bezieht sich darauf, sicherzustellen, dass MQDH die korrekten Kommunikationswege verwendet.

**Kontoanforderungen:**
Ihr Meta-Konto muss von WPS aktivierte Entwicklerrechte haben, bevor MQDH ordnungsgemäß funktioniert. Das ist nicht etwas, was Sie selbst aktivieren können - es erfordert Koordination mit WPS-Personal, das die Entwicklerorganisationseinstellungen verwaltet. Diese Sicherheitsmaßnahme stellt sicher, dass nur autorisiertes Personal benutzerdefinierte Anwendungen auf WildXR-Deployment-Headsets installieren kann.

## Fehlerbehebung

**Download schlägt fehl oder ist beschädigt:**
- Stabile Internetverbindung während des gesamten Downloads überprüfen
- Versuchen, von anderem Browser oder Inkognito-Modus herunterzuladen
- Verfügbaren Festplattenspeicher vor Download überprüfen
- WPS kontaktieren, wenn Download konsistent fehlschlägt

**Installationsprozess stoppt oder schlägt fehl:**
- Administrative Privilegien auf Computer sicherstellen
- Antivirus während Installation temporär deaktivieren
- Überprüfen, dass System Mindestanforderungen erfüllt
- Computer neu starten und Installation wiederholen
<div style="page-break-after: always;"></div>

**Authentifizierung schlägt wiederholt fehl:**
- Gmail-Adresse mit VR-Setup-Konto abgleichen
- Passwort-Genauigkeit mit WPS-Personal bestätigen
- Überprüfen, dass Konto Entwicklerrechte aktiviert hat
- Sicherstellen, dass 2FA-Codes aktuell sind (30-Sekunden-Ablauf)

**MQDH startet nach Installation nicht:**
- Windows Defender oder Antivirus-Quarantäne überprüfen
- Überprüfen, dass Installation erfolgreich abgeschlossen wurde
- Versuchen, als Administrator auszuführen
- Computer neu starten und Start wiederholen

**Headset wird von MQDH nicht erkannt:**
- Überprüfen, dass sowohl Computer als auch Headset mit demselben WiFi-Netzwerk verbunden sind
- Bestätigen, dass Ihr Meta-Konto Entwicklerrechte über WPS hat
- Prüfen, dass Developer-Modus sowohl in der Oculus-Phone-App als auch in Headset Settings > Advanced > Developer aktiviert ist
- Sicherstellen, dass keine ausstehenden Headset-Updates unter Settings > General > Software Update existieren

**USB-Debugging-Autorisierung erscheint nicht:**
- Überprüfen, dass USB-Kabelverbindungen an beiden Enden sicher sind
- Nach ausstehenden Headset-Updates suchen, die Autorisierung verhindern könnten
- Nach ausstehenden MQDH-Updates suchen, die durch Banner oben in der Anwendung angezeigt werden
- Versuchen, USB-Kabel nach 30 Sekunden zu trennen und wieder zu verbinden
- Headset vollständig aus- und einschalten und Verbindung wiederholen

**Gerät erscheint verbunden, aber zeigt als inaktiv:**
- Bestätigen, dass USB-Debugging ordnungsgemäß mit "Always allow" Option autorisiert wurde
- Meta-Konto-Konsistenz zwischen MQDH und Headset überprüfen
- Prüfen, dass Developer-Modus in Headset-Einstellungen aktiviert bleibt
- Versuchen, Gerät über MQDH-Setup-Assistent zu entfernen und wieder hinzuzufügen
<div style="page-break-after: always;"></div>

## Wichtige Hinweise

⚠️ **Entwicklerrechte erforderlich**: Ihr Meta-Konto muss von WPS gewährten Entwicklerzugang haben, bevor MQDH ordnungsgemäß für benutzerdefinierte App-Installation funktioniert.

⚠️ **Konto-Konsistenz**: Das in MQDH verwendete Meta-Konto muss exakt mit dem Konto übereinstimmen, das mit Ihren VR-Headsets verbunden ist. Gemischte Konten verhindern ordnungsgemäße Geräteerkennung.

⚠️ **Headset-Verknüpfung**: MQDH erfordert, dass Headsets ADB für einige Funktionalitäten aktiviert haben. Wenn Funktionalität fehlt, kann dies das Problem sein.

⚠️ **Software-Updates**: MQDH befindet sich in einem konstanten Entwicklungszustand und erfordert daher oft ein Update. Wenn möglich, MQDH immer aktualisieren, wenn dazu aufgefordert, bevor andere Aufgaben in MQDH abgeschlossen werden.

## Überprüfungsschritte

Überprüfen Sie, dass Ihre MQDH-Anwendung in der Lage ist, VR-Headsets ohne zusätzliche Konfigurationsschritte zu erkennen, sich zu verbinden und zu verwalten.

**Vollständige Funktionalitätsüberprüfung:**
- MQDH startet ohne Fehler und zeigt Kontoinformationen korrekt an
- Mindestens ein Headset erscheint als "Active" in der Geräteliste
- USB-Debugging-Autorisierung wurde gewährt und bestätigt
- Geräteverwaltungssymbole sind in der linken Seitenleiste zugänglich und reagieren
- Sie können auf das Dateisystem des Headsets und Anwendungsverwaltungsfeatures zugreifen