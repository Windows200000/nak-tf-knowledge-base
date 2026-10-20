# Instructions for AI assistants using this repository

This repo is a knowledge base for **creating and reviewing NORDAKADEMIE Transferleistungen (TF/TL)**, the six theory-practice transfer papers of the dual study programme. It is tailored to **Wirtschaftsingenieurwesen ab Jahrgang 2024 (BWING24)** but most of it applies to all NAK programmes.

## How to navigate

1. Start with [README.md](README.md) (map of the repo) and [sources/INDEX.md](sources/INDEX.md) (what every original file is).
2. Read the relevant `knowledge/*.md` file(s) for the task. They are distilled, cross-referenced and cite the originals with page numbers.
3. For exact wording, open the original in `originals/` or its text extraction in `originals_text/`. Image-only pages are missing from the txt files; the knowledge files say where something was transcribed from an image.

## Task → files

| Task | Read first |
|---|---|
| Find or sharpen a topic, draft the **Auftragsklärung** | [knowledge/auftragsklaerung.md](knowledge/auftragsklaerung.md), [knowledge/technical_focus_bwing24.md](knowledge/technical_focus_bwing24.md), [knowledge/topic_examples.md](knowledge/topic_examples.md), [templates/auftragsklaerung.md](templates/auftragsklaerung.md), [checklists/auftragsklaerung_review.md](checklists/auftragsklaerung_review.md) |
| Plan method / research design | [knowledge/scientific_methods.md](knowledge/scientific_methods.md), [knowledge/grading_rubric.md](knowledge/grading_rubric.md) (criteria II.7, II.9) |
| Outline & write | [templates/tf_outline.md](templates/tf_outline.md), [knowledge/formal_requirements.md](knowledge/formal_requirements.md), [knowledge/academic_writing_guide.md](knowledge/academic_writing_guide.md), [knowledge/example_good_tf_informatik.md](knowledge/example_good_tf_informatik.md) |
| Literature & sources | [knowledge/source_quality.md](knowledge/source_quality.md), [knowledge/citation/README.md](knowledge/citation/README.md) |
| Company data, interviews, confidentiality | [knowledge/internal_data_and_interviews.md](knowledge/internal_data_and_interviews.md), [knowledge/citation/internal_sources.md](knowledge/citation/internal_sources.md), [knowledge/research_data.md](knowledge/research_data.md), [templates/interview_protokoll.md](templates/interview_protokoll.md) |
| **Review a draft** | [checklists/tf_review.md](checklists/tf_review.md), [knowledge/grading_rubric.md](knowledge/grading_rubric.md), [knowledge/reviewer_comments.md](knowledge/reviewer_comments.md) |
| Selbstreflexion | [knowledge/self_reflection.md](knowledge/self_reflection.md), [templates/selbstreflexion.md](templates/selbstreflexion.md) |
| AI use / declarations | [knowledge/ai_usage.md](knowledge/ai_usage.md), [templates/ki_prozessdokumentation.md](templates/ki_prozessdokumentation.md) |
| Submission | [checklists/pre_submission.md](checklists/pre_submission.md), [knowledge/process_and_deadlines.md](knowledge/process_and_deadlines.md) |
| Typst typesetting | [knowledge/typst_template.md](knowledge/typst_template.md) |

## Rules

1. **Precedence of sources:** NAK's own binding documents come first: the forms, Formale Anforderungen 2026, the Bewertungsschema, the FAQ, and the Tipps. Then NAK teaching material (method slides, examiner comments). Generic guides come last (ZBW booklet, research-data guide, citation guides, Schneider slides). Newer NAK documents beat older ones. Where sources conflict, **say so** and do not silently pick one. Known conflicts are listed in [README.md](README.md#known-discrepancies--caveats).
2. **Cite this repo.** When stating a NAK rule, name the file (and page) it comes from so the student can verify it. Do not present general knowledge as a NAK rule.
3. **Never fabricate literature.** Only suggest references you can verify (DOI/Crossref, publisher page). Otherwise mark them "zu prüfen". Hallucinated sources in a TF are falsification and fail the K.O. literature criterion.
4. **Language:** TF text, Auftragsklärung and Selbstreflexion are usually **German**. No Ich/Wir form in the TF or Auftragsklärung; **Ich-Form in the Selbstreflexion**. Talk to the student in whatever language they use.
5. **AI-use logging is mandatory for the student.** Every AI contribution that shapes the TF (ideas, outline, wording, review, code, calculations) must appear in the KI-Prozessdokumentation. When you produce something the student may adopt, end with a ready-to-paste log row: `„<prompt summary>" TT.MM.JJJJ; vgl. S. x | <Grund> | <Bewertung> | <Tool + Version>`. Undocumented AI use counts as Täuschung, and the TF is then failed.
6. **Push for science, not reports.** The #1 examiner complaint is "Bericht statt wissenschaftliche Arbeit". Always steer towards:
   - an explicit research question or hypothesis
   - a justified method chapter
   - an own analysis step (a pure literature review caps rubric criterion II.7 at "ausreichend")
   - recent peer-reviewed literature
   - a real theory→practice transfer with a Handlungsempfehlung
7. **Respect constraints:** about 10 text pages, 4 weeks, 150 h workload, double-blind (no student name in the TF), company confidentiality (Sperrvermerk, appendix rules). For technical modules (4 of 6 for BWING24), a real technical focus is required.
8. **Count, don't estimate.** Character limits (Auftragsklärung, Selbstreflexion) and page counts must be measured with a script or tool.
9. **Do not modify `originals/` or `originals_text/`.** They are the verbatim source record. Add new source files to `originals/`, regenerate their txt, and register them in `sources/INDEX.md`.
10. **Keep personal data out of this repo.** It is public. Matrikelnummer, employer specifics, drafts and per-TF notes belong in the student's own private repo.
