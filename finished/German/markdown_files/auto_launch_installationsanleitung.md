# WildXR Auto Launch Installationsanleitung

## Zweck & Kontext
Diese Anleitung installiert die WPS Auto Launch Anwendung, die WildXR automatisch startet, wenn ein Headset eingeschaltet wird. Auto Launch eliminiert die Notwendigkeit von Hand-Controllern in öffentlichen Installationen, schafft eine nahtlose Benutzererfahrung und ermöglicht die Fernüberwachung der Headset-Betriebszeit. Dieser Prozess verwandelt ein Standard-VR-Headset in ein kiosk-bereites System, das minimale Benutzerinteraktion benötigt, um die Naturschutz-Erfahrung zu beginnen.

⚠️ **Meta**: Meta Hardware und Software (einschließlich MQDH) liegen außerhalb der Kontrolle von WPS. Meta-Updates können unerwartete Funktionalitätsänderungen in VR-Systemen verursachen. WPS überwacht Meta-Veröffentlichungen, um Benutzer über potenzielle Auswirkungen und Änderungen zu informieren.

## Voraussetzungen
- Meta Quest Developer Hub vollständig installiert und konfiguriert mit mindestens einem verbundenen Headset und autorisiertem USB-Debugging *(siehe MQDH Setup Guide)*
- VR-Headset mit aktiviertem Entwicklermodus sowohl in der Oculus-App als auch in den Headset-Einstellungen
- WildXR-Anwendung bereits installiert und mindestens einmal erfolgreich auf dem Ziel-Headset ausgeführt
- `autolaunchping_v.1.0.0.apk` Datei *(bereitgestellt von WPS)*
- Meta-Konto mit von WPS aktivierten Entwicklerrechten
- USB-Kabel zur Verbindung des Headsets während der Installation

## Schneller Überblick (für erfahrene Benutzer)
1. Ziel-Headset mit Computer verbinden *(oder bestehende MQDH-Verbindung überprüfen)*
2. MQDH App-Verwaltung aufrufen und `autolaunchping` APK installieren
3. Auto Launch App starten und WildXR-Integration konfigurieren
4. Automatische Startfunktionalität testen

## Detaillierte Schritte

### Vorbereitung für Auto Launch Installation

1. **Headset für Dateiübertragung verbinden**
   - **Meta Quest Developer Hub** starten
   - Quest Headset einschalten
   - Headset mit USB-Kabel an Computer anschließen
<div style="page-break-after: always;"></div>

2. **Headset-Verbindung überprüfen**
   - Sicherstellen, dass Ihr Ziel-Headset als **"Active"** in der MQDH-Geräteliste erscheint
   - *Neue Headsets benötigen typischerweise den gleichen USB-Debugging-Autorisierungsprozess, der während des MQDH-Setups abgeschlossen wurde (siehe MQDH Setup Guide)*
   - Bestätigen, dass das Headset keine Fehlerindikatoren oder Verbindungsprobleme zeigt

3. **WildXR-Bereitschaft bestätigen**
   - Überprüfen, dass WildXR auf dem Ziel-Headset installiert ist
   - Sicherstellen, dass WildXR mindestens einmal erfolgreich gestartet wurde
   - *Auto Launch kann keine Anwendungen registrieren, die nie auf dem System gelaufen sind*
   - WildXR-Start manuell testen, wenn Sie sich über den Betriebsstatus unsicher sind

### Installation der Auto Launch Anwendung

4. **Anwendungsverwaltung aufrufen**
   - In MQDH auf das **Ordner-Symbol** in der linken Seitenleiste klicken
   - *Dies öffnet die Datei- und Anwendungsverwaltungsschnittstelle*
   - Unter dem Bereich **"On Device"** auf das **"Apps"** Ordner-Symbol klicken
   - *Dies zeigt die aktuell installierten Anwendungen auf Ihrem Headset an*

5. **Auto Launch Anwendung hinzufügen**
   - **"Add Build"** Schaltfläche in der oberen rechten Ecke klicken
   - *Dateibrowser öffnet sich, um Ihre APK-Installationsdatei zu lokalisieren*
   - Zum Speicherort navigieren, wo Sie `autolaunchping_v.1.0.0.apk` gespeichert haben
   - APK-Datei auswählen und **"Open"** klicken

6. **Installationsfortschritt überwachen**
   - MQDH zeigt Installationsfortschrittsindikatoren an
   - Datei vollständig installieren lassen, bevor Sie fortfahren
   - *Installation dauert typischerweise 30-60 Sekunden je nach Systemleistung*
   - Sie sollten `com.wps.autowildxrping` in Ihrer Apps-Liste sehen, wenn die Installation abgeschlossen ist

### Auto Launch Integration konfigurieren

7. **Auto Launch Anwendung starten**
   - `com.wps.autowildxrping` in Ihrer MQDH Apps-Liste lokalisieren
   - Auf das **Drei-Punkte-Menü-Symbol** rechts vom Anwendungsnamen klicken
   - **"Launch App"** aus dem Dropdown-Menü auswählen
   - VR-Headset aufsetzen, um die Konfiguration abzuschließen
<div style="page-break-after: always;"></div>

8. **Auto Launch Setup abschließen**
   - WildXR kann sofort starten, wenn Auto Launch eine bestehende Konfiguration erkennt
   - Wenn WildXR automatisch startet, Headset abnehmen und aus-/einschalten, um die Funktionalität zu testen
   - Wenn Sie stattdessen ein **"WildXRAutoPing"** Fenster sehen, mit manueller Konfiguration fortfahren
   - *Nach einem Kachel-Symbol suchen, das einem Alien oder ungewöhnlichen Symbol ähnelt, in der Quest-Menüleiste, wenn das Fenster nicht sofort sichtbar ist*

9. **Konfiguration abschließen**
   - Im **WildXRAutoPing** Fenster auf die **"Save URL"** Schaltfläche klicken
   - *Dies erstellt die dauerhafte Verbindung zwischen Auto Launch und WildXR*
   - WildXR sollte sofort nach dem Klicken auf **Save URL** starten
   - Headset abnehmen und Gerät aus-/einschalten, um die automatische Startfunktionalität zu überprüfen

## Verstehen des Zwecks der Auto Launch Technologie

Bevor Sie mit der Installation beginnen, hilft es zu verstehen, was Auto Launch erreicht und warum es diesen spezialisierten Installationsprozess benötigt. Traditionelle VR-Anwendungen erfordern, dass Benutzer manuell durch Menüs navigieren und Anwendungen mit Controllern auswählen. Dies funktioniert gut für den persönlichen Gebrauch, schafft aber Barrieren in öffentlichen Naturschutz-Umgebungen, wo Besucher möglicherweise nicht mit VR-Schnittstellen vertraut sind oder wo Controller verloren gehen oder beschädigt werden könnten.

Die WPS Auto Launch Anwendung arbeitet auf der Android-Systemebene und registriert sich selbst, um ausgelöst zu werden, wenn das Headset seine Startsequenz abschließt. Stellen Sie es sich vor wie das Einstellen eines Standard-Webbrowsers auf Ihrem Computer, außer dass statt Web-Links Auto Launch das Headset-Startereignis behandelt. Wenn das System hochfährt, signalisiert Auto Launch sofort WildXR zu beginnen und schafft einen nahtlosen Übergang vom Einschalten zum Naturschutz-Inhalt.

Diese Systemebenen-Integration ist der Grund, warum die Installation Meta Quest Developer Hub statt Standard-App-Installationsmethoden erfordert. Wir modifizieren im Wesentlichen das Verhalten des Headsets auf einer tieferen Ebene, als normale Anwendungen darauf zugreifen.

## Fehlerbehebung

**MQDH zeigt keine verbundenen Geräte:**
- Überprüfen Sie, dass Sie das vollständige MQDH-Setup einschließlich USB-Debugging-Autorisierung abgeschlossen haben
- Prüfen Sie, dass Ihr Ziel-Headset dasselbe ist, das während des MQDH-Setups konfiguriert wurde
- Bei Verwendung eines anderen Headsets benötigt es den gleichen USB-Debugging-Autorisierungsprozess
- Sicherstellen, dass das Headset während der gesamten Installation eingeschaltet und verbunden bleibt
<div style="page-break-after: always;"></div>

**Auto Launch Installation schlägt fehl:**
- Bestätigen Sie, dass WildXR ordnungsgemäß installiert ist und mindestens einmal erfolgreich ausgeführt wurde
- Überprüfen Sie, dass das Headset ausreichend Speicherplatz für zusätzliche Anwendungen hat
- Prüfen Sie, dass `com.wps.autowildxrping` in der MQDH Apps-Liste erscheint, bevor Sie mit der Konfiguration fortfahren
- Sicherstellen, dass die `autolaunchping` APK-Datei nicht beschädigt ist, indem Sie die Installation auf einem anderen Headset versuchen

**Auto Launch Funktionalität funktioniert nach Installation nicht:**
- Überprüfen Sie, dass `com.wps.autowildxrping` als laufend im MQDH Drei-Punkte-Menü erscheint
- Bestätigen Sie, dass WildXR manuell startet, um die Anwendungsintegrität sicherzustellen
- Testen Sie einen kompletten Aus-/Einschaltvorgang statt Schlaf/Aufwachen, um das Startverhalten zu überprüfen
- Prüfen Sie, dass **"Save URL"** während der Konfiguration geklickt wurde und dass WildXR danach gestartet ist

**WildXRAutoPing Fenster nicht sichtbar:**
- Nach einem ungewöhnlichen oder alien-ähnlichen Symbol in der Quest-Menüleiste suchen
- Versuchen Sie, das Headset abzunehmen und wieder aufzusetzen, um die Schnittstelle zu aktualisieren
- Sicherstellen, dass die Auto Launch App tatsächlich von MQDH gestartet wurde, nicht nur installiert
- Prüfen Sie, dass WildXR mindestens einmal vor der Auto Launch Konfiguration ausgeführt wurde

## Wichtige Hinweise

⚠️ **Entwicklerkonto-Anforderungen**: Ihr Meta-Konto muss verifizierten Entwicklerstatus bei Wildlife Protection Solutions haben, bevor jede benutzerdefinierte Anwendungsinstallation erfolgreich sein wird.

⚠️ **Systemkompatibilität**: Auto Launch erfordert Headsets mit ordnungsgemäß aktiviertem Entwicklermodus sowohl in der Oculus Mobile-Anwendung als auch in den internen Einstellungen des Headsets unter **Advanced > Developer**.

⚠️ **Konto-Übereinstimmung**: Das für MQDH verwendete Meta-Konto muss exakt mit dem Konto übereinstimmen, das zur Konfiguration des Headsets verwendet wird. Nicht übereinstimmende Konten verhindern Geräteerkennung und Anwendungsinstallation.

⚠️ **WildXR Voraussetzungen**: WildXR muss erfolgreich installiert und mindestens einmal gestartet werden, bevor die Auto Launch Installation erfolgt. Auto Launch kann keine Anwendung registrieren, die das System nicht erkennt.
<div style="page-break-after: always;"></div>

## Überprüfung und Testen

Nach Abschluss der Installation überprüfen Sie die Auto Launch Funktionalität durch umfassende Tests. Schalten Sie das Headset mit dem Power-Button vollständig aus, warten Sie 30 Sekunden und schalten Sie es dann wieder ein. Auto Launch sollte den WildXR-Start ohne manuelle Intervention oder Controller-Verwendung auslösen. Wenn manuelle Navigation immer noch erforderlich ist, wurde der Registrierungsprozess nicht erfolgreich abgeschlossen und sollte ab Schritt 5 wiederholt werden.