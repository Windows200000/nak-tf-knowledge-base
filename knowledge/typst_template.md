# NAK Typst template — what it is and where it deviates from NAK formalia

**Source:** [originals/nak-typst-template-main/](<../originals/nak-typst-template-main/>) (MIT licence, © 2025 Leon Heuer; upstream `github.com/heuerleon/nak-typst-template`). The README calls it an *"Officially approved template for Nordakademie transfer papers"*. Note that the NAK FAQ says NAK itself provides **no** templates on purpose and points to student templates.

## Layout of the template

| Path | Purpose |
|---|---|
| `src/main.typ` | Entry point: `transfer_paper.with(language, "<TF-Nr>", "<Matrikelnr>", "<Thema>", "<Studiengang, Zenturie>", appendix_content: include "chapters/99_appendix.typ")`, then `#include` the chapters |
| `src/const.typ` | `language = "de"` / `"en"`; NAK blue `rgb(8,31,92)` |
| `src/components/transfer_paper.typ` | The document layout: cover → TOC → lists of figures/tables/listings → abbreviations (Roman page numbers) → body (Arabic, from 1, headings `1.1`, justified) → bibliography → appendix (`A.1`) |
| `src/pages/cover.typ` | Cover page matching the official Deckblatt fields (Transferleistung Theorie/Praxis Nr., Matrikelnummer, Freigegebenes Thema, Studiengang/Zenturie). **No name field** (good for double-blind) |
| `src/abbreviations.typ` | Glossary entries (glossarium package) |
| `src/ai_documentation.typ` + `components/ai_table.typ` | **KI-Prozessdokumentation table** in the appendix. Each entry: `date` (YYYY-MM-DD), `query`, `reason`, `quality`, `software`; all required (compile fails otherwise). Matches the 4 NAK columns |
| `src/res/literature.bib` | BibTeX bibliography |
| `src/components/code.typ`, `tables.typ`, `formatting.typ` | Helpers for code listings (zebraw), tables, text |
| `src/chapters/*.typ` | Example chapters (citing, code, tables) |
| `src/res/header_de.png`, `header_en.png`, `nordakademie_logo.png` | Page header graphics |

Packages: `@preview/zebraw:0.5.5`, `@preview/glossarium:0.5.8`. Build: `typst compile src/main.typ` (or the typst.app web editor / VS Code with Tinymist). The README mentions `main_de.typ`/`main_en.typ`, but the actual file is `main.typ`.

## ⚠ Defaults that deviate from NAK formal requirements

Compare with [formal_requirements.md](formal_requirements.md). Check and override these before submitting:

| Setting (in `transfer_paper.typ`) | Template default | NAK requirement | Fix |
|---|---|---|---|
| `font_size` / font | 12 pt, body font = Typst default (Libertinus Serif) | **Times New Roman 12 pt or Arial 11 pt** | `set text(font: "Times New Roman")` (or Arial + 11 pt) |
| `margin_y` | **3 cm** | **2 cm all sides** | `margin_y: 2cm` |
| line spacing | not set (Typst default leading ≈ 0.65 em) | **1,25** | set `par(leading: …)` to approximate 1.25 line spacing and verify visually |
| hyphenation | not explicitly enabled | **Blocksatz mit Silbentrennung** | `set text(hyphenate: true)`, `set par(justify: true)` (justify is already on in the body) |
| `citation_style` | **"ieee"** (numeric) | *"übliche Zitierweise aus dem jeweiligen Fachgebiet"*, uniform | For WI/business, author-year styles (APA/Harvard) are more usual; pick one, see [citation/README.md](citation/README.md) |
| Level-1 headings | forced page break | free choice; NAK says new pages per chapter are usually not needed for short TFs | Optional: remove `pagebreak(weak: true)` |
| Abbreviation list | always printed | only if needed; no trivial abbreviations | Keep the list short |

**Placement of the AI documentation.** The template renders the KI-Prozessdokumentation *inside the TF's appendix* (`99_appendix.typ`). The NAK sources are ambiguous on this:
- The FAQ says the Prozessdokumentation must be submitted *"neben den Dokumenten Transferleistung und Selbstreflexion"* in CIS, which reads like a separate upload.
- Formale Anforderungen 2026 says *"Prozessdokumentation über KI-Nutzung anfügen"* (attach).

The safe option is both: keep it in the appendix and also upload it separately if CIS offers a slot.

Things it gets right: Roman/Arabic page numbering, separate lists, no name on the cover, an appendix after the bibliography, and the AI documentation table.

**Page counting:** Typst does not count "Textseiten" for you. NAK's 10 ± 10 % excludes lists, appendix, figures and code but includes self-made tables. Count manually.
