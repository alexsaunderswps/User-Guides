# Quest VR Headset Empfohlene Einstellungen

## Zweck & Kontext
Diese Anleitung beschreibt empfohlene Einstellungen für Quest 2, Quest 3 und Quest 3s, um die WildXR VR-Erfahrung konsistent und zuverlässig zu machen.

⚠️ **Meta**: Meta Hardware und Software (einschließlich MQDH) liegen außerhalb der Kontrolle von WPS. Meta-Updates können unerwartete Funktionalitätsänderungen in VR-Systemen verursachen. WPS überwacht Meta-Veröffentlichungen, um Benutzer über potenzielle Auswirkungen und Änderungen zu informieren.

## Voraussetzungen
- Quest-Headset und Controller mit Batterien

## Schneller Überblick (für erfahrene Benutzer)
1. Das **Settings** Menü aufrufen
2. Energieeinstellungen entsprechend gewünschtem Anwendungsfall ändern
3. Aktivieren:
    - **Do Not Disturb**
    - **Developer Mode**
    - **Enable MTP connection**
4. Deaktivieren:
    - **Cloud Backup**
    - **Automatic Updates**
    - **Interactive Elements**

## Detaillierte Schritte

### Auf das Settings Menü zugreifen

1. **WildXR-Anwendung beenden (falls laufend)**
   - **Meta-Logo-Taste** (Quest 3 und Quest 3s) oder **Horizontale Ovale Taste** (Quest 2) am rechten Hand-Controller drücken
   - **"Quit"** im App-Verwaltungsfenster auswählen, das erscheint
   - Falls das App-Verwaltungsfenster nicht erscheint:
     - **Headset-Power-Taste** drücken, um das Headset in den Ruhemodus zu versetzen
     - **Headset-Power-Taste** erneut drücken, um das Headset aufzuwecken
     - **Meta-Logo-Taste** am rechten Hand-Controller drücken
     - **"Quit"** im App-Verwaltungsfenster auswählen

2. **Quick Settings Menü öffnen**
   - Die **Taste klicken, die Zeit, WiFi-Stärke und Batteriestand anzeigt** in der linken Menüleiste
   - *Ein neues schwebendes Fenster sollte erscheinen, das Quick Menu Settings anzeigt*
<div style="page-break-after: always;"></div>

3. **Settings Menü öffnen**
   - **"Settings"** oben rechts in der Quick Settings Menü-Anzeige klicken
   - *Ein neues schwebendes Fenster sollte erscheinen, das Headset Settings anzeigt*
   - *Einige Optionen sind nicht sichtbar, bis Sie die linke Liste der Einstellungskategorien scrollen*
   - *Joysticks an beiden Controllern ermöglichen das Scrollen, wenn das Zielkreuz über der Liste schwebt*

### General Settings

4. **Software Update Einstellungen**
   - Den **"Software Update"** Tab klicken
   - Alle Optionen **ausschalten**:
     - `Software updates`
     - `Security and Critical updates`
     - `Automatically power headset to update`
     - `Update and backup before shutdown`

5. **Cloud Backup Einstellungen**
   - Den **"Cloud Backup"** Tab klicken
   - `Cloud Backups` **ausschalten**

6. **Power Einstellungen**
   - Den **"Power"** Tab klicken
   - **"Display Off"** auf **4 hours** setzen
   - **"Auto Sleep Headset"** auf **4 hours** setzen *(möglicherweise nicht bei allen Headsets vorhanden)*
   - Alle Optionen unter **"Battery"** **ausschalten**:
     - `Battery Saver`
     - `Low battery audio alert`
     - `Low battery voice alert`

### Notification Settings

7. **Notification Einstellungen**
   - `Do Not Disturb` **einschalten**
   - **"Until I turn it off"** aus den erscheinenden Optionen auswählen
   - **"Done"** klicken

### Environment Setup Settings

8. **Interactive Objects Einstellungen**
   - Den **"Interactive objects"** Tab klicken
   - Alle Optionen **ausschalten**:
     - `Avatar Mirror`
     - `First Encounters`
     - `Portal to Meta Horizon World`
<div style="page-break-after: always;"></div>

### Advanced Settings

9. **Developer Einstellungen**
   - `Enable Developer Settings` **einschalten**
   - `Enable MTP Notification` **einschalten**
   - `Physical Space Features` **ausschalten**
   - `Link Auto-Connect` **ausschalten**

### Nächste Schritte

10. **App-PIN erstellen und Apps sperren**
    - Der **Library Management** Anleitung folgen

## Empfohlene Headset-Einstellungen verstehen

**Warum diese Einstellungen:**
Die empfohlenen Einstellungen wurden in öffentlichen Veranstaltungsorten getestet und bieten bis heute die konsistenteste und langlebigste Benutzererfahrung.

**Software Update Einstellungen**
Das Ausschalten aller automatischen Update-Einstellungen verhindert, dass ein Headset während öffentlicher Öffnungszeiten unerwartet nicht verfügbar ist. Es ermöglicht auch, Software-Updates auf kontrollierte Weise zu testen, um unvorhergesehene Konflikte zwischen WildXR, Auto Launch und Headset-Software zu verhindern. Meta hat erzwungene Updates nach 30 - 45 Tagen Verzögerung eingeführt, was WPS ein Zeitfenster gibt, Updates auf Leistung zu prüfen und, wenn möglich, auf Software-Konflikte zu reagieren. Wir empfehlen, Headsets alle 21 Tage als Routinewartung auf ausstehende Updates zu überprüfen und WPS bezüglich der Installation um Anleitung zu bitten.

**Cloud Backup Einstellungen:**
Es gibt keinen Nutzen für Cloud Backup in den meisten Endbenutzer-Anwendungsfällen, wo WildXR in öffentlichen oder Bildungseinstellungen verwendet wird.

**Power Einstellungen**
Das Setzen von **"Display Off"** auf **4 hours** ermöglicht es Headsets, die in öffentlichen oder Bildungseinstellungen verwendet werden, sofort auf Nutzung zu reagieren. Das Ausschalten des Displays verlängert die Batterielaufzeit, kann aber dazu führen, dass das Headset langsam auf Nutzung reagiert und die Ausrichtung von Szenen in WildXR auf unerwartete Weise beeinflusst.

**Notification Einstellungen**
Benachrichtigungen können Benutzererfahrungen stören, indem sie Pop-up-Fenster innerhalb der WildXR-Anwendung anzeigen.

**Interactive Objects Einstellungen**
Ein Benutzer kann sich im Quest-Hauptmenübildschirm wiederfinden, wenn es ein unerwartetes Problem mit dem Auto Launch-Programm oder der WildXR-Anwendung gibt. Benutzer, die mit VR-Headsets vertraut sind, können WildXR in bestimmten Situationen zwangsweise beenden, um auf das Quest-Hauptmenü zuzugreifen. Durch das Verbergen interaktiver Objekte können wir einiges bösartiges oder einfach neugieriges Verhalten verhindern, das Geräteeinstellungen verändert.
<div style="page-break-after: always;"></div>

**Developer Einstellungen**
Das Ausschalten physischer Raumfunktionen entfernt die Notwendigkeit, eine Grenze im Headset zu definieren. Grenzeinstellungen können die Benutzererfahrung beeinträchtigen, indem sie die WildXR-Anzeige unterbrechen, wenn ein Benutzer sich außerhalb der Grenze bewegt. Grenzen müssen auch jedes Mal eingerichtet werden, wenn ein Headset irgendeine Entfernung bewegt wird, und können in einigen Situationen unerwartetes Verhalten verursachen.
MTP-Benachrichtigungen ermöglichen es, das Headset als Laufwerk zu sehen, wenn es über USB mit einem Computer verbunden ist. Dies ermöglicht Dateiübertragung und -manipulation, die in einigen Fehlerbehebungssituationen benötigt wird.

## Fehlerbehebung

**Developer-Bereich nicht sichtbar unter Advanced Settings:**
- Die Anleitung zur Aktivierung von Developer Settings auf Ihrem Headset überprüfen
- Sicherstellen, dass Ihr Meta-Konto von WPS aktivierte Entwicklerrechte hat
- Überprüfen, dass Developer-Modus sowohl in der Meta Horizon Phone-App als auch in den Headset-Einstellungen aktiviert ist

**Einstellungsänderungen bleiben nicht bestehen:**
- Sicherstellen, dass Sie jeden Abschnitt vollständig abschließen, bevor Sie zum nächsten übergehen
- Überprüfen, dass das Headset nicht in einem eingeschränkten Modus oder unter Kindersicherung steht
- Prüfen, dass Ihr Konto Administratorrechte auf dem Gerät hat

**Kann nicht auf bestimmte Einstellungsoptionen zugreifen:**
- Bestätigen, dass Ihr Meta-Konto die notwendigen Berechtigungen hat
- Prüfen, ob das Headset in einem Organisationsverwaltungssystem eingeschrieben ist
- Überprüfen, dass die Headset-Software-Version alle aufgelisteten Einstellungen unterstützt

**Power-Einstellungen verursachen unerwartetes Verhalten:**
- Verschiedene **"Display Off"** Zeiteinstellungen testen, wenn 4 Stunden Probleme verursachen
- Batterielaufzeit mit angepassten Einstellungen überwachen
- Sicherstellen, dass das Headset während Spitzennutzungszeiten reagiert

## Wichtige Hinweise

⚠️ **Standardwerte-Warnung**: Standardwerte können die Batterielaufzeit verlängern, aber unerwartetes Verhalten in der WildXR-Anwendung einführen.

⚠️ **Developer-Voraussetzungen**: Wenn ein Developer-Bereich unter Advanced Settings nicht sichtbar ist, überprüfen Sie die Anleitung zur Aktivierung von Developer Settings auf Ihrem Headset.

⚠️ **Update-Verwaltung**: Meta hat erzwungene Updates nach 30-45 Tagen Verzögerung eingeführt. Headsets alle 21 Tage auf ausstehende Updates prüfen und WPS um Anleitung bitten.

⚠️ **Entwicklerrechte erforderlich**: Ihr Meta-Konto muss von WPS gewährten Entwicklerzugang haben, bevor erweiterte Einstellungsänderungen verfügbar sind.