# Example of a Good Transferleistung (Informatik)
**Sources:** [Gute TL Informatik.pdf](<../originals/Gute TL Informatik.pdf>) · full text: [txt](<../originals_text/Gute TL Informatik.txt>) · related NAK slide: [2021_03_16_Transferleistungen_Erstesemester_Methoden INF.pdf](<../originals/2021_03_16_Transferleistungen_Erstesemester_Methoden INF.pdf>) (S. 21)

Page references below use **PDF page numbers** ("PDF p. n") plus the printed page number where useful ("printed S. n"). PDF p. 1 (cover) and PDF p. 18–20 (appendix code listings) have no extractable text and were rendered and read as images.

---

## 1. Identification

| Item | Value |
|---|---|
| Title / "Freigegebenes Thema" | **„Untersuchung von Schema Evolution verschiedener Datenbanktypen für Business Process Management Systeme"** (cover, PDF p. 1) |
| Document type | NAK cover sheet "Transferleistung Theorie/Praxis* **4**" – i.e. the 4th Transferleistung (PDF p. 1) |
| Student | Studiengang/Zenturie **A16a** (presumably an Informatik Zenturie of the 2016 cohort; the file name says Informatik) (PDF p. 1) |
| Date | PDF created 11.10.2019 (metadata); sources accessed Sep 2019 |
| Tool | LaTeX (pdfTeX, hyperref), Latin Modern 12 pt body, A4 (PDF metadata/fonts) |
| Why it is "good" | The file name ("Gute TL") is the only explicit verdict; no grade or examiner comment is included. The evaluation below is inferred. |
| Link to NAK teaching | This exact topic is the **worked example** in the NAK method slides: „Untersuchung von Schema Evolution verschiedener Datenbanktypen für Business Process Management Systeme **am Beispiel vom Unternehmen X**", Methode: Experiment, with an outline matching this paper (Methoden INF, S. 21). NAK itself uses it as the model of an experiment-based TF. |

Caveat: this is a 2019 TF under older rules (cover sheet with footnote on PVO 03.02.2015). It contains no KI-Prozessdokumentation, no Eigenständigkeitserklärung and no Selbstreflexion in this PDF. Check current formal requirements separately.

---

## 2. Research question and goal

Stated at the end of the problem paragraph in the introduction (PDF p. 6, printed S. 1):

> „Insofern stellt sich folgende Frage: **Welcher Datenbanktyp eignet sich am besten für Business Process Management System (BPMS) angesichts der Unterstützung für Schema Evolution?**"

Goal sentence immediately after:

> „Die Unterstützung verschiedener Datenbanktypen für Schema Evolution zu untersuchen ist Ziel dieser Arbeit."

Restated in the method chapter (PDF p. 10):

> „Um die Frage zu beantworten, welcher der beiden vorgestellten Datenbanktypen sich hinsichtlich Schema Evolution von BPMS besser eignet, wird ein Fallbeispiel bearbeitet."

RQ type in NAK terms: *"Vergleiche von Datenbanken, Software, etc."* + *"Evaluation"* (Methoden INF S. 12); design type: **comparison by criteria, operationalised as an experiment** (Schneider Folie 24; Methoden INF S. 19–21). No explicit hypothesis is formulated.

---

## 3. Full outline with page share

Front matter (Roman numerals): cover · Inhaltsverzeichnis (i) · Tabellenverzeichnis (ii) · Abbildungsverzeichnis (iii) · Abkürzungsverzeichnis (iv, 11 entries). Body: printed S. 1–10 (PDF p. 6–15). Back matter: Quellenverzeichnis (printed iv–v, PDF p. 16–17) · Anhang (printed vi–viii, PDF p. 18–20; code only, no heading page).

| Chapter (verbatim) | Printed pages | ≈ Pages | ≈ Share of body | Content |
|---|---|---|---|---|
| 1 Einleitung | 1 | 1.0 | 10 % | Context → problem → RQ → goal → roadmap |
| 2 Grundlagen | 2–4 (+ ¼ of 5) | 3.3 | 34 % | 2.1 Schema Evolution · 2.2 Workflow Engines (Camunda) · 2.3 Relationale Datenbanken · 2.4 Graph Datenbanken (Neo4j, Fig. 1) |
| 3 Vergleichbare Arbeiten | 5 | 0.4 | 4 % | Related work [17]–[19]: speed, scaling, size, maturity |
| 4 Analyse | 5–9 | 4.2 | 43 % | 4.1 Methodik (~0.6) · 4.2 Fallbeispiel (~1.2, Fig. 2, 4 scenarios) · 4.3 Objektive Messungen (~1.4, Tables 1–4) · 4.4 Subjektive Messungen (~0.6) · 4.5 Diskussion (~0.6) |
| 5 Fazit | 9–10 | 0.8 | 9 % | Summary, results vs. literature, recommendation |
| **Total body** | | **≈ 9.7** | | ≈ 3,200 words incl. tables (word count of extracted text, PDF p. 6–15) |

Proportions to note: theory (Grundlagen + related work) ≈ 38 %, own analysis ≈ 43 %, intro + conclusion ≈ 19 % – matching Schneider's rule "Introduction and conclusion are never more than 20% of the paper" (Schneider, Folie 36). Heading depth is max. 2 levels. Length fits "10 Seiten (+/- 10%)" (Methoden INF S. 8).

---

## 4. How the introduction is built (PDF p. 6)

Funnel structure in one page, four moves:

1. **Broad relevance (BPM in companies), with sources:**
   > „Moderne Business Process Management (BPM) Systeme sind zur Erstellung und Verbesserung von Workflows unerlässlich in Großunternehmen geworden. Sie ermöglichen die Identifikation von optimierbaren Prozessen, die durch Methoden wie Automatisierung erfolgreicher und schneller bearbeitet werden können.[1]"
2. **Narrowing to the technical problem** (workflow engines log every step → database persistence → changing processes):
   > „Jederzeit können Prozesse verändert, gelöscht oder hinzugefügt werden. Aus diesem Grund muss die verwendete Datenbank Schema Evolution unterstützen.[6]"
   Key term defined in a footnote: „Schema Evolution ist die Möglichkeit, Daten und Schema trotz Veränderungen des Schemas konsistent zu halten.[5]"
3. **RQ + goal** (see §2) – introduced with „Insofern stellt sich folgende Frage:".
4. **Roadmap of the paper (Gang der Untersuchung)**, naming the method and the expected output:
   > „Zunächst werden dafür die Grundlagen erläutert. […] Anschließend werden ähnliche wissenschaftliche Arbeiten zu diesem Thema betrachtet. Um daraufhin die verschiedenen Datenbanktypen bewerten zu können, wird ein Fallbeispiel entwickelt, welches verschiedene Aspekte der Schema Evolution abdeckt. Anschließend wird dieses mit je einem Vertreter eines Datenbanktyps durchgeführt, protokolliert und ausgewertet. Zuletzt wird auf Basis dieser Ergebnisse ein Fazit erstellt, womit eine Empfehlung für den zu verwendenden Datenbanktypen in einem BPMS abgegeben wird."

No separate "Problemstellung"/"Zielsetzung" subheadings – problem, goal and procedure are integrated into a single Einleitung of one page. Every factual claim in the intro carries a source ([1]–[6]).

---

## 5. Grundlagen – scoped to the RQ

Pattern: each basics section ends by stating what is (ir)relevant for the RQ, which keeps the theory part lean:
- „Im Zuge der Schema Evolution sind allerdings ausschließlich Strukturen relevant, die sich durch Anpassungen im Workflow verändern. Daher werden nur diese bei der späteren Analyse in Betracht gezogen." (2.2, PDF p. 7)
- „Moderne relationale Datenbanken bieten viele weitere Operationen und Funktionalitäten an, welche allerdings zur Beantwortung der Forschungsfrage zu vernachlässigen sind." (2.3, PDF p. 8)
- „Im Hinblick auf die Schema Evolution ist der Aspekt der Schemaanpassung von besonderer Bedeutung." (2.3, PDF p. 8)
- Neo4j's constraint mechanism is explained precisely because it matters for schema evolution: „Dieser Punkt unterscheidet Neo4j von anderen Graph Datenbanken hinsichtlich der Schema Evolution …" (2.4, PDF p. 10)

Concrete abstractions (Camunda chosen "exemplarisch" for workflow engines, Neo4j for graph DBs) are made explicit and justified (Neo4j: "seit mehreren Jahren bereits (Stand 09.2019) die relevanteste Graph Datenbank" citing DB-Engines ranking [15], PDF p. 9). A literature-based problem example is quantified: MediaWiki – „pro Schemaänderung bis zu 70% der DCL-Skripte angepasst werden.[13]" (PDF p. 8).

## 6. Vergleichbare Arbeiten – related work as bridge to the method (PDF p. 10)

Short (≈ 0.4 pages) but functional: it extracts from prior studies **which metrics are used** (query speed, scaling, physical DB size, non-measurable factors such as maturity) and these become the metrics of the own analysis. Example formulations:
> „Es gibt viele Vergleiche von relationalen Datenbanken zu Graph Datenbanken. Insbesondere die Abfragegeschwindigkeit in verschiedenen Szenarien wird in Arbeiten wie [17] oder [18] ausgiebig untersucht."
> „Ebenso werden nicht messbare Faktoren in den Vergleich der Datenbanktypen miteinbezogen. In [17] und [19] wird die fehlende Einheitlichkeit sowie der unzureichende Reifegrad der Software kritisiert."

The gap is implicit (comparisons exist, but not specifically for schema evolution in BPMS) – not stated in one explicit sentence.

---

## 7. Method and its justification (4.1 Methodik, PDF p. 10–11)

**Method:** experiment/benchmark on a constructed case example ("Fallbeispiel") – both databases execute the same schema-evolution scenarios via scripts; measured with objective and subjective metrics.

Justification moves (each a sentence that can be imitated):
- **Choice of representatives, with source:** „Als relationale Datenbank wird SQLite gewählt, da es kein komplexes Datenbankmanagementsystem benötigt und alle notwendigen SQL Statements für Schema Evolution implementiert [20]. Das zuvor vorgestellte Neo4j (Version 3.5.9) wird für diesen Zweck als Graph Datenbank verwendet."
- **Reproducibility:** „Alle Schritte der Schema Evolution werden in SQL bzw. Cypher in Textform (Skript) festgehalten. (siehe Anhang S. vi - vii)" – full scripts in the appendix; exact software version given.
- **Objective metrics, with rationale and repetition:** „Darunter fallen alle Messungen, die während der Laufzeit der Skripte erfasst werden können. Das beinhaltet Laufzeit (Performance), Arbeitsspeicherverbrauch, sowie Festplattenspeicherverbrauch. Um eine höhere Genauigkeit bei der Ausführung des Beispiels zu erreichen, wird es mehrmals durchgeführt, wobei das Ergebnis als Tupel von arithmetischen Mittel der Messungen sowie der Standardabweichung angegeben wird."
- **Script metrics justified by literature:** LOC and number of statements – „Auch wenn diese beiden Metriken sich nicht explizit auf die Leistung der Datenbank auswirken, so sind sie dennoch relevant für die Benutzbarkeit der Datenbank.[17]"
- **Subjective metrics openly labelled as such, with an explicit evaluation rule:** „Diese Aspekte der Datenbank sind nicht quantifizierbar, sind jedoch essentiell zur Beantwortung der Frage, wie leicht eine Schema Evolution auf einer Datenbank durchzuführen ist. […] Dabei gilt, umso einfacher die Statements zu verfassen sind, desto besser ist die Sprache für eine Schema Evolution geeignet.[17]"

**Case design (4.2, PDF p. 11–12):** a simple warehouse workflow Annahme → Lagerung → Sendung (Fig. 2), 1,000,000 randomised records per database, and four scenarios that each represent a type of schema change: (1) delete all data and schemas; (2) remove a workflow step (Lagerung) and bridge it; (3) insert a new step (Begutachtung) with default value for historic data; (4) add an attribute (Stockwerk) with default. Success condition stated: „Dabei gilt im Allgemeinen, dass alle Szenarien fehlerlos von den Systemen bewältigt werden müssen." Scope limitation stated up front: „Erweiterte Möglichkeiten eines BPM wie beispielsweise Entscheidungen werden nicht betrachtet."

What is *not* there: no discussion of alternative methods (e.g. why not interviews or a literature-only comparison), which NAK's later guidance demands ("wodurch grenzt sich diese von anderen Methoden ab", Methoden INF S. 18).

---

## 8. Results, discussion and conclusion

### 8.1 Results (4.3 / 4.4, PDF p. 12–14)
- Four result tables with captions **above** the table, units in the caption, e.g. „Tabelle 1: Ausführungsdauer in Millisekunden (Dauer; Standardabweichung)"; Tables 2–3 memory/disk in KB; Table 4 LOC and statements.
- Text after the tables interprets, quantifies and explains anomalies:
  > „Wie in Tabelle 1 abzulesen ist, gibt es keine signifikanten Unterschiede in der Laufzeit der Szenarien, abgesehen von Szenario 4. Dennoch konnte Neo4j in Szenario 2 und 3 eine im Durchschnitt 2,3-fach kürzere Zeit aufweisen als SQLite. Lediglich in Szenario 4 war Neo4j um mehrere Größenordnungen langsamer. Das hängt mit der Natur des ausgeführten Skripts zusammen."
- Results are **tied back to literature**: „Die deutlich höhere physikalische Größe von Neo4j deckt sich mit anderen Arbeiten wie [17]."
- Fairness caveats placed directly at the result: „Dabei ist notwendig zu erwähnen, dass Neo4j einen Datenbankserver erstellt, welcher dauerhaft läuft, während SQLite lediglich während einer Transaktion aktiv ist."
- Subjective findings (4.4) are reported as experience from writing the scripts („Bei der Erstellung der Skripte ist schnell aufgefallen, dass …"), still in impersonal style.

### 8.2 Discussion (4.5, PDF p. 14) – self-critical validity check
Opening: „Im Folgenden wird die Aussagekräftigkeit der Daten behandelt. Dabei wird sich auf das Fallbeispiel und Auffälligkeiten der Messungen bezogen."
- Limited realism of the case, and why it was still chosen: „Zunächst stellt das Fallbeispiel nur einen bedingt realistischen Fall dar. Workflows enthalten häufig Entscheidungsmöglichkeiten, durch die das Datenmodell komplexer wird. […] Das einfache Fallbeispiel wurde gewählt, um sicherzustellen, dass beide Datenbanken ohne Probleme mit dem Datenmodell zurechtkommen."
- Own design flaw admitted: „In Bezug auf die Metriken wäre die Nutzung eines Databanken Management Systems von Vorteil gewesen, um einen besseren Vergleich mit Neo4j zu garantieren. Durch die Verwendung von SQLite ist der Vergleich der Arbeitsspeichernutzung sowie der LOC irreführend."
- Tool-specific artefact explained (SQLite cannot add foreign keys afterwards → extra statements/LOC).

### 8.3 Fazit (5, PDF p. 14–15)
Three moves:
1. **Recap of the procedure** in past tense: „In dieser Arbeit wurden zunächst relationale sowie Graph Datenbanken vorgestellt und ihre Besonderheiten hinsichtlich der Schema Evolution herausgestellt. […] Nach Durchführung der der Tests und Bewertung der Messdaten wurde über die Validität der Analyse diskutiert."
2. **Results relative to literature:** „Die Testergebnisse zeigen Ähnlichkeiten zu den vorgestellten Arbeiten auf. […] Allerdings zeigt sich auch, dass die Graph-Datenbank ein einen höheren Speicherverbrauch […] besitzt".
3. **Answer + recommendation (Handlungsempfehlung):**
   > „Insgesamt hat sich gezeigt, dass die genutzte Graph Datenbank Neo4j nur wenige konkrete objektive Vorteile gegenüber der eingesetzten relationalen Datenbank SQLite besitzt in Bezug auf die Schema Evolution des dargestellten Beispielworkflows."
   > „Damit spricht wenig für einen Wechsel der Datenbank in BPMS. Insbesondere ein Wechsel von einer bestehenden relationalen Datenbank wäre aufgrund zusätzlicher Arbeit und eines wahrscheinlich auftretenden Umgewöhnungsfaktors unwirtschaftlich."

The answer is appropriately hedged to the tested setting ("der genutzten", "des dargestellten Beispielworkflows"). No new sources in the Fazit (consistent with Schneider, Folie 34). Missing compared to Schneider's findings checklist: explicit "areas for further study" (e.g. complex workflows with decisions are only mentioned in 4.5).

---

## 9. Citation style

- **IEEE-style numeric citations** in square brackets, numbered in order of first appearance, [1]–[20]. In-text placement mostly directly after the sentence period without space („…bearbeitet werden können.[1]"), sometimes before the period („…implementiert [20]."), occasionally doubled („[10][11]"). No page numbers in in-text citations. Figure taken from a source is cited in the caption: „Abbildung 1: Beispielhafte Darstellung eines Graphen von Personen [14]".
- **Quellenverzeichnis** (PDF p. 16–17): IEEE format with German labels – „Hrsg.", „Bd.", „Nr.", „S.", online sources with „[Online]. Verfügbar unter: … [Zugegriffen: 25. Sep 2019]." Example: „[17] C. Vicknair, M. Macias, Z. Zhao, X. Nan, Y. Chen, und D. Wilkins, A comparison of a graph database and a relational database, in Proceedings of the 48th Annual Southeast Regional Conference, 2010, S. 1."
- **Source mix (20):** 8 books (incl. MIT Press, CRC Press, O'Reilly, a published dissertation), 4 conference/workshop proceedings (IEEE ICDE, ICEIS, ACM Southeast, FoMLaDO), 2 journal articles, 1 encyclopedia, 5 web/vendor sources (OMG BPMN spec, Camunda docs ×2, DB-Engines ranking, Neo4j manual). Vendor docs are used only for product facts; claims about comparisons rest on scientific papers.
- Footnotes are used only for term definitions (Schema Evolution, MediaWiki), not for citations.
- Consistent with NAK: "übliche Zitierweise aus dem jeweiligen Fachgebiet (wichtig: Einheitlichkeit)" (see current formal requirements) – IEEE is the standard in Informatik.

## 10. Figures, tables, appendix

- **2 figures** (both with numbered captions below, referenced in text): Abb. 1 graph example taken from [14] (PDF p. 9); Abb. 2 own simple workflow diagram with DB attributes (PDF p. 11).
- **4 tables** (numbered captions above, all referenced in text, all own measurement data).
- Inline code: one Cypher pattern in the running text (PDF p. 9).
- **Appendix** (PDF p. 18–20, printed vi–viii): complete SQL scripts (initial set-up + scenarios 1–4) and Cypher scripts (initial set-up + scenarios 1–4) as syntax-highlighted, line-numbered listings with short labels („Initialer Aufbau (SQL)", „Szenario 2:" …). No appendix heading/index.
- Verzeichnisse: Tabellen-, Abbildungs-, Abkürzungsverzeichnis even for a 10-page paper; every abbreviation introduced at first use in the form „Business Process Management (BPM)".

---

## 11. Why it is presumably considered good – imitable patterns

Inferred from comparing the paper with NAK criteria (Methoden INF S. 18–27; Schneider Folie 11, 17, 26, 34, 36):

1. **One precise RQ, stated as a question in the intro** and restated at the start of the method chapter – the roter Faden is visible.
2. **Comparison design with explicit criteria**: objects (DB types) → representatives (justified) → metrics (justified from literature) → scenarios → measurement → interpretation. Exactly Schneider's comparison recipe (Folie 24/26) and NAK's experiment steps (Methoden INF S. 19–21).
3. **Literature is used, not decorated**: Grundlagen are restricted to what the RQ needs; related work supplies the metrics; results are checked against literature („deckt sich mit [17]").
4. **Reproducibility**: versions, data volume (1,000,000 records), repeated runs with mean and standard deviation, complete scripts in the appendix – "kann eine Person … zu den gleichen Ergebnissen kommen?" (Methoden INF S. 22).
5. **Objective vs. subjective measurements separated and labelled**, with an explicit evaluation rule for the subjective part.
6. **Honest discussion of validity**: limits of the case, an admitted design flaw (SQLite vs. full DBMS), tool artefacts – shows scientific attitude rather than "Berichtcharakter".
7. **Clear, hedged answer + Handlungsempfehlung** including an economic argument („unwirtschaftlich").
8. **Professional form**: balanced chapter proportions, max. two heading levels, all tables/figures numbered and referenced, uniform IEEE citation, abbreviations list, impersonal academic style (passive voice, no "ich"/"man").
9. **Scientific sources** dominate (proceedings, journals, standard books); web sources limited to product documentation.

### Reusable formulations (German)
- Problem → RQ: „Insofern stellt sich folgende Frage: …?"
- Goal: „… zu untersuchen ist Ziel dieser Arbeit."
- Roadmap: „Zunächst werden dafür … erläutert. … Anschließend … Um daraufhin … bewerten zu können, wird … Zuletzt wird auf Basis dieser Ergebnisse ein Fazit erstellt, womit eine Empfehlung für … abgegeben wird."
- Scoping: „…, welche allerdings zur Beantwortung der Forschungsfrage zu vernachlässigen sind."
- Method: „Um die Frage zu beantworten, welcher …, wird ein Fallbeispiel bearbeitet."
- Choice justification: „Als … wird … gewählt, da …"
- Accuracy: „Um eine höhere Genauigkeit … zu erreichen, wird es mehrmals durchgeführt, wobei das Ergebnis als Tupel von arithmetischen Mittel … sowie der Standardabweichung angegeben wird."
- Discussion opener: „Im Folgenden wird die Aussagekräftigkeit der Daten behandelt."
- Limitation: „Zunächst stellt das Fallbeispiel nur einen bedingt realistischen Fall dar." / „… wäre … von Vorteil gewesen, um …"
- Conclusion: „Insgesamt hat sich gezeigt, dass …" / „Damit spricht wenig für …"

### Skeleton to imitate (experiment/comparison TF, ~10 pages)
1 Einleitung (~1 p.: context with sources → problem → RQ → goal → procedure) · 2 Grundlagen (~3 p., only RQ-relevant concepts) · 3 Vergleichbare Arbeiten / Stand der Forschung (~0.5–1 p., derive criteria/metrics) · 4 Analyse: 4.1 Methodik (method + justification), 4.2 Fallbeispiel/Versuchsaufbau, 4.3 Ergebnisse (tables + interpretation), 4.4 (optional qualitative findings), 4.5 Diskussion (validity, limits) (~4 p.) · 5 Fazit (~1 p.: recap, answer, Handlungsempfehlung, outlook) · Quellenverzeichnis · Anhang (raw material).

---

## 12. Weaknesses – do not copy blindly

Observed in the document itself (useful so an AI reviewer does not treat everything as a model):
- **Thin company link.** The NAK slide version of the topic says "am Beispiel vom Unternehmen X" (Methoden INF S. 21), but the submitted paper uses a generic, constructed warehouse workflow and no company data, internal documents or stakeholders. Today "Die Theorie wird auf die Praxis angewendet und reflektiert" is a **K.O.-Kriterium** (Methoden INF S. 26) – a current TF should anchor the case in the employer's real situation.
- **No discussion of alternative methods** and no explicit hypothesis (cf. Methoden INF S. 18, 20).
- **Gap not stated explicitly** in the related-work chapter (cf. Schneider Folie 17 "Summarize gaps").
- **No "further research" outlook** in the Fazit (cf. Schneider Folie 34).
- **Language/typos:** „der der Tests", „ein einen höheren Speicherverbrauch", „Databanken Management Systems"; source title „PRISM Workwench" (presumably Workbench – general knowledge). BPMN expanded as „Business Process Management Notation" while its own source [3] is titled „Business Process Model and Notation".
- **Pagination glitches:** Abkürzungsverzeichnis and Quellenverzeichnis both numbered "iv"; method text refers to "Anhang S. vi - vii" although the scripts span vi–viii.
- *(General knowledge, not from source:)* SQL's query part is usually called DQL/DML; DCL normally denotes permission statements (GRANT/REVOKE). The paper labels querying as "Data Control Language (DCL)" – a technical inaccuracy a reviewer could flag.
- The SQLite-vs-Neo4j set-up is admittedly unequal (embedded vs. server) – the paper discusses this, but the recommendation still rests on that comparison.

## 13. Cross-references
- Method background (experiment steps, comparison design, grading criteria): [scientific_methods.md](<scientific_methods.md>)
- Current formal requirements: [2026_Formale Anforderungen.pdf](<../originals/2026_Formale Anforderungen.pdf>) · IEEE citation guide: [IEEE.pdf](<../originals/IEEE.pdf>)
