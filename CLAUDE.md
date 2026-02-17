# Prompt Verzameling

## Wat is dit?
Interactieve Nederlandse prompt-collectie als webpagina. Gebouwd als product voor eigen gebruik en om te delen met AI workshop-klanten.

## Eigenaar
André Bergsma — Massoeba

## Doelgroep
- **Level 2 (AI Practitioner):** Dagelijkse AI-gebruikers die transitie maken naar Claude Code
- **Level 3 (AI Native):** Bouwen eigen tools, multi-agent workflows
- **Niet** voor beginners — daar komt later een aparte versie voor

## Gebaseerd op
- "The Cloned Consultant" bonussen van Pip Decks (Bonus 1-4)
- Bronbestanden staan in `/Claudeprojects/AI cloned consultant bonuses/`
- Eigen categorieën, eigen toevoegingen, eigen structuur — geen kopie van het origineel

## Technisch

| | |
|---|---|
| **Type** | Enkel HTML-bestand met inline CSS + JS |
| **Frameworks** | Geen — puur HTML/CSS/JS |
| **Hosting** | Vercel (auto-deploy bij push naar main) |
| **Code opslag** | GitHub: github.com/AndreBMas/prompt-verzameling |
| **Live URL** | https://prompt-verzameling.vercel.app |
| **Later** | Subdomein prompts.massoeba.nl koppelen |

## Hoe het werkt
1. Code staat op GitHub (github.com/AndreBMas/prompt-verzameling)
2. Vercel is gekoppeld aan de `main` branch
3. Bij elke push gaat het automatisch live (1-2 min)

## Bestandsstructuur
```
prompt-verzameling/
├── index.html              <- Prompt Verzameling pagina (CSS + JS + content)
├── ai-cheatsheet.html      <- AI Cheat Sheet (printbare A4 referentiekaart)
├── CLAUDE.md               <- Dit bestand
└── .gitignore
```

## Inhoud van de pagina

### 7 categorieën (eigen indeling, niet van het origineel)
| Categorie | Wat | Aantal prompts |
|---|---|---|
| Instappen | Claude Code oriëntatie, CLAUDE.md, eerste project | 9 (I1-I9) |
| Maken | Websites, tools, formulieren, dashboards | 10 (M1-M10) |
| Schrijven | E-mails, voice training, content | 6 (S1-S6) |
| Slim werken | Data, automatisering, rapportages | 8 (SW1-SW8) |
| Fixen | Debuggen, foutmeldingen, setup troubleshooting | 7 (F1-F7) |
| Ontdekken | Verrassingen, audits, 30-min builds, leren | 7 (O1-O7) |
| Bijsturen | Magic phrases, principes, spiraalherkenning | 6 (B1-B6) + extras |

### Extra secties
- **10 Magic Phrases** — korte zinnen die altijd werken
- **8 Prompting Principes** — de regels achter de prompts
- **3 Soorten vragen** — Task / Outcome / Explore framework
- **8 Prompt Chains** — workflows van meerdere stappen (5 origineel + 3 nieuw)
- **4 Industrie Packs** — Coaches (5), Agency (5), Freelancers (5), Corporate (5)

### Totaal: 60+ prompts, 10 magic phrases, 8 chains, 8 principes

## Features
- Zoekfunctie (doorzoekt titels, beschrijvingen, content)
- Categorie-filter knoppen
- Dark/light mode met localStorage
- Kopieer-knop per prompt (NL en EN apart)
- Tool-tags: "Claude Code" vs "Elke AI"
- Inklapbare tips en fix-prompts per prompt
- Responsive (mobiel + desktop)

## Elke prompt heeft
- Titel + "wanneer gebruik je dit"
- Nederlandse versie + kopieer-knop
- Engelse versie + kopieer-knop
- Tip (inklapbaar)
- Fix-prompt als het misgaat (inklapbaar, niet bij allemaal)
- Tool-tag (Claude Code of Elke AI)

## Relatie met andere projecten
- **massoeba-site**: apart project, aparte repo. Prompt Verzameling is GEEN onderdeel van de website
- **ai-workshops**: het business plan voor workshops. Prompt Verzameling is een product dat je kunt inzetten bij Level 2/3 workshops
- **AI cloned consultant bonuses**: bronmateriaal (PDF's). Staat los, geen repo

## Regels voor wijzigingen
- Alles zit in één bestand (index.html) — geen externe bestanden
- Houd de inline CSS + JS structuur aan (geen losse bestanden tenzij noodzakelijk)
- Nieuwe prompts volgen het patroon: titel, wanneer, NL prompt, EN prompt, tip, fix-prompt
- Data-attributes: `data-category` voor filters, `data-searchable` voor zoektrefwoorden
- Tool-tags: `<span class="tool-tag cc">Claude Code</span>` of `<span class="tool-tag all">Elke AI</span>`

## AI Cheat Sheet (ai-cheatsheet.html)
- Standalone printbare A4 referentiekaart
- Gebaseerd op "The Cloned Consultant" bonussen (Pip Decks cursus)
- Twee kolommen: links 4 stappen + 10 magische zinnen, rechts 8 gekleurde tip-boxen
- Massoeba huisstijl (kleuren, fonts, tone of voice)
- Standalone HTML met embedded CSS, geen JS (behalve print-knop)
- Google Fonts: Plus Jakarta Sans + Inter
- Print-optimalisatie: `@page { size: A4 }`, `print-color-adjust: exact`
- Status: bijna klaar, laatste finetuning op A4-fitting

## Nog te doen
- [ ] Review: samen prompt-verzameling content doorlopen en checken
- [ ] AI Cheat Sheet: laatste finetuning A4-fitting
- [ ] Beginners-versie maken (apart product, later)
- [ ] Subdomein prompts.massoeba.nl koppelen (DNS Cloud86 + Vercel)
- [ ] Eventueel linken vanuit massoeba.nl of workshop-materiaal
