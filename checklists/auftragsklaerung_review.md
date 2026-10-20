# Auftragsklärung review checklist (for AI reviewers)

Basis: [knowledge/auftragsklaerung.md](../knowledge/auftragsklaerung.md) · acceptance criteria from the [FAQ](<../originals/converted_faq-2305.md>) · examiner patterns from [reviewer_comments.md](../knowledge/reviewer_comments.md).

## A. Acceptance criteria NAK applies (each must be a clear "yes")

- [ ] **Module fit:** does the topic clearly apply content from the chosen module? Is the module from the current or previous semester (otherwise a justification is needed)?
- [ ] **Problem clearly described:** concrete object, context, and consequence of leaving it unsolved (field 4)
- [ ] **Approach coherent and goal-oriented:** methods named, justified, and feasible in 4 weeks / ~10 pages
- [ ] **Technical focus** (technical module, BWING24): field 2 filled concretely; the topic is about the design, use or operation of technical systems or goods; not just the Problemlösungszyklus on an organisational task → [technical_focus_bwing24.md](../knowledge/technical_focus_bwing24.md)

## B. Quality checks (prevent problems later in grading)

- [ ] **Thema** is a research question or a precisely bounded problem, not "Darstellung / Überblick / Erstellung / Einführung von …"
- [ ] An explicit **Forschungsfrage** (and, where suitable, a hypothesis or Arbeitshypothesen) is derivable
- [ ] **Anlass** (field 3) says how the problem was noticed and what has already been tried
- [ ] **Ziel** (field 5) is concrete and checkable at the end (e.g. "Ableitung einer Handlungsempfehlung zu …", "Bewertung von … anhand von …"), and fits the Thema
- [ ] **Vorgehen** (field 6):
  - names concrete methods, e.g. Literaturanalyse + Experteninterviews + Nutzwertanalyse
  - says why they fit
  - includes an **own analysis step** beyond the literature review (rubric II.7 caps pure literature work at 3,7–4,0)
  - names the main verb: analysieren / vergleichen / prüfen / …
- [ ] **Scope:** one department, process or product; realistic for 150 h workload and a 4-week window; interviews feasible inside the window
- [ ] **Literature availability** checked (Tipps: *"Ist die Quellenlage ausreichend?"*); a quick Google Scholar or EBSCO probe returns relevant peer-reviewed work
- [ ] **Data access / confidentiality** clarified with the Betreuer; decision on the Sperrvermerk (checkbox at upload)
- [ ] **Length:** ≤ 3000 characters (form) and ideally ~2000–2500 (to also satisfy the 2000 guide value in other NAK docs); count **with** spaces unless stated otherwise
- [ ] **No Ich-Form**; impersonal and precise; company named with its legal form or an abbreviation introduced
- [ ] Betreuer **signature** and Matrikelnummer present
- [ ] For TF 6 as a BA Vorstudie: mentioned under "Wie lautet Ihr Thema"

## C. Output format

```
## Ampel: Annahme wahrscheinlich? (grün/gelb/rot) + Hauptgrund
## Feld-für-Feld-Feedback (Feld | Problem | Verbesserter Formulierungsvorschlag)
## Zeichenzählung (mit/ohne Leerzeichen) je Feld + gesamt
## Risiken für die spätere Bewertung (Rubrik-Kriterien)
```

Count characters with a script, not by estimate, e.g. `python3 -c "import sys;t=open(sys.argv[1]).read();print(len(t),len(t.replace(' ','')))" file.txt`.
