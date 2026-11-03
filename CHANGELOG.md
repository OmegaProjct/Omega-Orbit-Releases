# Changelog

## [0.8.5] - 2026-11-03

#### Behoben
- **Build- und Release-Pipeline stabilisiert**: Ein Fehler im automatisierten Paketierungsprozess wurde behoben, sodass alle Verbesserungen der Version 0.8.4 (orbitaler Kamera-Blob, Hardware-Exklusivität für Webcams und stabiler Fensterfokus) nun zuverlässig über den Updater bereitstehen.

## [0.8.4] - 2026-11-02

#### Hinzugefügt
- **Orbitaler Kamera-Blob am Orbit-Rad**: Die Live-Kameravorschau dockt nun direkt am Orbit-Rad an und kann mit der Maus stufenlos 360° um das Rad herum positioniert werden.
- **Wählbare Kameraform (16:9 oder Kreis)**: Der Kamera-Blob kann wahlweise im 16:9-Kinoformat oder als kompakter runder Kreis angezeigt werden.
- **Einklapp-Modus für das Orbit-Rad**: Ein Klick auf „Schließen“ blendet das Rad aus und lässt auf Wunsch nur die schwebende Kamera auf dem Desktop zurück.
- **Kamerabild in Bildschirmaufnahmen verbergen**: Ist „Orbit in Bildschirmaufnahmen ausblenden“ aktiv, bleibt auch der angedockte Kamera-Blob für die Aufnahme unsichtbar.

#### Behoben
- **Aufnahmeabbrüche bei Kamera- und Bildschirmaufnahme**: Konflikte beim gleichzeitigen Zugriff auf die Webcam („Device in use“) und daraus resultierende FFmpeg-Abbrüche (SIGTERM) wurden vollständig behoben.
- **Unerwünschte Fensterverschiebung bei Discord und Spotify**: Maximierte Anwendungsfenster behalten ihre Vollbild-Position und werden beim Klick im Orbit-Rad nicht mehr um 10 % nach unten und zur Seite verschoben.

## [0.8.3] - 2026-11-02

#### Hinzugefügt
- **Orbit in Bildschirmaufnahmen ausblenden**: In den Video-Einstellungen kann festgelegt werden, dass das Orbit-Rad während der Aufnahme unsichtbar bleibt und nicht im fertigen Video erscheint.
- **Schwebende Kamera-Live-Vorschau**: Das eigene Kamerabild kann während der Aufnahme als schwebender Kreis oder Rahmen direkt auf dem Desktop eingeblendet werden.
- **Kamera-Ausschnitt und Zoom (100 % – 300 %)**: In den Video-Einstellungen kann der Bildausschnitt der Kamera per Schieberegler stufenlos herangezoomt werden, um z. B. nur das Gesicht zu zeigen.
- **Kamera-Vorschau per Maus verschieben**: Die Position der Kameraeinblendung lässt sich in der Einstellungsvorschau nun bequem per Drag & Drop mit der Maus an die gewünschte Stelle ziehen.
- **Direkte MP4-Aufnahme**: Bei Auswahl des MP4-Formats wird direkt als MP4 aufgezeichnet, ohne Zwischenschritt und ohne doppelte Restdateien.

#### Behoben
- **Kamera-Pufferüberlauf bei Auslastung**: Abbrüche bei gleichzeitiger Kamera- und Bildschirmaufnahme durch zu kleine Echtzeit-Eingangspuffer behoben.
- **Lippensynchronität bei Videoaufnahmen**: Bild und Ton bleiben nun auch bei dropped Frames und schwankenden Systemlasten dauerhaft synchron.
- **Fensterfokus bei Spotify und Discord**: Minimierte Fenster bleiben beim Klick im Orbit-Rad nun dauerhaft im Vordergrund geöffnet und schließen sich nicht mehr sofort wieder.
- **Berechtigungsdialoge unter Windows**: UAC-Berechtigungsabfragen führen nicht mehr zum Abbruch der Videoaufnahme; die Aufnahme pausiert sicher und setzt sich nahtlos fort.
- **Löschen der Quelldatei beim Umpacken**: Wenn das automatische Löschen der MKV-Quelldatei nach erfolgreichem MP4-Umpacken aktiviert ist, wird die Quelldatei nun zuverlässig entfernt.

## [0.8.2] - 2026-11-02

#### Hinzugefügt
- **Bereits laufende Apps in den Vordergrund holen**: Klickt man im Orbit-Rad auf eine bereits geöffnete Anwendung (z. B. Spotify oder Discord), wird das vorhandene Fenster sofort wiederhergestellt und in den Vordergrund geholt, statt eine zweite Instanz zu starten.

#### Geändert
- **Rad beim App-Start immer ausblenden**: Das Orbit-Rad schließt sich beim Starten einer Anwendung nun zuverlässig in allen Schließ-Modi, auch wenn „Dauerhaft geöffnet bleiben“ aktiv ist.

#### Behoben
- **Fehlende App-Symbole im App-Starter**: Symbole für Microsoft-Store-Apps (wie Spotify), Squirrel-Anwendungen (wie Discord), Steam-Spiele und Windows-Systemwerkzeuge werden nun vollständig erkannt und angezeigt.

## [0.8.1] - 2026-11-02

#### Hinzugefügt
- **Aufnahme-Einstellungen im Rad**: Eine neue Kachel im Aufnahmemenü öffnet direkt die Video- und Aufnahmeeinstellungen an der richtigen Stelle.
- **Erweiterte Video-Optionen**: Zusätzliche Auflösungen (4K UHD, 1440p QHD, 480p SD) und Bildraten (24 FPS, 120 FPS) sowie verständliche Erklärungen zu Encodern und Qualitätsstufen ergänzt.

#### Geändert
- **Integrierte Hinweis- und Fehlermeldungen**: Meldungen zur Aufnahme erscheinen nun als verschiebbares Fenster direkt im Vordergrund vor dem Orbit-Rad statt als verdeckter Systemdialog.

#### Behoben
- **Start der Bildschirm- und Kameraaufnahme**: Abbrüche beim Starten von Videoaufnahmen mit mehreren Monitoren, aktiven Kameravorschauen oder langsamer initialisierenden Kameras behoben.
- **Automatische Kameraauswahl**: Beim Start einer Kameraaufnahme ohne vorherige Auswahl wird nun automatisch die erste verfügbare Kamera genutzt.

## [0.8.0] - 2026-11-02

- Bildschirm- und Webcam-Aufnahme: Bildschirme und Fenster direkt über das Orbit-Rad aufzeichnen, synchron mit Systemton und Mikrofon.
- Smarte Kamera-Einblendung: Bild-in-Bild-Webcam mit kreisförmiger, abgerundeter oder eigener Maskenform direkt im Video platzieren.
- Hardware-beschleunigte Videoaufnahme: Automatische Erkennung und Nutzung von NVIDIA NVENC, Intel QuickSync und AMD AMF für flüssige Aufnahmen in 1080p bei 60 FPS.
- Verlustfreies MP4-Remuxing: Robuste MKV-Aufnahmen direkt nach der Aufnahme oder später in den Einstellungen sicher in MP4 umpacken.
- Visueller Fortschrittsring: Der Regenbogenrand am Orbit-Rad zeigt den Status beim Umpacken und Konvertieren von Aufnahmen live an.

## [0.7.1] - 2026-11-02

- Tastenkürzel zum Öffnen des Orbit-Rads in den Einstellungen anpassbar gemacht.
- Darstellung der Versionshinweise im Update-Fenster korrigiert.

## [0.7.0] - 2026-11-02

- Smarter App-Katalog im Rad: Beim Klick auf das Plus-Symbol im Apps-Menü steht nun eine durchsuchbare Liste aller installierten Windows-Programme bereit, über die sich Anwendungen mit einem Klick und Original-Symbol hinzufügen lassen.
- Zuverlässiger Start geschützter Windows-Tools: Der Task-Manager und andere Systemprogramme lassen sich nun fehlerfrei über das Rad starten.
- Verbesserte Dateidarstellung: Längere Dateinamen brechen sauber zweizeilig um, ein Tooltip zeigt den vollständigen Pfad und Dateien erhalten automatisch das Symbol des im System verknüpften Standardprogramms (z. B. Mediaplayer für Videos).
- Volle Bedienbarkeit während Aufnahmen: Apps, Dateien und Lesezeichen können nun auch während einer laufenden Audioaufnahme im Rad verwaltet werden, ohne vom Aufnahmestatus verdeckt zu werden.
- Fensterverschiebung beim Speichern: Das Orbit-Rad kann nun auch während der Konvertierung und Speicherung von Aufnahmen frei am Mittelbereich verschoben werden.
- Fehler- und Hinweismeldungen werden nicht mehr am unteren Fensterrand abgeschnitten.

## [0.6.1] - 2026-11-01

- Darstellung beim schnellen Hinzufügen von Dateien und Apps korrigiert.
- Wackelanimation und Entfernen-Schaltfläche im Bearbeitungsmodus verbessert.

## [0.6.0] - 2026-11-01

- Eigene Bereiche für Lesezeichen und Dateien: Neben installierten Apps können nun auch Web-Lesezeichen und Dateien direkt im Orbit-Rad sowie in den Einstellungen verwaltet und im Standardbrowser bzw. der Standardanwendung geöffnet werden.
- Schnelles Verwalten im Rad: Über ein Plus- und Minus-Symbol in der Radmitte können Elemente direkt angelegt (auch per Klick aus der Zwischenablage) oder im iOS-Wackelmodus per Lösch-Knopf entfernt werden.
- Symboldarstellung korrigiert: Das echte Programmsymbol von Brave sowie das authentische Aktivitätssymbol des Windows Task-Managers werden nun zuverlässig angezeigt.

## [0.5.9] - 2026-11-01

- Erweiterte Download-Anzeige im Rad: Die Radmitte zeigt während des Updates neben Prozentwerten nun auch die aktuelle Download-Geschwindigkeit, die verbleibende Restzeit und das übertragene Datenvolumen live an.

## [0.5.8] - 2026-11-01

- Kacheln im Orbit-Rad lückenlos verbunden und den Wechsel der Beschriftung geglättet.
- Feedback-Versand und Schutz persönlicher Angaben in Protokollen verbessert.
- Fehler beim erneuten Start abgebrochener Update-Downloads behoben.
- App-Starter für Skripte verbessert.

## [0.5.7] - 2026-11-01

- Rad-Verschiebung bei Windows-Skalierung stabilisiert.
- Update-Downloads und Feedback-Übermittlung zuverlässiger gemacht.
- Fehlererkennung beim App-Start verbessert und Changelogs in der App ergänzt.

## [0.5.6] - 2026-11-01

- Download-Fortschritt nach dem Schließen des Update-Fensters im Rad anzeigen.
- Automatische Update-Prüfung beim Öffnen des Rads und im Hintergrund ergänzt.

## [0.5.5] - 2026-11-01

- Verschieben und Andocken des Rads sowie Monitorwechsel verbessert.
- App-Starter in den Einstellungen übersichtlicher gemacht.

## [0.5.4] - 2026-11-01

- Originale Windows-Programmsymbole für den App-Starter ergänzt.
- Update-Hinweise und Zusammenspiel von Rad und Einstellungen verbessert.

## [0.5.3] - 2026-11-01

- Blättern über die Radmitte, App-Umbenennung und weitere Darstellungsoptionen ergänzt.

## [0.5.2] - 2026-11-01

- Verschieben des Rads, Positionierung und Dateiauswahl für Apps ergänzt und verbessert.

## [0.5.1] - 2026-11-01

- Fehler beim Start des App-Starters behoben.

## [0.5.0] - 2026-11-01

- App-Starter, mehrere Radseiten und anpassbare Kachelanzahl ergänzt.
- Sitzungsprotokolle und Feedback-Bereich hinzugefügt.

## [0.4.2] - 2026-11-01

- Neues Omega-Orbit-Symbol für Anwendung und Infobereich ergänzt.

## [0.4.1] - 2026-11-01

- Fortschritt beim Herunterladen, Umwandeln und Speichern direkt am Rand des Orbit-Rads anzeigen.

## [0.4.0] - 2026-11-01

- Neues Update-Fenster direkt über das Orbit-Rad öffnen.
- Versionshinweise während und nach dem Herunterladen übersichtlicher anzeigen.
- Update-Ansicht in den Einstellungen verbessert.

## [0.3.0] - 2026-11-01

- Fortschritt beim Umwandeln und Speichern von Aufnahmen anzeigen.
- Fehler beim mehrfachen Beenden einer Aufnahme behoben.
- Updates direkt über das Orbit-Rad prüfen und herunterladen.
- Audio-Einstellungen übersichtlicher gestaltet und Hilfe und Protokoll ergänzt.
- Fehler beim Windows-Autostart behoben.

## [0.2.0] - 2026-11-01

- Omega Orbit öffnet sich per Tastenkürzel direkt am Mauszeiger.
- Audio aus mehreren Quellen gleichzeitig aufnehmen und in einer Datei speichern.
- Aufnahmeformat WAV oder MP3 in den Audio-Einstellungen oder direkt im Audio-Rad wählen.
- Gespeicherte Aufnahmen über das Audio-Rad im Explorer finden.
- Aufnahmeordner, Sprache, Radgröße und Windows-Start einstellen.
- Updates direkt in Omega Orbit herunterladen und installieren.
