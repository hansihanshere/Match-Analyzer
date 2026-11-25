# Match Analyzer PWA

## Funktionen
- Spieluhr mit Anstoß, Halbzeit, zweiter Halbzeit und Abpfiff
- Tore, Gegentore, Video-Marker und Notizen per Schnellbutton
- automatische Spielzeit plus Korrektur um ±5/±10 Sekunden
- Veo-Arbeitsliste mit einstellbarem Vorlauf
- Torzeiten, Torarten, Gegentorursachen und letzte 5 Spiele
- lokale Speicherung, Offline-Betrieb sowie JSON-Export/Import

## Kostenlos über GitHub Pages veröffentlichen
1. Auf GitHub ein neues Repository erstellen, z. B. `match-analyzer`.
2. Alle Dateien aus diesem Ordner in die oberste Ebene des Repositorys hochladen.
3. Unter **Settings > Pages** bei **Build and deployment** `Deploy from a branch` wählen.
4. Branch `main`, Ordner `/(root)` wählen und speichern.
5. Nach der Bereitstellung die angezeigte HTTPS-Adresse auf dem Android-Handy in Chrome öffnen.
6. Chrome-Menü > **App installieren** oder **Zum Startbildschirm hinzufügen**.

## Wichtig zur Datenspeicherung
Die Daten liegen ausschließlich im Browser des jeweiligen Geräts. Nutze unter **Mehr > Daten exportieren** regelmäßig ein Backup. Beim Löschen der Browserdaten können sonst alle Einträge verloren gehen. Für den Umzug auf ein anderes Gerät: Exportdatei übertragen und dort importieren.

## Test auf dem PC
Im Ordner `python -m http.server 8080` starten und anschließend `http://localhost:8080` öffnen. Nicht per Doppelklick starten, weil der Service Worker dafür HTTP/HTTPS benötigt.

## Vorbelegte Saison
Diese Version enthält alle 26 Kreisliga-2-Spiele des SV Tennenlohe 2026/27. Für Spieltage 1 bis 15 sind die bekannten Endergebnisse hinterlegt. Die exakten Torzeiten wurden nicht erfunden; daher fließen die Ergebnisse in die Gesamtstatistik ein, aber noch nicht in die Torzeitfenster. Sobald Torereignisse mit Zeiten ergänzt werden, werden die Zeitdiagramme daraus berechnet.
