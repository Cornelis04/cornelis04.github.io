# CE Website – persönliche Website von Cornelis Ebel

Privater Auftritt, ergänzt das LinkedIn-Profil. Kommunikation mit Cornelis: Deutsch, Du-Form.

## Entscheidungen (20.11.2026)
- **Stack:** statisches HTML/CSS/JS, keine Build-Tools, kein npm, keine Frameworks.
- **Hosting:** GitHub Pages, live unter https://cornelis04.github.io (Repo `Cornelis04/cornelis04.github.io`, öffentlich). Am 20.11.2026 kurz offline/privat, am selben Tag auf Cornelis' Wunsch wieder online. Jeder `git push` auf `main` geht nach ca. 1 Minute live, deshalb nur nach Cornelis' OK pushen. Eigene Domain und neue Accounts nur nach seinem ausdrücklichen OK.
- **Domain:** noch keine eigene. Kann später dazu (dann `CNAME`-Datei + DNS beim Domain-Anbieter + Eintrag unter Settings → Pages).
- **Umfang:** Onepager (`index.html`) plus `impressum.html` und `datenschutz.html`.
- **Stil:** hell und minimal, Editorial-Look. Systemschriften (keine Google Fonts, keine externen Requests, kein Tracking, keine Cookies). Das hält die Datenschutzerklärung schlank.

## Struktur
- `index.html` – Hero, Über mich, Themen, Werdegang, Projekte, Kontakt
- `impressum.html`, `datenschutz.html` – Rechtstexte (ausgefüllt)
- `assets/style.css` – alle Styles, Farben als CSS-Variablen in `:root`
- `assets/main.js` – nur Kleinkram (Jahr im Footer, Mobile-Menü)
- `assets/portrait.jpg` – Porträtfoto (LinkedIn-Profilfoto, 800×800)

Lokal ansehen: `index.html` im Browser öffnen oder `python3 -m http.server 8000` im Ordner und `http://localhost:8000`.

Hinweis: Der Vorschau-Runner der Claude-App darf auf macOS nicht direkt im Desktop-Ordner starten. Deshalb den Server per Terminal/Bash im Hintergrund starten; `.claude/launch.json` hängt sich nur an `http://localhost:8000` an.

## Veröffentlichen
Änderung committen, dann `git push` (nur nach Cornelis' OK). Build-Status: `gh run list -L1`.
Offline nehmen: Pages lässt sich bei `<user>.github.io` nicht abschalten → Repo umbenennen (`gh repo rename ce-website`), dann `gh api -X DELETE repos/Cornelis04/ce-website/pages`.

## Interview (privat)
`_interview/INTERVIEW.md` – großes Interview zu Zielen, Werdegang, Projekten, Meinungen und LinkedIn-Feinschliff. Steht in `.gitignore`, weil das Repo öffentlich ist: **nie committen**. Antworten mit `[intern]` nur als Hintergrund nutzen, nie veröffentlichen.

## Harte Inhaltsregeln
- **SuperNurse** nur als normale Station im Werdegang (Rolle, Zeitraum). Keine Kunden, Preise, Kennzahlen, Interna, Prozesse.
- **„Cornelis Ebel - Ventures“** wird nicht genannt.
- **SuperNurse-Mailadresse** kommt nicht auf die Seite. Kontakt läuft über LinkedIn.
- **Impressum/Datenschutz:** Angaben hat Cornelis am 20.11.2026 geliefert (private Anschrift Meerbusch, GMX-Adresse). Änderungen daran nur mit seinen Angaben, nichts erfinden.
- Keine erfundenen Zahlen oder Projekte. Belegbare Fakten nur aus dem LinkedIn-Projekt.

## Quellen (nur lesen, dort nichts ändern)
`/Users/cornelisebel/Desktop/Claude Master/SN Account/CE LinkedIN`
- `01_Strategie/positionierung.md` – Kernthese, 3 Themen, Alleinstellung
- `02_Profil/PROFIL_NACHBAU.md` – offene LinkedIn-Entscheidungen Block A–G
- `02_Profil/PROFIL_NEU.md` – Werdegang, Info-Text (Stand: noch nicht final)
- `07_Ressourcen/stimme-und-stil.md` – Tonalität
- `tools/linkedin/ANLEITUNG.md` – LinkedIn-Connector (Projektbeschreibung)

## Ton
Direkt, nahbar, konkret. Keine KI-Floskeln („Lass uns eintauchen“, „Game Changer“), keine Emoji-Wände. Pfeile (→) sparsam als Stilmittel ok.

## Offene Punkte
- Prüfen, ob `cornelis.ebel@gmx.de` erreichbar ist (laut LinkedIn-Projekt war eine alte GMX-Adresse nicht erreichbar)
- LinkedIn-URL: aktuell `linkedin.com/in/cornelis-ebel-a3a820288`; falls die Vanity-URL `/cornelis-ebel` kommt, in `index.html` und Footer der Unterseiten ersetzen
- Werdegang abgleichen, sobald `PROFIL_NEU.md` final ist
