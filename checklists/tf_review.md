# TF review procedure (for AI reviewers)

Use this when asked to review a TF draft (full or partial). It mirrors NAK's [grading rubric](../knowledge/grading_rubric.md) so the feedback maps onto how the examiner will grade.

## 0. Before reviewing, establish

- TF number (1–6). Examiners are more lenient on TF 1; from TF 2 on, concrete company value / Handlungsempfehlung is expected ([reviewer_comments.md](../knowledge/reviewer_comments.md) §5).
- Module, and whether it is a **technical** module (BWING24: 4 of 6) → [technical_focus_bwing24.md](../knowledge/technical_focus_bwing24.md).
- The **approved Auftragsklärung** text (Thema, Ziel, Vorgehen). The TF must deliver what it promised.
- The citation style chosen.
- Whether a draft Selbstreflexion exists.

## 1. Fast K.O. screen (report these first)

| Check | Fail signal |
|---|---|
| **Theory → practice transfer** (rubric I.3, K.O.) | Theory chapter and practice chapter run side by side without connection; no result applicable in practice; "Bericht" character |
| **Literature** (rubric II.8, K.O.) | Few sources; textbooks or web only; no peer-reviewed journals; no current research; key papers missing |
| **Technical focus** (if technical module) | Organisational or cost topic only structured with the Problemlösungszyklus; technical content only mentioned as context |
| **Research question / hypothesis** | Missing or implicit |
| **Formal hard limits** | Length outside 9–11 text pages; name visible; no Selbstreflexion planned |

## 2. Criterion-by-criterion review

For each criterion: give an **estimated band** (5,0 / 3,7–4,0 / 2,7–3,3 / 1,7–2,3 / 1,0–1,3) with a **justification quoting the rubric wording**, then **concrete fixes** pointing to the location (chapter/paragraph).

**I. Praxistransfer (45 %)**
1. Kernpunkte erfasst / inhaltliche Richtigkeit: does the Fazit answer the Zielsetzung? Is the topic clearly bounded? Are there factual errors?
2. Selbstreflexion: critical, names weaknesses + solutions, chapter references, Ich-Form (→ [self_reflection.md](../knowledge/self_reflection.md))
3. Theorie auf Praxis (K.O.): results usable in practice? Compared and checked against theory? Practice placed against research?
4. Lösungsansätze / Handlungsempfehlungen: own ideas, not only replication; recommendations derived from the analysis
5. Aufbau / Gliederung: roter Faden; no single sub-points; the introduction contains Hintergrund + Zielsetzung + Gang der Untersuchung; the method is announced early
6. Studienbezug / Fachsprache: terms defined with sources; link to module content

**II. Wissenschaftliches Arbeiten (35 %)**

7. Arbeitsformen: is there an **own** analysis step (data, interviews, model, calculation, evaluation)? A pure literature review is capped at 3,7–4,0 here.

8. Literatur (K.O.): source quality, recency, peer review, every claim backed, internal sources in the appendix (→ [source_quality.md](../knowledge/source_quality.md))

9. Methoden: is there a method chapter? Is the choice justified against alternatives? Are limitations named? Validity and reliability? (→ [scientific_methods.md](../knowledge/scientific_methods.md))

**III. Formalia (20 %)**

10. Language: spelling, no Ich/Wir, no colloquialisms, precise (no vague quantifiers, no weak passive conclusions); calculations correct
11. Layout: page count, Times New Roman 12 / Arial 11, 2 cm margins, line spacing 1,25, justified with hyphenation; lists present and correct; Roman/Arabic numbering; figures referenced in text; cross-references correct (→ [formal_requirements.md](../knowledge/formal_requirements.md))
12. Zitation: one consistent style; bibliography complete (publisher, year, pages, URL plus access date); only cited sources; no categorisation; interviews and internal docs listed (→ [citation/README.md](../knowledge/citation/README.md))

## 3. Cross-cutting red flags

Run the 12-point list at the end of [reviewer_comments.md](../knowledge/reviewer_comments.md). In particular:
- company description too long
- writing as an employee instead of an observer
- "Methodenwahl" that is really a table of contents
- unsupported claims
- conversations mentioned but not documented

## 4. Output format

```
## Gesamteindruck (2–4 Sätze) + Risiko: bestanden? (K.O.-Kriterien explizit)
## Bewertung je Kriterium (Tabelle: Kriterium | geschätzte Note | Begründung (Rubrik-Wortlaut) | Top-Fix)
## Priorisierte Maßnahmen (max. 10, nach Wirkung auf Note sortiert, mit Fundstelle)
## Formale Mängel (Liste)
## Offene Fragen an den/die Studierende(n)
```

Write the review in **German** if the TF is in German. Be specific: quote the problematic sentence and give a better formulation. Never invent sources. If suggesting literature, mark it "zu prüfen" unless it was verified (DOI/Crossref).

## 5. AI-usage reminder

If the student adopts AI-suggested text or structure from the review, it must be logged in the KI-Prozessdokumentation (→ [ai_usage.md](../knowledge/ai_usage.md)). End every review with a ready-to-paste log row:
`„<Prompt summary>" <Datum>; vgl. S. <x> | Feedback/Review des Entwurfs | <Bewertung> | <Tool + Version>`
