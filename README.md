# NAK Transferleistungen — Knowledge Base

An organised, AI-ready reference for **creating and reviewing NORDAKADEMIE Transferleistungen** (Theorie/Praxis transfer papers). It is built from the full Moodle "Transferleistungen" course dump (October 2026). **AI assistants: start with [CLAUDE.md](CLAUDE.md).**

## Repository map

```
CLAUDE.md / AGENTS.md      → instructions for AI assistants (task → file routing, rules)
sources/INDEX.md           → catalogue of every original file: what it is, date, caveats, where used
originals/                 → ALL original files, unchanged except one privacy redaction (incl. the 2 user-provided .md conversions)
originals_text/            → plain-text extractions of the originals (for grep / AI reading)
knowledge/                 → distilled, cross-referenced knowledge files (cite originals + pages)
  process_and_deadlines.md      timeline, CIS upload, Sperrvermerk, examiners, repeats, TF 6, team projects
  formal_requirements.md        length, layout, required parts & order, outline rules, style
  auftragsklaerung.md           the topic-proposal form, field by field, and how NAK judges it
  technical_focus_bwing24.md    the 4-of-6 technical-TF rule for WI ab Jg. 2024
  grading_rubric.md             FULL Bewertungsschema transcription (weights, K.O. criteria, all bands)
  reviewer_comments.md          real examiner comments by criterion + condensed red-flag list
  self_reflection.md            Selbstreflexion questions, rules, annotated example
  ai_usage.md                   KI policy, Eigenständigkeitserklärung, Prozessdokumentation + example
  internal_data_and_interviews.md  internal documents, confidentiality, expert-interview rules
  scientific_methods.md         research process, research questions, 17-method catalogue, selection aid
  example_good_tf_informatik.md NAK's "good TF" example dissected
  source_quality.md             source evaluation (Prexl figure, booklet, NAK FAQ rules)
  academic_writing_guide.md     ZBW booklet distilled (writing process, style, checklists)
  research_data.md              finding / citing / documenting data
  topic_examples.md             past TF titles by programme & module
  typst_template.md             the bundled Typst template + where it deviates from NAK formalia
  citation/                     APA, Harvard, IEEE, DIN ISO 690, MLA, internal sources + overview
checklists/
  auftragsklaerung_review.md    pre-upload review of the topic proposal
  tf_review.md                  rubric-mapped review procedure + output format
  pre_submission.md             NAK checklist + formal/upload checks
templates/                      auftragsklaerung · selbstreflexion · ki_prozessdokumentation · interview_protokoll · tf_outline
```

## The 10 things that matter most

1. **Process:** Auftragsklärung (signed by the Betreuer) → NAK decision within 1 week → **4 weeks** of writing → upload TF + Selbstreflexion + Eigenständigkeitserklärung (+ KI-Prozessdokumentation) → about 4 weeks of grading. **No changes after upload.** Not submitted means failed.
2. **Length:** **10 text pages ± 10 %** (~25,000 characters). Times New Roman 12 / Arial 11, 2 cm margins, 1,25 line spacing, justified with hyphenation. One PDF ≤ 10 MB.
3. **Grading:** Praxistransfer 45 % · Wissenschaftliches Arbeiten 35 % · Formalia 20 %. **K.O. criteria:** theory applied to practice; suitable literature.
4. **"Bericht statt Wissenschaft"** is the most common examiner complaint. You need an explicit research question or hypothesis, a justified method (ideally its own chapter), and an own analysis step.
5. **A pure literature review is capped** at "ausreichend" on rubric criterion II.7.
6. **Literature:** recent, peer-reviewed, every claim backed. No marketing pages, blogs, lexica, Medium or Wikipedia. Not only internet sources.
7. **Internal sources and interviews** must be verifiable via the appendix. Interview protocols need date, partner, function and topic, and must be signed.
8. **Double-blind:** no student name in the TF. Use the official Deckblatt. Set the Sperrvermerk via the CIS checkbox, not as a page in the document.
9. **AI is allowed only with full documentation.** Undocumented use counts as Täuschung and the TF fails.
10. **BWING24:** 4 of 6 TFs in technical modules, with a real technical focus. Business-only topics in a technical module can count as a Fehlversuch.

## Known discrepancies & caveats

| # | Issue | Details / recommendation |
|---|---|---|
| 1 | **Auftragsklärung length** | The form (2024) says **3000** characters; Formale Anforderungen 2026, Tipps 2022 and the FAQ say **2000**. Both are *Richtwert*. Aim for ~2000–2500. |
| 2 | **Mislabeled file** | `2022_07_Selbstreflexion_Transferleistungen.pdf` is byte-identical to the BWING24 Auftragsklärung. The blank Selbstreflexion form is `2022_07_Selbstreflexion_bsp_Transferleistungen.pdf`. |
| 3 | **KI-Prozessdokumentation placement** | FAQ: upload *in addition to* the TF and Selbstreflexion. Formale Anforderungen 2026: *"anfügen"*. The Typst template puts it in the appendix. Safest is to do both. |
| 4 | **Recency** | One examiner: everything older than 3 years is "veraltet". The rubric still accepts *"angemessene Grundlagenwerke"*. Prefer recent peer-reviewed work and use classics only for foundations. |
| 5 | **Internal documents** | FAQ: unpublished internal documents are in principle not citable, *except* in case studies or explorative work (the usual TF situation). Formale Anforderungen: internal documents belong in the appendix. In practice: cite them **and** attach them. |
| 6 | **Typst template** | It calls itself "officially approved", but NAK says it provides no templates. Its defaults (3 cm vertical margins, default font and line spacing, IEEE style) deviate from NAK formalia. See [typst_template.md](knowledge/typst_template.md). |
| 7 | **Rubric validity wording** | Page 1: *"ab Jahrgang 2021"*; page 2: *"ab 01.10.2021 gültig für alle Jahrgänge"*. It applies to BWING24 either way. |
| 8 | **Age / audience of method material** | The method slides are from 2021 and Informatik-oriented. The "good TF" example is from 2019 (older rules, no real company data). The ZBW booklet and research-data guide are generic, and the latter predates the GDPR. NAK's current documents win. |
| 9 | **Image-only pages** | The rubric (pp. 2–3), the example Selbstreflexion (pp. 2–3), several slides and the Prexl figure have no text layer. They are transcribed in the knowledge files, but the `originals_text/` versions are incomplete for them. |
| 10 | **Missing from the dump** | Leitfragen Technische TL (202510), the NAK KI-Richtlinie (22.10.2024), the list of technical modules, the Modulhandbuch, PVO 2024, the current Selbstreflexion form. See [sources/INDEX.md](sources/INDEX.md#referenced-by-nak-but-not-in-this-dump-worth-downloading-from-moodlecis). |

Further style-specific conflicts between the citation guides are in [knowledge/citation/README.md](knowledge/citation/README.md).

## Maintenance

- Add new source files to `originals/` unchanged.
- Generate a text extraction into `originals_text/` (e.g. with PyMuPDF: `page.get_text()` per page with `=== PAGE n ===` markers).
- Register the file in `sources/INDEX.md` and update the affected `knowledge/` file(s).
- Keep personal TF work (drafts, Matrikelnummer, company details) in a separate private repo. This one is public.
