# Changelog

## [0.9.0] - 2026-11-10

#### Hinzugefügt
- **Radio-Plugin**: Neues eigenständiges Plugin für Internetradio direkt im Orbit-Rad.
- **Sendersuche & Vorschau**: Weltweite Radiosender nach Name, Genre, Land oder Beliebtheit durchsuchen und direkt per Klick vorhören.
- **Senderfavoriten im Rad**: Lieblingssender zur persönlichen Favoritenliste hinzufügen und direkt aus dem Orbit-Rad starten.
- **Satelliten-Player**: Kompakter Radio-Player, der sanft am Orbit-Rad andockt, mit gedrückter Maustaste um das Rad bewegt oder frei auf dem Desktop platziert werden kann.
- **Timeshift-Puffer**: Bis zu 3 Minuten Puffer zum flexiblen Vor- und Zurückspringen im laufenden Radioprogramm sowie Sofort-Rückkehr zu LIVE.
- **Song-Erkennung & Export**: Erkennt laufende Musiktitel aus dem Radiostream und speichert beliebige Songs mit einem Klick verlustfrei als Audiodatei.
- **Radio-Aufnahme**: Komplette Radiosendungen mitschneiden und wahlweise als Original-Stream, MP3, WAV oder FLAC abspeichern.
- **Eigenes Audio-Ausgabegerät**: Der Radio-Player kann auf ein separates Audiogerät gelegt werden (z. B. GoXLR Music-Kanal oder Kopfhörer), ohne andere Systemsounds zu verändern.
- **Lautstärkeregelung per Mausrad**: Durch Scrollen über dem Lautstärkeregler lässt sich die Lautstärke in 10%-Schritten (oder feinen 2%-Schritten mit Umschalttaste) anpassen.
- **Reaktiver Beat-Puls**: Optionaler Regenbogen-Puls am Rahmen des Players, der synchron zum Rhythmus der Musik leuchtet.
- **Detaillierte Sitzungsprotokolle**: Umfassende Protokollanzeige in den Einstellungen mit farbigen Zähler-Badges für Info, Warnungen und Fehler.

#### Geändert
- **Aufnahme-Sicherheit**: Stoppen und Speichern von Aufnahmen schlagen auch bei unerwartetem Ausfall einzelner Audioquellen nicht mehr fehl.
- **Sicheres Speichern**: Bestätigte Zielaufnahmen werden über geschützte Zwischenkopien ersetzt, um Datenverlust bei vollen Datenträgern auszuschließen.
- **Datenschutz in Protokollen**: Persönliche Benutzerpfade und Zugangsdaten werden in allen Fehlerprotokollen automatisch unkenntlich gemacht.

#### Behoben
- **Satelliten-Verzögerung**: Der Radio-Player und die Sendersuche folgen dem Verschieben des Orbit-Rads jetzt nahtlos ohne Verzögerung.
- **Fenstergröße der Sendersuche**: Die Sendersuche öffnet sich zuverlässig in fester Größe, ohne sich unbeabsichtigt aufzuschaukeln.
- **Play/Pause-Umschaltung**: Der Play/Pause-Button schaltet beim Pausieren und Fortsetzen sofort synchron zwischen Play- und Pause-Symbol um.
- **Höhe des Radio-Players**: Das Player-Fenster passt seine Höhe beim Öffnen der Titelliste automatisch an, sodass alle Bedienelemente bedienbar bleiben.

## [0.8.15] - 2026-11-08

#### Hinzugefügt
- **Videoaufnahme**: Bildschirm-, Kamera- und Overlay-Aufnahmen sind jetzt verfügbar. Systemton, Mikrofon und weitere Geräte oder Apps lassen sich gemeinsam aufnehmen.
- **Kamera-Vorschau in groß**: Die Kameraeinstellungen lassen sich in einer großen Vorschau bearbeiten. Zwischen dem Overlay in der Bildschirmaufnahme und einer reinen Kameraansicht kann direkt umgeschaltet werden.
- **Aufnahme mit oder ohne Kamera**: Beim Start einer Bildschirmaufnahme im Rad lässt sich vorher festlegen, ob die Kamera eingeblendet wird. Die Auswahl gilt auch für die Einstellungen.
- **Kompakte Zahlenfelder**: Kameraposition, Größe, Ausschnitt und Synchronisation lassen sich präzise mit Zahlenfeldern und Plus/Minus-Tasten einstellen. Gedrückthalten wiederholt die Änderung.

#### Geändert
- **Video-Einstellungen neu organisiert**: Klare Bereiche für Bildschirm, Audio, Qualität, Format, Speichern und Kamera. Aufgeräumte Karten, besserer Kontrast und besser lesbare Schrift.
- **Kamera-Overlay**: Die Kamera lässt sich frei positionieren, skalieren, zuschneiden und als Rechteck, abgerundetes Rechteck, Kreis oder eigene PNG-Maske einblenden.
- **Getrennte Anzeigegrößen**: Die Größe im Bildschirm-Overlay und in der reinen Kamera-Vorschau sind unabhängig einstellbar.
- **Kamera-Synchronisation**: Die Kamera-Latenz im Overlay wird automatisch ausgeglichen, damit Kamerabild und Stimme zusammenpassen.

#### Behoben
- **Ton und Bild starten synchron**: Bildschirm-, Kamera- und Audioaufnahmen beginnen jetzt gemeinsam; der Ton läuft nicht mehr voraus.
- **Kamera-Overlay erscheint zu spät**: Das Kamerabild im Overlay wird um die gemessene Verzögerung ausgeglichen.
- **Kamera-Vorschau setzt aus**: Doppelte Vorschauverbindungen wurden entfernt; die Vorschau läuft stabiler.
- **Große Kameraansicht springt**: Kein Scrollen und kein Springen mehr beim Wechsel zwischen Overlay und reiner Kameraansicht.
- **Kamera-Zuschnitt und Maske**: Der Zuschnitt verändert nicht mehr die Maske; das Kamerabild wird vor der Maske beschnitten.

## [0.8.14] - 2026-11-06

#### Hinzugefügt
- **Aufgeräumte Seitenleiste**: Die Einstellungen sind jetzt in die Bereiche „Rad & Allgemein“ und „Inhalte“ gegliedert. Beide Bereiche lassen sich unabhängig auf- und zuklappen, mehrere können gleichzeitig offen bleiben.
- **Direkte Sprünge**: Ein Klick auf einen Eintrag in der Seitenleiste öffnet sofort die passende Einstellungsseite beziehungsweise den passenden Unterbereich.
- **Passende Fensterbreite**: Das Einstellungsfenster passt seine Breite automatisch so an, dass alle Reiter sichtbar sind – ohne manuelles Ziehen oder horizontales Scrollen.

#### Geändert
- **Rad-Layout unter „Rad & Allgemein“**: Die Anordnung der Rad-Kacheln ist jetzt unter „Rad & Allgemein → Rad-Layout“ zu finden statt unter Plugins.
- **Plugins als ein Eintrag**: In der Seitenleiste gibt es nur noch „Plugins“. Plugin-Verwaltung, Audio & Quellen und Video & Aufnahmen sind als Reiter innerhalb der Plugins-Seite angeordnet.
- **Schnellerer App-Starter**: Beim Öffnen des App-Starters friert die Anwendung nicht mehr ein; installierte Apps werden im Hintergrund eingelesen.

#### Behoben
- **Unnötige Lücke in der Seitenleiste**: Der Plugins-Eintrag steht jetzt direkt unter „Hilfe & Protokoll“ statt mit großem Abstand am unteren Rand.

#### Entfernt
- **Hinweis zur Rad-Kapazität**: Der erklärende Kasten im App-Starter wurde entfernt; die Seite beginnt direkt mit den konfigurierten Apps.

## [0.8.13] - 2026-11-06

#### Hinzugefügt
- **Plugin-Verwaltung**: In den Einstellungen lassen sich Funktionen wie die Audioaufnahme bequem ein- und ausschalten. Der neue Bereich „Plugins“ steht ganz unten in der Seitenleiste; die zugehörigen Einstellungen erscheinen direkt darunter.
- **Eigenes Rad-Layout**: Die Reihenfolge der Kacheln und ihre Verteilung auf die Seiten des Orbit-Rads lassen sich frei anpassen. „Standard wiederherstellen“ setzt alles zurück.

#### Geändert
- **Aufnahme als eigenständige Funktion**: Die Audioaufnahme ist jetzt als Plugin organisiert und kann unabhängig verwaltet werden. Die Videoaufnahme ist für eine spätere Version vorbereitet, in 0.8.13 aber standardmäßig deaktiviert.
- **Aufgeräumte Einstellungen**: Der Plugins-Bereich steht am Ende der Einstellungen; die zugehörigen Unterbereiche erscheinen nur, wenn die Funktion aktiviert ist.

#### Behoben
- **Leere Aufnahme-Kachel**: Wenn Audio- und Videoaufnahme beide deaktiviert sind, wird die Aufnahme-Kachel vollständig aus dem Rad entfernt statt als leerer Eintrag stehen zu bleiben.

## [0.8.11] - 2026-11-04

#### Hinzugefügt
- **Kameraränder zuschneiden**: Linker, rechter, oberer und unterer Rand lassen sich separat entfernen, ohne den übrigen Bildinhalt zu vergrößern.

#### Geändert
- **Übersichtliche Kameraeinstellungen**: Kameraauswahl nur noch im Kamera-Reiter; Darstellung, Zuschnitt, Anzeige und Satellit sind in aufklappbare Bereiche gegliedert.
- **Einheitliches Aufnahmesymbol**: Ein roter Punkt mit weißem REC kennzeichnet die Aufnahme unabhängig von der Aufnahmeart. Interne Symbole sind farbig gestaltet.

#### Behoben
- **Bildschirmzuordnung**: Kleine Rundungsabweichungen bei Bildschirmgrößen verhindern die Auswahl des passenden Monitors nicht mehr.

## [0.8.10] - 2026-11-04

#### Hinzugefügt
- **Mehrere Audioquellen für Videoaufnahmen**: Bis zu 20 Geräte und Apps lassen sich auswählen und mit eigener Lautstärke zusammenmischen.
- **Audioformate einstellen**: MP3-Bitrate sowie Abtastrate und Kanäle sind wählbar; WAV unterstützt zusätzlich 16 und 24 Bit.
- **Mauszeiger aufnehmen**: Der Mauszeiger lässt sich für Bildschirmaufnahmen ein- oder ausschalten.

#### Geändert
- **Übersichtlichere Hilfe und Updates**: Feedback und Support befinden sich bei Hilfe und Protokoll. Update-Einstellungen und Status sind untereinander angeordnet.
- **Aufnahme-Einstellungen**: Audio- und Videoaufnahme haben getrennte Speicherorte und jeweils passende Formateinstellungen.

#### Behoben
- **Mauszeiger bei Bildschirmaufnahmen**: Die Bildschirmaufnahme verwendet einen anderen Aufnahmeweg, um Cursorflackern zu vermeiden und den Mauszeiger weiterhin aufzuzeichnen.
- **Kameravorschau**: Fehler beim Kamerazugriff werden angezeigt und die Vorschau kann erneut geladen werden.
- **Ordnerauswahl**: Der Dialog öffnet sich beim eingestellten Aufnahmeordner.

## [0.8.8] - 2026-11-03

#### Geändert
- **Übersichtliche Aufnahme-Einstellungen**: Quellen, Audio, Video, Formate, Speicherorte und Kamera sind in eigenen Reitern angeordnet.
- **Getrennte Aufnahmeordner**: Für Audio- und Videoaufnahmen lassen sich separate Speicherorte wählen. Der bisherige Ordner wird zunächst für beide übernommen.

#### Behoben
- **Kameravorschau wieder sichtbar**: Die Live-Vorschau wird in den Kamera-Einstellungen wieder angezeigt und beim Verlassen des Kamera-Reiters freigegeben.
- **Kamera-Satellit nur bei Bedarf**: Der Satellit erscheint ausschließlich bei laufender oder pausierter Kameraaufnahme beziehungsweise Bildschirmaufnahme mit Kamera und aktivierter Satellitenanzeige.
- **Orbit bis an die Taskleiste bewegen**: Das sichtbare Rad und ein aktiver Kamera-Satellit lassen sich direkt bis an die Taskleiste verschieben, ohne sie zu überdecken.

## [0.8.7] - 2026-11-03

#### Geändert
- **Frei verschiebbare Hinweisfenster**: Fehler- und Benachrichtigungsdialoge können nun frei mit der Maus auf dem Bildschirm und über mehrere Monitore hinweg verschoben werden.
- **Sicherer Erhalt von Originalaufnahmen**: Beim Umwandeln von MKV- in MP4-Dateien wird die Originalaufnahme vor dem Löschen auf Vollständigkeit aller Spuren geprüft und bei Unstimmigkeiten sicher auf der Festplatte behalten.
- **Zuverlässige Update-Prüfsummen**: Der integrierte Updater gleicht heruntergeladene Aktualisierungen noch robuster mit den veröffentlichten Prüfsummen ab und schützt zuverlässig vor unvollständigen Downloads.

#### Behoben
- **Kamera-Konflikte zwischen Vorschau und Aufnahme behoben**: Die Kamera-Vorschau in den Einstellungen und der Kamera-Satellit am Rad können nun zeitgleich mit Videoaufnahmen aktiv sein, ohne dass die Webcam als belegt gemeldet wird.
- **Schutz laufender Aufnahmen vor Kamerawechsel**: Ein Gerätewechsel der Kamera in den Einstellungen ist während einer aktiven Aufnahme gesperrt, um Abbrüche zu verhindern.
- **Audio bei Videoaufnahmen**: Die Verarbeitung beim Start und Beenden von Videoaufnahmen wurde stabilisiert.
- **Erhalt von Videosegmenten bei unerwarteten Abbrüchen**: Bricht eine Videoaufnahme unerwartet ab, bleiben alle bis dahin aufgezeichneten Segmente sicher auf dem Datenträger erhalten.

## [0.8.6] - 2026-11-03

#### Hinzugefügt
- **H.265 / HEVC-Video-Encoder**: Unterstützung für moderne H.265 / HEVC-Hardware-Beschleunigung (NVIDIA NVENC, Intel Quick Sync, AMD AMF) und CPU-Encoding für kleinere Videodateien bei gleicher Bildqualität.
- **Kamerabild-Zoom und Bildausschnitt**: In den Video-Einstellungen kann das Kamerabild vergrößert und der Bildausschnitt horizontal sowie vertikal verschoben werden, um den gewünschten Bereich exakt einzupassen.
- **Größe und Position des Kamera-Blobs einstellbar**: Neue Schieberegler in den Video-Einstellungen ermöglichen die präzise Anpassung der Blob-Größe und des Winkels am Orbit-Rad.

#### Geändert
- **Klick-Durchlässigkeit um das Orbit-Rad**: Transparente Bereiche außerhalb des Rads und des Kamera-Blobs lassen Mausklicks ungehindert durch, sodass dahinterliegende Fenster und der Desktop direkt bedienbar bleiben.
- **Exakter Andock-Abstand zu den Einstellungen**: Das Orbit-Rad dockt nun mit einem sauberen, gleichmäßigen 16-Pixel-Abstand direkt an das Einstellungsfenster an.
- **Vergrößerte Hinweisfenster**: Fehlermeldungen und Systemhinweise werden nun in einem größeren, scrollbaren Dialogfenster über dem gesamten Bildschirmbereich dargestellt.

#### Behoben
- **Dauerhafte Kamera-Einblendung behoben**: Das Kamerabild am Rad erscheint nun ausschließlich während einer aktiven Kameraaufnahme und wird nach dem Beenden automatisch geschlossen.
- **Live-Vorschau statt Aufnahmezeit im Kamera-Blob**: Während der Aufnahme zeigt der Kamera-Blob das echte Kamerabild anstelle des statischen Aufnahmehinweises.
- **Abschneiden des 16:9-Kamerabilds bei 3 Uhr und 9 Uhr**: Im Querformat wird das Kamerabild auch an den seitlichen Rändern des Rads nicht mehr abgeschnitten.
- **Pufferüberläufe und Aufnahmeabbrüche**: Unerwartete Signal-Abbrüche bei gleichzeitiger Kamera- und Bildschirmaufnahme durch zu kleine Audiopuffer wurden behoben.
- **Wiederherstellung des eingeklappten Rads**: Wurde das Rad eingeklappt, lässt es sich nun jederzeit zuverlässig über das globale Tastenkürzel oder das Taskleistensymbol wieder öffnen.

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
