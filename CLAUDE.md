# CE Website – persönliche Website von Cornelis Ebel

Privater Auftritt, ergänzt das LinkedIn-Profil. Kommunikation mit Cornelis: Deutsch, Du-Form.

## Entscheidungen (20.11.2026)
- **Stack:** statisches HTML/CSS/JS, keine Build-Tools, kein npm, keine Frameworks.
- **Hosting (geplant):** GitHub Pages. Noch nicht veröffentlicht. Deploy, Repo auf GitHub, Accounts oder Domain-Kauf nur nach Cornelis' ausdrücklichem OK.
- **Domain:** noch keine. Erst `<user>.github.io`, eigene Domain kann später dazu (dann `CNAME`-Datei + DNS).
- **Umfang:** Onepager (`index.html`) plus `impressum.html` und `datenschutz.html`.
- **Stil:** hell und minimal, Editorial-Look. Systemschriften (keine Google Fonts, keine externen Requests, kein Tracking, keine Cookies). Das hält die Datenschutzerklärung schlank.

## Struktur
- `index.html` – Hero, Über mich, Themen, Werdegang, Projekte, Kontakt
- `impressum.html`, `datenschutz.html` – Rechtstexte mit Platzhaltern `[bitte ergänzen]`
- `assets/style.css` – alle Styles, Farben als CSS-Variablen in `:root`
- `assets/main.js` – nur Kleinkram (Jahr im Footer, Mobile-Menü)
- `assets/portrait.jpg` – Porträtfoto (kommt noch; bis dahin Platzhalter mit Initialen in `index.html`)

Lokal ansehen: `index.html` im Browser öffnen oder `python3 -m http.server 8000` im Ordner und `http://localhost:8000`.

Hinweis: Der Vorschau-Runner der Claude-App darf auf macOS nicht direkt im Desktop-Ordner starten. Deshalb den Server per Terminal/Bash im Hintergrund starten; `.claude/launch.json` hängt sich nur an `http://localhost:8000` an.

## Veröffentlichen (erst nach Cornelis' OK)
1. Leeres Repo auf GitHub anlegen (z. B. `cornelisebel.github.io` → Seite liegt dann direkt unter dieser Adresse).
2. `git remote add origin …` und `git push -u origin main`.
3. GitHub → Settings → Pages → Source „Deploy from a branch“, Branch `main`, Ordner `/ (root)`.
4. Vorher: Impressum/Datenschutz ausgefüllt, `noindex` dort entfernt.

## Harte Inhaltsregeln
- **SuperNurse** nur als normale Station im Werdegang (Rolle, Zeitraum). Keine Kunden, Preise, Kennzahlen, Interna, Prozesse.
- **„Cornelis Ebel - Ventures“** wird nicht genannt.
- **SuperNurse-Mailadresse** kommt nicht auf die Seite. Kontakt läuft über LinkedIn.
- **Impressum/Datenschutz:** Angaben (Name, Anschrift, Kontakt) liefert Cornelis selbst. Nichts erfinden, Platzhalter stehen lassen, bis er sie liefert. Seiten nicht live schalten, solange Platzhalter drin sind.
- Keine erfundenen Zahlen oder Projekte. Belegbare Fakten nur aus dem LinkedIn-Projekt.

## Quellen (nur lesen, dort nichts ändern)
`/Users/cornelisebel/Desktop/LinkedIN`
- `01_Strategie/positionierung.md` – Kernthese, 3 Themen, Alleinstellung
- `02_Profil/PROFIL_NEU.md` – Werdegang, Info-Text (Stand: noch nicht final)
- `07_Ressourcen/stimme-und-stil.md` – Tonalität
- `tools/linkedin/ANLEITUNG.md` – LinkedIn-Connector (Projektbeschreibung)

## Ton
Direkt, nahbar, konkret. Keine KI-Floskeln („Lass uns eintauchen“, „Game Changer“), keine Emoji-Wände. Pfeile (→) sparsam als Stilmittel ok.

## Offene Punkte
- Porträtfoto
- Impressum-/Datenschutz-Angaben
- LinkedIn-URL: aktuell `linkedin.com/in/cornelis-ebel-a3a820288`; falls die Vanity-URL `/cornelis-ebel` kommt, in `index.html` und Footer der Unterseiten ersetzen
- Werdegang abgleichen, sobald `PROFIL_NEU.md` final ist
