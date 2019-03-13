# hoerbert
Ein Skript um unter Linux Playlists für den Hörbert zu erstellen

### Voraussetzungen
* `cdparanoia`
* `sox`

### Vorbereitung
* Speicherkarte in den Computer stecken
* Konfigurationvorlage `.config.template` kopieren zu `.config` und Pfad zur Speicherkarte anpassen (`BASE_DIR`)

### Benutzung
* CD einlegen
* Skript starten mit `./hoerbert_playlist`
* Nummer der Playlist eingeben: [0..8]
* Ist die Playlist leer: Erstellung der Playlist startet automatisch
* Ist die Playlist bereits gefüllt: Auswählen ob neue Musik hinzugefügt werden soll: [J/n]

### Ablauf
* Konvertierung der CD in wav Dateien mit cdparanoia
* Konvertierung und Umbennennung der wav Dateien in das Hörbert Format
* Verschieben der wav Dateien auf die Speicherkarte in die gewählte Playlist
