# VR Headset Basic Connection Anleitung

## Zweck & Kontext
Diese Anleitung schafft die Grundlage für alle VR-Headset-Dateiverwaltungsaufgaben. Sie verbinden Ihr Meta Quest 2, Quest 3 oder Quest 3s mit einem Computer und greifen auf die WildXR-Anwendungsdateien zu. Diese Verbindung ist erforderlich, bevor Sie Mediendateien übertragen, Konfigurations- oder localConfiguration-Dateien bestätigen oder Anwendungsprobleme beheben.

⚠️ **Meta**: Meta Hardware und Software (einschließlich MQDH) liegen außerhalb der Kontrolle von WPS. Meta-Updates können unerwartete Funktionalitätsänderungen in VR-Systemen verursachen. WPS überwacht Meta-Veröffentlichungen, um Benutzer über potenzielle Auswirkungen und Änderungen zu informieren.

## Voraussetzungen
- Meta Quest 2, Quest 3 oder Quest 3s VR-Headset
- USB-C-Kabel *(empfohlen)* oder USB-C zu USB-A-Kabel
- Computer mit File Explorer *(Windows)* oder Finder *(Mac)*
- AA-Batterien für Controller
- WildXR-Anwendung auf Headset installiert
- Developer-Einstellungen auf dem Headset aktiviert

## Schneller Überblick (für erfahrene Benutzer)
1. Headset einschalten und sicherstellen, dass Controller Batterien haben
2. USB-Kabel verbinden und WildXR beenden, falls laufend
3. USB-Verbindung über Quest-Benachrichtigungen aktivieren
4. Navigieren zu: `Quest` > `Internal shared storage` > `Android` > `data` > `com.wps.wildx` > `files`

## Detaillierte Schritte

### Erste Einrichtung

1. **Controller-Batterien installieren**
   - Sowohl Quest 2 als auch Quest 3 verwenden **AA-Batterien**
   - Sicherstellen, dass beide Controller eingeschaltet sind

2. **Headset einschalten**
   - **Quest 2**: **Power-Taste** auf der rechten Seite drücken
   - **Quest 3 & Quest 3s**: **Power-Taste** auf der linken Seite drücken

3. **USB-Kabel verbinden**
   - **Quest 2**: USB-Anschluss befindet sich auf der linken Seite unter dem Bügel
   - **Quest 3 & Quest 3s**: USB-Anschluss befindet sich auf der linken Seite am Bügel
<div style="page-break-after: always;"></div>

4. **Primären Controller identifizieren**
   - **Quest 2**: Rechter Controller hat **horizontale ovale Taste**
   - **Quest 3 & Quest 3s**: Rechter Controller hat **Meta-Logo-Taste**

### WildXR-Anwendung beenden

*Wenn WildXR automatisch startet, müssen Sie es beenden, um auf Dateien zuzugreifen.*

5. **Versuchen, Systemmenü zu öffnen**
   - Headset aufsetzen
   - **Ovale/Meta-Taste** am rechten Controller drücken und loslassen
   - Wenn **Quit/Resume** Bildschirm erscheint, zu Schritt 8 springen

6. **Menü-Erscheinen erzwingen (falls nötig)**
   - **Power-Taste** drücken, um Headset schlafen zu legen *(Bildschirm wird dunkel)*
   - **Power-Taste** erneut drücken, um Headset aufzuwecken
   - **Ovale/Meta-Taste** erneut versuchen
   - Wiederholen, bis **Quit/Resume** Bildschirm erscheint

7. **WildXR beenden**
   - **"Quit"** mit Controller-Trigger auswählen
   - *Sie sollten die Quest-Startumgebung sehen*

### Computer-Zugang aktivieren

8. **Benachrichtigungen öffnen**
   - Zielpunkt auf **Glocken-Symbol** in der Menüleiste richten
   - **Controller-Trigger** *(unter Zeigefinger)* drücken, um Benachrichtigungen zu öffnen

9. **USB-Verbindung aktivieren**
   - *Sie müssen Developer-Einstellungen auf dem Headset aktiviert haben*
   - **"USB Detected"** Benachrichtigung finden
   - Auf Benachrichtigung zielen und **Controller-Trigger** drücken
   - *Dies ermöglicht es dem Computer, das Headset als externes Laufwerk zu erkennen*

### Auf Dateien am Computer zugreifen

10. **Dateibrowser öffnen**
    - **Windows**: **File Explorer** öffnen, **"This PC"** klicken
    - **Mac**: **Finder** öffnen

11. **Zum Headset navigieren**
    - Doppelklick auf **"Quest 2"**, **"Quest 3"** oder **Quest 3s**
    - Doppelklick auf **"Internal shared storage"**
<div style="page-break-after: always;"></div>

12. **Zu WildXR-Dateien navigieren**
    - Doppelklick auf **"Android"**
    - Doppelklick auf **"data"**
    - Doppelklick auf **"com.wps.wildx"**
    - Doppelklick auf **"files"**

*Sie haben jetzt Zugang zu WildXR-Dateien und -Ordnern.*
## WildXR-Dateien und -Ordner verstehen

**downloads Ordner**
- Enthält alle heruntergeladenen Videos für die WildXR-Anwendung
- Dateien benannt mit universell eindeutiger 36-Zeichen-ID (UUID)
- Alle im MP4-Format
- *Dieser Ordner ist, wo **sideloadete** Video-Dateien platziert werden*

**textures Ordner**
- Enthält alle heruntergeladenen Thumbnail-Bilder für die WildXR-Anwendung
- Dateien benannt mit UUID, die der Video-UUID entspricht
- Alle im PNG-Format

**temp Ordner**
- Enthält temporäre Dateien, die von der WildXR-Anwendung benötigt werden
- Enthält oft Video-Dateien, die von der WildXR-Anwendung heruntergeladen werden

**Unity Ordner**
- WildXR Unity-Dateien
- Kein Zugang für die meisten Benutzer nötig

**localConfiguration.json Datei**
- Konfigurationseinstellungen, die gerätespezifisch (Headset) sind
- Enthält Device ID, Environment und OfflineMode-Einstellungen

**configuration.json Datei**
- Konfigurationseinstellungen, die das Erscheinungsbild der WildXR-Anwendung steuern
- Wenn Headset oder Computer (Gerät) über WildXR Web Portal registriert ist, werden diese Einstellungen remote gesteuert
- Wenn Headset oder Computer (Gerät) nicht über WildXR Web Portal registriert ist, sind diese Einstellungen von der WildXR-Anwendung vorkonfiguriert

**metadataDatabase.json**
- Metadaten, die von der WildXR-Anwendung für ordnungsgemäße Funktion benötigt werden
<div style="page-break-after: always;"></div>

**DownloadQueue.json**
- Informationen für Video-Download-Funktion in der WildXR-Anwendung
- Kann leer oder abwesend sein, wenn keine Videos zum Download in der Warteschlange stehen

**Player.log und Player-prev.log**
- Log-Dateien, die das neueste und vorherige Verhalten der WildXR-Anwendung aufzeichnen
- Wichtig für die Diagnose von Problemen und können von WPS-Personal zur Diagnose angefordert werden

**youtubeData.json**
- Daten zur Sortierung von Videos in Thumbnail-Galerien basierend auf verschiedenen Faktoren

## Fehlerbehebung

**Headset erscheint nicht im Dateibrowser:**
- Sicherstellen, dass USB-Kabel vollständig verbunden ist
- Anderen USB-Anschluss am Computer versuchen
- Prüfen, dass Sie USB-Verbindung in Schritt 9 aktiviert haben
- Überprüfen, dass das USB-Kabel Datenübertragung unterstützt, nicht nur Laden

**Kann WildXR nicht beenden:**
- Headset kurz abnehmen, dann wieder aufsetzen
- Headset aus-/einschalten *Power-Taste drücken, um Headset schlafen zu legen, dann erneut drücken zum Aufwecken*
- Sicherstellen, dass Controller ausreichend Batterieleistung haben

**Controller reagieren nicht:**
- Batterie-Installationsrichtung überprüfen
- Frische AA-Batterien versuchen
- Sicherstellen, dass Controller gekoppelt sind *(sollte automatisch beim Headset-Start passieren)*
- Controller aus-/einschalten durch Entfernen und Wiedereinsetzen der Batterien

**USB-Verbindungsbenachrichtigung erscheint nicht:**
- USB-Kabel trennen und wieder verbinden
- Anderen USB-Anschluss am Computer versuchen
- Sicherstellen, dass Headset vollständig eingeschaltet und nicht im Ruhemodus ist
- Prüfen, ob Developer-Modus in Headset-Einstellungen aktiviert ist
- *Sie müssen die USB-Verbindungsbenachrichtigung jedes Mal akzeptieren, wenn USB verbunden wird*
<div style="page-break-after: always;"></div>

**Dateien/Ordner erscheinen leer oder unzugänglich:**
- Überprüfen, dass WildXR mindestens einmal auf dem Headset ausgeführt wurde
- Prüfen, dass der korrekte Pfad befolgt wird: `Android` > `data` > `com.wps.wildx` > `files`
- Sicherstellen, dass USB-Debugging-Berechtigungen gewährt wurden, falls dazu aufgefordert
- Dateibrowser-Ansicht aktualisieren versuchen

## Wichtige Hinweise

⚠️ **Dateibearbeitungseinschränkung**: Dateien wie `configuration.json` können nicht direkt auf dem Headset bearbeitet werden. Sie müssen:
1. Dateien auf Ihren Computer kopieren
2. Sie dort bearbeiten
3. Die modifizierten Dateien zurückkopieren, um Originale zu überschreiben
4. Dateien können geöffnet werden, um zu überprüfen, dass Änderungen angewendet wurden *(siehe **File Transfer Verification** unten)*

⚠️ **Backup-Empfehlung**: Immer eine Backup-Kopie von Konfigurationsdateien vor der Bearbeitung erstellen.

⚠️ **Dateibearbeitungsüberprüfung**: Immer prüfen, dass bearbeitete Dateien erfolgreich auf das Headset übertragen wurden.

⚠️ **Dateiübertragungsempfehlung**: Beim Sideloading von Video-Dateien überprüfen, dass der **downloads** Ordner die Anzahl der Videos enthält, die Sie zu sideloaden versucht haben.

⚠️ **Kabelanforderungen**: Sicherstellen, dass Ihr USB-Kabel Datenübertragung unterstützt. Einige Kabel sind nur zum Laden und erlauben keinen Dateizugriff.

⚠️ **WildXR-Voraussetzungen**: WildXR muss installiert und mindestens einmal ausgeführt werden, bevor Dateien in der erwarteten Verzeichnisstruktur zugänglich sind.