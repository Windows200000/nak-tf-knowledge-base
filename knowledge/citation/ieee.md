# IEEE — numeric [n] citation style (common in computer science and engineering)

**Source:** [IEEE.pdf](<../../originals/IEEE.pdf>) · full text: [txt](<../../originals_text/IEEE.txt>)

## About this source

- *Zitations-Styleguide IEEE*: 4 pages, no author or institution named. **Not identifiable as a NAK document.**
- It is mostly a German frame around two quoted English excerpts:
  - [1] *IEEE Transactions, Journals and Letters (2006): Information for Authors*, IEEE Periodicals.
  - [2] *TeLaRS Web Team (2005): IEEE Style*, The University of Melbourne.
- The guide says the IEEE citation style quoted from [1] „hier als Maßstab festgesetzt werden soll“ (p. 1).
- It recommends **BibTeX** for managing references (p. 1).
- Page refs = PDF pages (no printed numbers).
- **Age warning (general knowledge, not from source):** the electronic-source formats come from a 2005 guide and are outdated. Current IEEE style (IEEE Reference Guide) writes online sources as `… [Online]. Available: URL`, adds an access date (`Accessed: Mon. DD, YYYY.`), and includes issue numbers (`no. x`). Use the guide's print formats as the core, and modernise electronic entries consistently if needed.

## NAK context (from other repo documents)
- NAK's example of a well-graded TF, [Gute TL Informatik.pdf](<../../originals/Gute TL Informatik.pdf>) (PDF p. 16, "Quellenverzeichnis"), uses IEEE numeric style with German localisation. Verbatim examples:
  - `[3] Object Management Group, BPMN Speciﬁcation - Business Process Model and Notation, 2019. [Online]. Verfügbar unter: http://www.bpmn.org/. [Zugegriﬀen: 25. Sep 2019].`
  - `[1] W. van der Aalst und K. M. van Hee, Workﬂow management: Models, methods and systems, 1. MIT Press paperback ed. Cambridge, Mass.: MIT Press, 2004.`
  - In that example the bracket follows the sentence period (`… bearbeitet werden können.[1]`). That **contradicts** this guide's rule that the bracket goes *inside* the punctuation.
- The NAK Typst template ([nak-typst-template-main](<../../originals/nak-typst-template-main/README.md>)) defaults to `citation_style: "ieee"` with a BibTeX file (`src/components/transfer_paper.typ`).
- ⚠ Tension: NAK's *Transferleistung_Tipps zur Anfertigung* (pp. 3, 5) asks for an „alphabetisches Quellenverzeichnis“ sorted „nach Autoren“. IEEE lists references **in order of first citation, not alphabetically**. Both NAK documents also say the style is „übliche Zitierweise aus dem jeweiligen Fachgebiet“. IEEE is customary in computer science and engineering, but less so in business / industrial engineering (*Wirtschaftsingenieurwesen*). See [README](README.md).

## 1. In-text citations (pp. 1–2, quoted from [1])

"The IEEE Style is an number style with two key components":
1. **In-text citations:** a citation number in square brackets.
2. **A reference list** at the end of the text, with full details of all references cited.

„It is important to BE CONSISTENT when you are referencing.“

### Citation numbers are… (p. 1)
1. Arabic numbers assigned to each reference **as it is cited**: the first reference is [1], the second [2], and so on.
2. **Reused** each time that reference is cited again.
3. In square brackets placed **inside** punctuation marks, colons and semicolons:
   - `"...was the most significant [4]."`
   - `"...had asserted [4]: further research..."`
4. Multiple references, **without spaces**:
   - non-inclusive: joined by commas, e.g. `Though unlikely, the same effects was reported by [2,4,7,10]`
   - inclusive: joined by a hyphen, e.g. `Motion or centrifugation can speed up the diagnosis of some viral infections [2-5]`

### Author-name substitution (p. 1)
The reference number can stand in for the author's name:
```
As [1], [2], and [3] demonstrate, the natural course of microprocessor evolution will likely lead to computers with...
According to [2], current Internet technology is still years behind industry projections...
```

### Note placement (p. 2)
Place the number **directly after the reference**, not necessarily at the end of a clause or sentence (though sometimes it will fall there):
```
One study [2] examined the mRNA levels of Jun C, Jun B, and Jun D in mouse tissues.
Current Internet technology is still years behind industry projections, one study suggested [2].
```

### Multi-reference citations (p. 2)
Separate the numbers with commas and **no spaces**: `[2,7,12]`. Ranges: `[19-22]`.

### More in-text rules (p. 2, quoted from [2])
- Write simply „in [1] …“, not „in reference [1] …“.
- „it is not necessary to mention the authors of a reference unless the mention is relevant to the text. It is almost never useful to give dates of references in text.“
- Phrases such as „For example,“ don't belong in the reference list. Put them in parentheses in the text: „For example, see [5].“

*(General knowledge, not from source: to cite a specific page, IEEE usually writes `[1, p. 45]` or `[1, pp. 45–47]`. The guide does not cover page-specific citation. Paraphrase markers like „vgl.“ are not used in IEEE.)*

## 2. Reference list (Bibliografie)

Rules (p. 2, quoted from [2]):
- „A numbered list of references must be provided at the end of the paper.“
- „The list should be arranged in the **order of citation in text, not in alphabetical order**.“
- „List only one reference per reference number.“
- „Each reference number should be enclosed by square brackets.“
- „Footnotes or other words and phrases that are not part of the reference format do not belong on the reference list.“

German note from the guide (p. 3): „Wichtig ist, auf die Vollständigkeit (Seitenzahlen, Datum, Ort, …) und das Layout (Reihenfolge, Abkürzungen von Namen, Anführungszeichen, Kursiv etc.) der spezifischen Informationen pro Quellentyp zu achten!“

Formatting conventions visible in the examples (pp. 2–3):
- Author: **initials first, then surname** (`G. O. Young`, `W.-K. Chen`). Two authors are joined with „and“; three or more with commas plus „, and“.
- Article or chapter titles in double quotes, with the comma **inside** the quotes.
- Abbreviations: `vol.`, `pp.`, `ed.`, `Ed.`, `Tech. Rep.`, abbreviated months (`Jan.`, `Dec.`, `Nov.`), abbreviated journal names (`IEEE Trans. Electron Devices`, `Phys. Rev.`).
- Page ranges use an en dash (`15–64`).
- *(General knowledge, not from source: book and journal titles are italic in IEEE. The extraction loses italics.)*

### Print sources: examples (pp. 2–3, verbatim)

**Books**
```
[1] G. O. Young, “Synthetic structure of industrial plastics,” in Plastics, 2nd ed., vol. 3, J. Peters, Ed. New York: McGraw-Hill, 1964, pp. 15–64.
[2] W.-K. Chen, Linear Networks and Systems. Belmont, CA: Wadsworth, 1993, pp. 123–135.
```
([1] is a chapter in an edited book; [2] is a monograph.)

**Periodicals**
```
[3] J. U. Duncombe, “Infrared navigation—Part I: An assessment of feasibility,” IEEE Trans. Electron Devices, vol. ED-11, pp. 34–39, Jan. 1959.
[4] E. P. Wigner, “Theory of traveling-wave optical laser,” Phys. Rev., vol. 134, pp. A635–A646, Dec. 1965.
[5] E. H. Miller, “A note on reflector arrays,” IEEE Trans. Antennas Propagat., to be published.
```

**Articles from conference proceedings (published)**
```
[6] D. B. Payne and J. R. Stern, “Wavelength-switched passively coupled single-mode optical network,” in Proc. IOOC-ECOC, 1985, pp. 585–590.
```

**Papers presented at conferences (unpublished)**
```
[7] D. Ebehard and E. Voges, “Digital single sideband detection for interferometric sensors,” presented at the 2nd Int. Conf. Optical Fiber Sensors, Stuttgart, Germany, 1984.
```

**Standards/Patents**
```
[8] G. Brandli and M. Dick, “Alternating current fed power supply,” U.S. Patent 4 084 217, Nov. 4, 1978.
```
(The only example under this heading is a patent. No standard is shown.)

**Technical reports**
```
[9] E. E. Reber, R. L. Mitchell, and C. J. Carter, “Oxygen absorption in the Earth’s atmosphere,” Aerospace Corp., Los Angeles, CA, Tech. Rep. TR-0200 (4230-46)-3, Nov. 1968.
```

### Electronic sources (pp. 3–4, quoted from [2])

The basis is described as „a modified illustration of the adaptation by the International Standards Organization (ISO) documentation system and the American Psychological Association (APA) style“.
- Three pieces of information are required: „1) protocol or service; 2) location where the item is to be found; and 3) item to be retrieved.“
- „It is not necessary to repeat the protocol (i.e., http) in Web addresses after “Available” since that is stated in the URL.“

| Type | Template (verbatim) | Example (verbatim) |
|---|---|---|
| Books | `Author. (year, month day). Title. (edition) [Type of medium]. volume (issue). Available: site/path/file` | `[1] J. Jones. (1991, May 10). Networks. (2nd ed.) [Online]. Available: http://www.atm.com` |
| Journals | `Author. (year, month). Title. Journal. [Type of medium]. volume (issue), pages. Available: site/path/file` | `[2] R. J. Vidmar. (1992, Aug.). On the use of atmospheric plasmas as electromagnetic reflectors. IEEE Trans. Plasma Sci. [Online]. 21(3), pp. 876–880. Available: http://www.halcyon.com/pub/journals/21ps03-vidmar` |
| Papers presented at conferences | `Author. (year, month). Title. Presented at Conference title. [Type of Medium]. Available: site/path/file` | `[3] PROCESS Corp., MA. Intranets: Internet technologies deployed behind the firewall for corporate productivity. Presented at INET96 Annu. Meeting. [Online]. Available: http://home.process.com/Intranets/wp2.htp` |
| Reports and handbooks | `Author. (year, month). Title. Company. City, State or Country. [Type of Medium]. Available: site/path/file` | `[4] S. L. Talleen. (1996, Apr.). The Intranet Architecture: Managing information in the new paradigm. Amdahl Corp., CA. [Online]. Available: http://www.amdahl.com/doc/products/bsg/intra/infra/html` |
| Computer programs and electronic documents | „ISO recommends that capitalization follow the accepted practice for the language or script in which the information is given.“ | `[5] A. Harriman. (1993, June). Compendium of genealogical software. Humanist. [Online]. Available e-mail: HUMANIST@NYVM Message: get GENEALOGY REPORT` |

The guide's own bibliography (p. 4, verbatim), which is also an example of citing a corporate/web document:
```
[1] IEEE Transactions, Journals and Letters (2006, 01). Information for Authors. IEEE Periodicals Transactions/Journal Department. New York. [Online]. Available: http://www.ieee.org/portal/cms_docs/pubs/transactions/auinfo03.pdf
[2] TeLaRS Web Team (2005, 02). IEEE Style. The University of Melbourne. [Online]. Available: http://www.lib.unimelb.edu.au/cite/ieee/citing.html
```

## Not covered by the source
The guide has nothing on: websites without a report format, access dates, laws, norms/standards (heading only), company-internal documents, interviews, e-mails, or AI tools. For TFs with internal sources, use [internal_sources.md](internal_sources.md) and adapt it to the numeric format. *(Suggestion, not from source: `[n] Melter AG, "Qualitätsmanagementhandbuch, Version 3.0," internal document [Intern], München, 2016. Available: Anhang A-1.`. Keep one consistent pattern and attach the document in the appendix, as NAK requires.)*

## Common mistakes / reviewer checks
- Reference list sorted alphabetically instead of by first citation.
- A reference given a new number when cited again (numbers must be reused).
- Spaces inside multi-citations (`[2, 4]` instead of `[2,4]`, per this guide). Ranges not collapsed (`[2,3,4,5]` instead of `[2-5]`).
- The bracket placed after the period instead of inside the punctuation.
- Author names and years written into the text out of habit (“Müller (2019) [3] …”). Use `[3]` as the noun instead, e.g. „According to [3], …“
- Full first names instead of initials. Surname written first.
- Mixed German/English labels (`S.`/`pp.`, `Hrsg.`/`Ed.`, `Verfügbar unter`/`Available`). Choose one language and keep it.
- Phrases or annotations inside reference-list entries.
- Missing completeness: pages, month/year, place, publisher.

## Quirks inside the source
- The verbatim quotes keep the source's typos: „an number style“, „the same effects was reported“, „Ebehard“.
- Under "Note Placement", the guide shows a reference *mid-sentence directly after the subject* („One study [2] …“). That does not contradict the punctuation rule; both say to place it right after the referenced item.
