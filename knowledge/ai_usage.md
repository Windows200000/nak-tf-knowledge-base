# AI usage: policy, Eigenständigkeitserklärung, Prozessdokumentation

**Sources:** [converted_faq-2305.md](<../originals/converted_faq-2305.md>) ("Einsatz von KI als Hilfsmittel", "Nutzung von ChatGPT & Co.") · [2024_10Eigenständigkeitserklärung KI.pdf](<../originals/2024_10Eigenständigkeitserklärung KI.pdf>) ([txt](<../originals_text/2024_10Eigenständigkeitserklärung KI.txt>)) · [NAK_Prozessdokumentation_KI_final.docx](<../originals/NAK_Prozessdokumentation_KI_final.docx>) (blank form, [txt](<../originals_text/NAK_Prozessdokumentation_KI_final.txt>)) · [NAK_Prozessdokumentation_KI_final_20250219.pdf](<../originals/NAK_Prozessdokumentation_KI_final_20250219.pdf>) (filled example, [txt](<../originals_text/NAK_Prozessdokumentation_KI_final_20250219.txt>)) · [2026_Formale Anforderungen.pdf](<../originals/2026_Formale Anforderungen.pdf>)

> **Relevance for this repo:** this knowledge base exists to have AI assist with TFs. Everything an AI contributes to the TF text, outline, ideas, wording, code or calculations must therefore be documented. AI assistants using this repo must remind the student to log their prompts. See the logging rule in [../CLAUDE.md](../CLAUDE.md).

## Policy (FAQ, verbatim core)

- *"Grundsätzlich ist die Nutzung von generativer KI als Hilfsmittel zugelassen, Voraussetzung ist dafür eine transparente Dokumentation."*
- On 22.10.2024 NAK published a *"Richtlinie zum Einsatz generativer Künstlicher Intelligenz bei Prüfungsleistungen, Studienleistungen und Abschlussarbeiten"*. It is valid from publication. (The guideline itself is **not in this dump**.)
- If AI was used, upload a **Prozessdokumentation** in CIS in addition to the TF and Selbstreflexion, *"in der transparent Prompts zur besseren Nachvollziehbarkeit eingegeben werden müssen"*. Also upload the **Eigenständigkeitserklärung** as a separate document.
- **If no AI was used:** NAK recommends informing the examiner in a note in the **first footnote**.
- *"Wenn eine Nutzung nicht oder fehlerhaft angegeben ist, liegt eine Täuschung vor und die Arbeit ist nicht bestanden."* For Prüfungsleistungen the examiner may also demand an oral defence.
- Formale Anforderungen 2026: *"Eigenständigkeitserklärung hochladen"* · *"Prozessdokumentation über KI-Nutzung anfügen"*.
- The Prozessdokumentation PDF header says the level of detail should be agreed with the examiner, *"ausgenommen sind Transferleistungen. Bei Rückfragen bitte an transferleistungen@nordakademie.de"*. So for TFs there is no individual agreement and the standard form applies.

## Eigenständigkeitserklärung (verbatim text, 2024_10 version)

> Mit meiner Unterschrift versichere ich, dass ich die hier vorliegende Arbeit selbständig, ohne fremde Hilfe und nur mit den angegebenen Hilfsmitteln verfasst habe und meine Angaben zu den verwendeten Quellen der Wahrheit entsprechen und vollständig sind. Alle Quellen, aus denen ich wörtlich oder sinngemäß übernommen habe, habe ich als solche gekennzeichnet.
>
> Darüber hinaus versichere ich, dass ich **sämtliche Teile der vorliegenden Arbeit, die unter Zuhilfenahme künstlicher Intelligenz (KI) generiert wurden, als solche gekennzeichnet habe und deren Entstehung in einer beigefügten Prozessdokumentation nachgewiesen habe.**
>
> Ich habe zur Kenntnis genommen, dass zuwiderlaufendes Verhalten als Täuschungsversuch gewertet wird und zu den in der geltenden Prüfungsverfahrensordnung genannten Konsequenzen führen wird.
>
> \<Ort\>, den \<Datum\> · \<Vorname Nachname\>

Note: this declaration carries the student's **name**. That is why it is a separate upload and never part of the anonymised TF PDF.

So AI-generated parts must be **marked in the text** *and* documented in the Prozessdokumentation. The example below shows marking via page references (*"vgl. S. 7"*).

## Prozessdokumentation form

Title: *"Prozessdokumentation — Für die Nutzung von Künstlicher Intelligenz (KI) in Prüfungs-, Transfer- und Studienleistungen"*. A 4-column table:

| Anfrage an folgende KI* (inkl. Abrufdatum) | Grund für die Verwendung der KI | Bewertung der Qualität des KI-Outputs | Verwendete Software und Versionsnummer |
|---|---|---|---|

\* *"Bitte formulieren Sie Ihre Anfrage und nennen Sie die verwendete KI."* Footer: *"Nach Dr. Ulrike Hanke Hochschuldidaktische Weiterbildungen - Hanke Teachertraining"*.

## NAK's filled example (20250219 PDF): what "good" looks like

Each row: the **verbatim prompt in quotes + date + page reference** where the output was used, the **reason**, a **critical assessment** (what was useful, what was wrong, how it was verified against literature), and **tool + version**. Selected rows (verbatim):

| Anfrage | Grund | Bewertung | Software |
|---|---|---|---|
| „Gib mir eine Auswahl an Themen für eine Hausarbeit im Zusammenhang mit Datenbanken." 19.02.2025; vgl. S. 5 | Themenfindung | Hilfreicher Input; einige Titel haben keinen Sinn ergeben. Je mehr ich spezifiziert habe, desto besser wurde das Ergebnis. | ChatGPT 4.0 |
| „Erstelle mir eine Gliederung für eine Hausarbeit zum Thema erneuerbare Energien." 19.02.2025; vgl. S. 5 | Impulse, erstes Konzept, Hauptsache etwas auf Papier | Wesentliche Bestandteile genannt …; hilfreicher Einstieg …; es fehlt aber an Konkretisierung, insbesondere zu Themen aus der Praxis | ChatGPT 4.0 |
| „Erstelle mir eine Formel für die Stichprobenberechnung." 19.02.2025; vgl. S. 5 | Erklärung; Herleitung der Formel | Hilfreich … Aber Achtung: Zum Teil fehlerhaft; Beispiel verifiziert in Literatur und im Ansatz genutzt vgl. S. 7 | ChatGPT 4.0 |
| „Welche Methode eignet sich, um Softwaretests im Unternehmen durchzuführen?" 19.02.2025; vgl. S. 5 | Es fehlten Beispiele aus der Praxis | … Quellen nicht zitierwürdig, u.a. wikipedia | Perplexity ai |
| „Schreibe folgenden Absatz um. Ziel ist es, wissenschaftlich und präzise zu formulieren." 19.02.2025; vgl. S. 5 und 8-9 | Formulierungshilfe, da Sätze oft langatmig sind … Schwierigkeiten mit der Kommasetzung. | Präziser formuliert; fehlerfrei (vgl. S. 5, 7-8, 10, 13) | DeepL Write |
| GitHub Copilot für Code (durchgängig genutzt) 19.02.2025 | Korrekturassistent; … Zeitersparnis | Gegengeprüft, ob richtig vervollständigt wurde. | GitHub Copilot |

Further rows cover: idea generation ("Du bist Umweltexperte…"), topic overviews (Microsoft Copilot: *"Forschungsergebnisse waren nicht aktuell"*), interview procedure (*"ersetzt aber nicht Grundlagenliteratur zu empirischer Forschung"*), definitions (BPMN), a gap-filler where the literature had nothing ("Farbe Türkis auf Verpackungen"), explaining complex concepts (*"mit der Literatur abgeglichen, verwendet und gekennzeichnet"*), and code translation Java→Python. So even **grammar tools (DeepL Write) and code completion (Copilot)** are logged.

## Practical rules for AI-assisted TF work (derived)

1. **Log every AI interaction that influences the TF**: topic finding, outline, explanations, wording or rewriting, translation, code, calculations, *and reviews*. Record the date, the verbatim prompt (or a faithful summary for long chats), the reason, a critical quality assessment, the page(s) affected, and the tool + model/version.
2. **Never cite AI as a source of facts.** Verify every AI-provided claim, formula or reference against real literature and cite that literature (the example does exactly this).
3. **Mark AI-generated text** in the TF where it is used (the Eigenständigkeitserklärung requires it). Better still: use AI for feedback and restructuring, and write the final text yourself.
4. A template for the log is in [../templates/ki_prozessdokumentation.md](../templates/ki_prozessdokumentation.md). The Typst template has a built-in `ai_documentation` table; see [typst_template.md](typst_template.md).
5. AI-suggested references must be checked for existence (DOI/Crossref), because hallucinated citations amount to falsified sources.
