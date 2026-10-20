# Source index — every original file, what it is, where it is used

All originals are stored **unchanged** (sole exception: the printing user's name/IP redacted on p. 1 of `Beispielhafte Komentare.pdf`) in [`originals/`](../originals/). This is the dump of the NAK Moodle course "Transferleistungen" (Moodle export, 20.10.2026), including the two user-provided Markdown conversions (`converted_*.md`). Plain-text extractions for AI grep/reading are in [`originals_text/`](../originals_text/) (same base name, `.txt`, with `=== PAGE n ===` markers; generated with PyMuPDF / openpyxl / python-docx). **Image-only pages are missing from the txt files.** Where they matter, they were transcribed by viewing renders, as noted below.

Legend: ⭐ = core/binding NAK document · 📘 = generic guide · 🧪 = example · ⚠ = caveat

## NAK process & requirements

| File | What it is | Date | Pages | Used in | Notes |
|---|---|---|---|---|---|
| ⭐ [2026_Formale Anforderungen.pdf](<../originals/2026_Formale Anforderungen.pdf>) | One-slide summary of formal requirements (lengths, 4/6 technical, upload rules) | 2026 | 1 | [formal_requirements](../knowledge/formal_requirements.md), [process](../knowledge/process_and_deadlines.md) | Newest doc; says Auftragsklärung 2000 chars ⚠ |
| ⭐ [Auftragsklärung_Transferleistung ab 2024.pdf](<../originals/Auftragsklärung_Transferleistung ab 2024.pdf>) | Official Auftragsklärung form (current) | 2024 | 3 (p. 3 blank) | [auftragsklaerung](../knowledge/auftragsklaerung.md), [template](../templates/auftragsklaerung.md) | Says 3000 chars ⚠ |
| ⭐ [2024_08 BWING24__Auftragsklärung_Transferleistung.pdf](<../originals/2024_08 BWING24__Auftragsklärung_Transferleistung.pdf>) | Same form, BWING24 layout | 08.2024 | 3 | as above | Wording identical to "ab 2024" |
| ⚠ [2022_07_Selbstreflexion_Transferleistungen.pdf](<../originals/2022_07_Selbstreflexion_Transferleistungen.pdf>) | **Mislabeled:** byte-identical (MD5 `68537084…`) to the BWING24 Auftragsklärung | — | 3 | — | Not a Selbstreflexion. Probably a wrong download; re-download the real Selbstreflexion form from Moodle if needed |
| ⭐ [2022_07_Selbstreflexion_bsp_Transferleistungen.pdf](<../originals/2022_07_Selbstreflexion_bsp_Transferleistungen.pdf>) | The **blank** Selbstreflexion form (7 questions), despite the "bsp" | 07.2022 | 3 | [self_reflection](../knowledge/self_reflection.md), [template](../templates/selbstreflexion.md) | |
| 🧪 [Beispiel Selbstreflexion.pdf](<../originals/Beispiel Selbstreflexion.pdf>) | Filled example (Airbus A350 / Porter 5 Forces) | — | 3 | [self_reflection](../knowledge/self_reflection.md) | pp. 2–3 image-only → transcribed in self_reflection.md |
| ⭐ [2022_07_Dokument_Transferleistung_Deckblatt.pdf](<../originals/2022_07_Dokument_Transferleistung_Deckblatt.pdf>) | Official cover sheet (Nr., Matrikelnummer, Thema, Studiengang/Zenturie) | 07.2022 | 1 | [formal_requirements](../knowledge/formal_requirements.md) | Must be used; no name |
| ⭐ [Bewertungsschema Transferleistungen.pdf](<../originals/Bewertungsschema Transferleistungen.pdf>) | **Grading rubric** (weights, K.O. criteria, full Erwartungshorizont) | 2021 (valid from 01.10.2021) | 3 | [grading_rubric](../knowledge/grading_rubric.md), [tf_review](../checklists/tf_review.md) | pp. 2–3 image-only → fully transcribed |
| ⭐ [Beispielhafte Komentare.pdf](<../originals/Beispielhafte Komentare.pdf>) | Moodle book of real examiner comments by criterion | printed 20.10.2026 | 9 | [reviewer_comments](../knowledge/reviewer_comments.md) | Moodle print; the printing user's name and IP were redacted on p. 1 (only change made to any original) |
| ⭐ [Transferleistung_Tipps zur Anfertigung.pdf](<../originals/Transferleistung_Tipps zur Anfertigung.pdf>) | NAK guide: goals, Auftragsklärung prep, structure, formalia, citing, checklist | 06.2022 | 5 | [formal_requirements](../knowledge/formal_requirements.md), [auftragsklaerung](../knowledge/auftragsklaerung.md), [pre_submission](../checklists/pre_submission.md) | |
| ⭐ [faq-2305.h5p](<../originals/faq-2305.h5p>) | Moodle FAQ (H5P accordion package) | 2023 base, updated (mentions PVO 2024, 202510 Leitfragen) | — | via conversion | Raw H5P; read the .md |
| ⭐ [converted_faq-2305.md](<../originals/converted_faq-2305.md>) | **User-provided conversion** of the FAQ H5P | — | — | [process](../knowledge/process_and_deadlines.md), [formal](../knowledge/formal_requirements.md), [internal data](../knowledge/internal_data_and_interviews.md), [ai_usage](../knowledge/ai_usage.md), [technical](../knowledge/technical_focus_bwing24.md), [source_quality](../knowledge/source_quality.md) | Verified complete: all 87 titled H5P entries are present. The 2 images in the H5P (CIS upload screenshots) are only referenced, not shown |
| ⭐ [2024_10Eigenständigkeitserklärung KI.pdf](<../originals/2024_10Eigenständigkeitserklärung KI.pdf>) | Declaration of independent work incl. AI clause | 10.2024 | 1 | [ai_usage](../knowledge/ai_usage.md) | Separate upload, contains name |
| ⭐ [NAK_Prozessdokumentation_KI_final.docx](<../originals/NAK_Prozessdokumentation_KI_final.docx>) | Blank KI-Prozessdokumentation form | 2025 | 1 | [ai_usage](../knowledge/ai_usage.md), [template](../templates/ki_prozessdokumentation.md) | |
| 🧪 [NAK_Prozessdokumentation_KI_final_20250219.pdf](<../originals/NAK_Prozessdokumentation_KI_final_20250219.pdf>) | Filled example of the KI log | 19.02.2025 | 2 | [ai_usage](../knowledge/ai_usage.md) | |
| [Themen Transferleistungen.xlsx](<../originals/Themen Transferleistungen.xlsx>) | List of past TF topics by programme + module | — | 1 sheet | [topic_examples](../knowledge/topic_examples.md) | |

## Methods & examples

| File | What it is | Date | Pages | Used in | Notes |
|---|---|---|---|---|---|
| [2021_03_16_Transferleistungen_Erstesemester_Methoden INF.pdf](<../originals/2021_03_16_Transferleistungen_Erstesemester_Methoden INF.pdf>) | NAK slides "TF Theorie/Praxis – Methoden Informatik" (1st semester) | 16.03.2021 | 27 | [scientific_methods](../knowledge/scientific_methods.md) | Informatik-oriented, but the most TF-specific method source |
| [2022_08_Wissenschaftliche Methoden.pdf](<../originals/2022_08_Wissenschaftliche Methoden.pdf>) | NAK library slides: finding method handbooks | 09.08.2022 | 6 | [scientific_methods](../knowledge/scientific_methods.md) | A reading list, not method content |
| 📘 [00 research methodologySchneider.ppt](<../originals/00 research methodologySchneider.ppt>) | Lecture "Scientific Methodology in Business and Economics" (EN) | — | 44 slides | [scientific_methods](../knowledge/scientific_methods.md) | Legacy .ppt |
| 📘 [converted_00_research_methodologySchneider.md](<../originals/converted_00_research_methodologySchneider.md>) | **User-provided conversion** of the ppt | — | — | [scientific_methods](../knowledge/scientific_methods.md) | ⚠ image-only slides are missing; they were extracted from the .ppt and are marked [ppt image] in scientific_methods.md |
| 🧪 [Gute TL Informatik.pdf](<../originals/Gute TL Informatik.pdf>) | Example of a good TF: "Untersuchung von Schema Evolution verschiedener Datenbanktypen für BPMS" (4th TF, 2019, experiment, IEEE) | 2019 | 20 | [example_good_tf_informatik](../knowledge/example_good_tf_informatik.md) | Older rules; no real company data |

## Writing, sources, data

| File | What it is | Date | Pages | Used in | Notes |
|---|---|---|---|---|---|
| 📘 [schreibe_deine_beste_hausarbeit_booklet.pdf](<../originals/schreibe_deine_beste_hausarbeit_booklet.pdf>) | ZBW/EconBiz booklet on writing an economics paper (incl. AI) | 3rd ed. 09.2025 | 40 | [academic_writing_guide](../knowledge/academic_writing_guide.md), [source_quality](../knowledge/source_quality.md) | Generic; NAK rules take precedence |
| 📘 [Die Wissenschaftlichkeit von Quellen bewerten Abb. 3 Prexl.jpg](<../originals/Die Wissenschaftlichkeit von Quellen bewerten Abb. 3 Prexl.jpg>) | Figure: relevant / zitierfähig / zitierwürdig | — | image | [source_quality](../knowledge/source_quality.md) | Transcribed; author's full name is unverified |
| 📘 [Forschungsdaten_DINA4_ONLINE_VER_02_06.pdf](<../originals/Forschungsdaten_DINA4_ONLINE_VER_02_06.pdf>) | ZBW/GESIS/RatSWD guide: finding, citing, documenting research data | 2015 (2nd ed.) | 28 | [research_data](../knowledge/research_data.md) | Pre-GDPR; quantitative data only |

## Citation guides

| File | What it is | Pages | Used in |
|---|---|---|---|
| [APA Zitierrichtlinien.pdf](<../originals/APA Zitierrichtlinien.pdf>) | APA style guide | 9 | [citation/apa](../knowledge/citation/apa.md) |
| [Harvard-Zitierweise.pdf](<../originals/Harvard-Zitierweise.pdf>) | Harvard style guide | 40 | [citation/harvard](../knowledge/citation/harvard.md) |
| [IEEE.pdf](<../originals/IEEE.pdf>) | IEEE style guide | 4 | [citation/ieee](../knowledge/citation/ieee.md) |
| [Zitieren_nach_DIN_ISO_690.pdf](<../originals/Zitieren_nach_DIN_ISO_690.pdf>) | DIN ISO 690 guide | 9 | [citation/din_iso_690](../knowledge/citation/din_iso_690.md) |
| [Zitierrichtlinien-MLA.pdf](<../originals/Zitierrichtlinien-MLA.pdf>) | MLA style guide | 10 | [citation/mla](../knowledge/citation/mla.md) |
| ⭐ [Zitieren interner Quellen.pdf](<../originals/Zitieren interner Quellen.pdf>) | Citing company-internal sources | 35 | [citation/internal_sources](../knowledge/citation/internal_sources.md), [internal_data_and_interviews](../knowledge/internal_data_and_interviews.md) |

## Tools

| File | What it is | Used in |
|---|---|---|
| [nak-typst-template-main/](<../originals/nak-typst-template-main/>) | Student-made Typst template for TFs (MIT, Leon Heuer, 2025), incl. a KI documentation table | [typst_template](../knowledge/typst_template.md) — ⚠ defaults deviate from NAK formalia |

## Referenced by NAK but NOT in this dump (worth downloading from Moodle/CIS)

- **Leitfragen Technische Transferleistungen im Studium Wirtschaftsingenieurwesen (202510)**: important for the 4 technical TFs.
- **Richtlinie zum Einsatz generativer KI bei Prüfungsleistungen, Studienleistungen und Abschlussarbeiten (22.10.2024)**.
- The real **Selbstreflexion form (2024+)**, since the `2022_07_Selbstreflexion_Transferleistungen.pdf` slot holds the wrong file.
- List of **technical modules** for BWING24 (NAK presentation).
- **Modulhandbuch Wirtschaftsingenieurwesen**: the "Verflechtung mit betrieblicher Praxis" sections are the official topic source.
- **PVO 2024** (Prüfungsverfahrensordnung).
- English versions of the forms ("Materials in englisch" in Moodle).
