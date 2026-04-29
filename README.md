# ElsterSide Studios — Website

**Live:** [elstersidestudios.de](https://elstersidestudios.de)  
**Repo:** github.com/elstersidestudios/elsterside-site  
**Deploy:** GitHub Pages — automatisch bei jedem Push auf `main`

---

## Seiten

| Datei | URL | Status |
|---|---|---|
| `index.html` | elstersidestudios.de | ✅ Live |
| `companies.html` | elstersidestudios.de/companies.html | ✅ Live |
| `mixing.html` | elstersidestudios.de/mixing.html | ✅ Live |
| `impressum.html` | elstersidestudios.de/impressum.html | ✅ Live |

---

## Assets

| Datei | Verwendung | Größe |
|---|---|---|
| `hero.jpg` | Homepage Hero (Karl-Heine-Kanal) | ~500KB |
| `studio-hero.jpg` | Mixing Page Hero | — |
| `companies-hero.jpg` | Companies Hero (Bar, Qui Nguyen/Unsplash) | ~500KB |
| `portrait.jpg` | Studio-Section auf Mixing Page | — |
| `logo.svg` | Navigation alle Seiten | — |
| `og-image.jpg` | Social Preview alle Seiten (1200×630) | 139KB |

---

## Technische Entscheidungen

- **Sprache:** EN/DE Toggle via `body.lang-en` / `body.lang-de` + localStorage. Startet auf Browsersprache.
- **Logo:** `<img src="logo.svg">` mit CSS `filter: brightness(0) invert(1)` für weiße Darstellung
- **Ken Burns:** zoom-out auf companies, zoom-in auf mixing + index
- **OG Tags:** Alle Seiten haben Open Graph + Twitter Card Meta-Tags
- **Fonts:** Playfair Display, JetBrains Mono — Google Fonts
- **Farben:** `--amber: #b5662a` · `--cream: #eee9e3` · `--ink: #090e14`

---

## Workflow

1. Claude holt Dateien via GitHub API (Token erforderlich — siehe Notion)
2. Claude bearbeitet lokal, pusht direkt auf `main`
3. GitHub Pages deployed automatisch (~30 Sekunden)

**Token-Speicherort:** Notion → ElsterSide HQ → Website Projekt → GitHub Token

---

## Noch offen

- [ ] Testimonials / echte Kundenzitate
- [ ] mixing.html Content-Review
- [ ] Studio-Page
