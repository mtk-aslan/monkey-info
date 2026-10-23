# MONKEY – öffentliche Informationsseiten

Dieses Repository enthält ausschließlich Datenschutz- und Supportseiten für MONKEY. Der App-Quellcode bleibt im separaten privaten Repository.

Die Datenschutzerklärung enthält noch die unter „Noch ergänzen“ aufgeführten Platzhalter für Hosting- und Aufbewahrungsangaben.

## Dateien

- `privacy.html`: Datenschutzerklärung für Offline-Spiel, den Online-Server auf Render und die Informationsseiten.
- `support.html`: Kontaktvorlage und Spielhilfe.
- `index.html`: Startseite mit Links auf beide Dokumente.
- `.nojekyll`: GitHub Pages soll die HTML-Dateien unverändert ausliefern.

## Bereits übernommen

- Anbieter: **MTK Consulting**, Deutschland (Angabe des Betreibers).
- Öffentliche Kontakt-E-Mail: **kdeux2011@gmail.com**.
- Eine Postanschrift wird auf Wunsch des Betreibers nicht veröffentlicht. Für einen geschäftlichen Auftritt in Deutschland kann eine Anschrift in einer Anbieterkennzeichnung erforderlich sein; vor der endgültigen Verwendung prüfen.
- Online-Spielserver: **Render**, Serverregion **Frankfurt, Deutschland** (Angabe des Betreibers).

## Noch ergänzen

| Platzhalter | Erforderliche Angabe |
| --- | --- |
| `{{ONLINE_HOST_AND_LOG_RETENTION}}` | Noch offene technische Protokollierung, Aufbewahrung und gegebenenfalls Übermittlungen bei Render; Anbieter und Frankfurt sind bereits eingetragen |
| `{{HOSTING_PROVIDER_AND_LOG_RETENTION}}` | GitHub Pages als Anbieter der Informationsseiten, tatsächliche technische Datenverarbeitung und Aufbewahrung laut Anbieter |
| `{{SUPPORT_RETENTION_POLICY}}` | Tatsächliche Lösch-/Aufbewahrungspraxis für Support-Anfragen |

Nur Angaben eintragen, die öffentlich sichtbar sein sollen. Keine Passwörter, Tokens, Signierschlüssel oder privaten App-Konfigurationen hier ablegen. GitHub-Commits können frühere Fassungen langfristig sichtbar halten.

Nach Vervollständigung alle `{{…}}`-Platzhalter prüfen und den Datenschutzhinweis mit dem tatsächlichen Betrieb abgleichen. Der Spielserver verarbeitet die Partie im RAM; Render- und GitHub-Protokolle sind davon getrennt. Diese Vorlage ersetzt keine Prüfung der konkreten Betreiberangaben.

## GitHub Pages aktivieren

1. Im Repository **Settings → Pages** öffnen.
2. Unter **Build and deployment** als Source **Deploy from a branch** wählen.
3. Branch **main**, Ordner **/ (root)** auswählen und **Save** anklicken.
4. Nach erfolgreicher Veröffentlichung die URLs ohne Anmeldung prüfen:
   - Datenschutz: <https://mtk-aslan.github.io/monkey-info/privacy.html>
   - Support: <https://mtk-aslan.github.io/monkey-info/support.html>
   - Startseite: <https://mtk-aslan.github.io/monkey-info/>

Das Hochladen der Dateien aktiviert GitHub Pages nicht automatisch. Der enthaltene `noindex,nofollow`-Hinweis bittet Suchmaschinen, die Seiten nicht zu indexieren; er schützt nicht vor öffentlichem Zugriff.

Nach Fertigstellung die Datenschutz- und Support-URL in App Store Connect und in den MONKEY-Releaseangaben hinterlegen. Die eigene Domain und die Render-Konfiguration müssen dafür nicht geändert werden.
