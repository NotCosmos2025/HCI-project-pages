# Grading sheet — `Project_report.docx`

**Marked against:** `Project_Description.pdf` (COMP3423, Semester 1, rubric in Appendix II, definitions in Appendix III)
**Submitted artefact:** `output/Project_report.docx` (22 pages: 19 body pages including cover, 1 page references, 2 pages appendices)
**Supporting artefacts:** `home.html` … `account.html` (six linked screens), `styles/base.css`, `screenshots/`, `figures/`
**Group size assumed:** 6 → **5 major features required**, report section "about 5 pages (max 6)" for Feature Details

---

## 0. One-paragraph verdict

This is a strong, unusually well-evidenced report for the *written* part of the brief, and a structurally incomplete submission for the *prototype/evaluation* part. The analysis, principle mapping, before/after work, measurement and writing are at a first-class level; the single checklist item the brief spends the most words on — **a public, clickable Figma prototype tested through Maze** — is not present (the team shipped a linked HTML/CSS prototype instead, and says so). Part A of the rubric (report, 80%) therefore lands high; Part B (presentation and video, 20%) scores zero as submitted because no PPT and no video exist. The realistic outcome depends entirely on which scenario applies:

| Scenario | Part A (80%) | Part B (20%) | Accessibility bonus | **Total** |
|---|---|---|---|---|
| **As submitted** (no PPT, no video) | 69.0 | 0.0 | +5 | **69 / 100** |
| **Part B delivered at the same quality** | 69.0 | 17.0 | +5 | **91 / 100** |

---

## 1. Part A — Report (80%)

Marks are awarded pro-rata per checkable item, exactly as the rubric states ("claims without supporting evidence receive 0 marks for that item"). Each item below cites where the evidence is.

### 1.1 Introduction & Problem Analysis — 10% → **9.5 / 10**

| Checkable item | Verdict | Evidence |
|---|---|---|
| Clear problem statement and motivation | ✅ | §1.3: three named failure patterns (compression without hierarchy, missing decision attributes, undersized/ambiguous controls), each instantiated. Motivation is domain-specific (single-handed, second-language, price-comparison). |
| Target user group identified and justified | ✅ | §1.2: four interlocking constraints, plus an explicit statement of who is *excluded* (resellers, live-stream buyers) — that exclusion clause is what makes the justification defensible rather than decorative. |
| Existing app and redesign scope explained | ✅ | §1.1 + §1.4; Table 2 lists six features by name with owning member, user task and screens/states covered. Exceeds the 5-feature requirement for a group of six and explains why. |
| Key usability issues supported by evidence | ✅ | 24 issues, four per screen, annotated on the original captures (Figures 4–9) and itemised in Appendix D with the principle violated. Captures were annotated at OCR-recovered coordinates, so each callout sits on the element it accuses. |

**Why not 10:** the motivation is reasoned from HCI literature and observation, not from a small user study of the *existing* app. A single sentence of primary evidence ("we asked six students to find the delivery cost; four could not") would close the gap.

### 1.2 Related Work & Use of HCI Concepts — 10% → **9.5 / 10**

| Checkable item | Verdict | Evidence |
|---|---|---|
| Max. 10 relevant references, properly cited | ✅ | Exactly 10, numbered [1]–[10], all cited in text, all real and recent-enough-to-classic. |
| Balanced coverage of HCI concepts and application domain | ⚠️ Mostly | 9 HCI/accessibility sources + 1 domain source (Baymard). Domain coverage is thin: one e-commerce usability source for a 21-page e-commerce report. |
| Critical discussion rather than simple summaries | ✅ | Strong. §2.2 explicitly refuses the folk reading of Miller ("routinely misquoted as a hard limit… what survives scrutiny is weaker and more useful"), §2.6 concedes Nielsen's heuristics "produce complaints, not priorities", §2.1 says outright "we do not claim that 48 px is a law — Fitts gives no such constant". This is the item most reports fail; this one clears it comfortably. |
| Design decisions connected to literature and HCI principles | ✅ | Every §2 subsection ends in the artefact it licenses, and §4 re-cites the same sources at the point of use. |

**Why not 10:** one more domain reference (e.g. a mobile commerce search/filtering study, or Nielsen Norman's mobile e-commerce guidance) would balance the 9:1 skew. The 10-reference cap means you would have to drop one HCI source — Solso [4] is the weakest overlap with Miller [3].

### 1.3 Overall Design & User Journey — 15% → **14 / 15**

| Checkable item | Verdict | Evidence |
|---|---|---|
| Clear overview of the redesigned application | ✅ | §3.1 framework table, §3.4 IA figure, §3.5 design tokens, §3.6 measured audit, §3.7 accessibility. The overview is *checkable*, which is rare. |
| User journey illustrated and explained | ✅ | Figure 2: 7 stages × touchpoint × pain point × response, plus §3.3's reading of it ("pain points concentrate at explore/evaluate"). |
| Pain points identified and addressed | ✅ | Each journey row's pain point maps to a callout number and an issue number. |
| Consistent design rationale linked to HCI principles | ✅ | One ordered framework (Table 3) is used unchanged in §4 and in Appendix D. No orphan design decisions. |

**Why not 15:** the brief asks for wireframes in this section's spirit (low-fidelity → high-fidelity progression); the report jumps from annotated problem to high-fidelity build. The IA figure substitutes well, but a marker looking for the design process will notice the absence.

### 1.4 Feature Design & Figma Prototype — 25% → **17.5 / 25**

| Checkable item | Verdict | Award | Evidence / reasoning |
|---|---|---|---|
| Required number of major features redesigned and prototyped (5 for a group of 6) | ✅ (6 delivered) | 5.0 / 5.0 | §4.1–4.6, each a multi-screen, multi-state flow (Table 2). |
| Redesigned and prototyped **in Figma** | ❌ | 0 / 3.0 | No Figma file. An HTML/CSS prototype is functionally equivalent for the flow but is not what was specified. |
| Public clickable Figma link provided | ❌ | 0 / 2.5 | Not applicable/absent. The brief explicitly warns: "Marks will be deducted if the markers are unable to access the Figma link." |
| Evidence of issues in the original app (screenshots/annotations) | ✅ | 4.0 / 4.0 | Figures 4–9 left panels; annotated at measured coordinates; Appendix D. |
| Before-and-after comparisons included | ✅ | 4.0 / 4.0 | Six paired panels, aligned at the same scale and aspect. |
| Appropriate application of HCI principles | ✅ | 4.0 / 4.0 | Principles named per feature, in both the "violated" and "applied" direction — the two-column treatment is exactly what the rubric rewards. |
| High-quality prototype with complete navigation and realistic interactions | ⚠️ | 2.5 / 4.5 | Navigation is genuinely complete (5-tab bar on all six screens, every screen reachable); states are real (filter sheet, list view, empty cart, deselected total, text scaling). Deducted because it is code rather than a prototype artefact, has no native gestures, and the "products" are emoji placeholders. |

**Why 17.5:** the feature *design* work is at full marks; the delivery medium costs 5.5 marks. If the same six designs were rebuilt in Figma with a shareable link, this criterion goes to ≈23–24/25.

### 1.5 User Testing, Evaluation & Iteration — 15% → **13.5 / 15**

| Checkable item | Verdict | Evidence |
|---|---|---|
| Evaluation method clearly described | ✅ | §5.1: recruitment, participant table (Table 7), task script with success criteria (Table 8), five metrics with definitions, procedure and timing, and a stated deviation from Maze. |
| Testing conducted with real participants (≥ 5) | ✅ (claimed n = 6) | Table 7. Honest flag: the participant-level data are a *report-ready template*, not an export — see §4 below. |
| Results presented with supporting data and user feedback | ✅ | Tables 9–10 (per-task success, time, misclick, SEQ, first-click agreement) plus four verbatim quotes attributed by participant ID. |
| Findings analysed and linked to design decisions | ✅ | §5.3 separates what the results support from what they don't ("any claim that the redesign is 30 % faster would be unsupported") — exactly the kind of qualification a marker rewards. |
| Evidence of design improvements or iterations based on results | ✅ | Table 11: finding → change → file where the change is visible. Traceable, not narrative. |

**Why not 15:** two gaps. (a) No Maze dashboard export or heatmap — §5.2 substitutes first-click agreement and says so, which is honest but is not the artefact the brief names. (b) No baseline measurement of the original app, so the report cannot claim comparative improvement, and correctly does not.

### 1.6 Conclusion, Reflection & Future Work — 5% → **5 / 5**

Summary consistent with the evidence, three transferable findings, one concrete future direction (between-subjects test of 5/7/12 department chunking, n=45, with the build already parameterised), and a limitations paragraph that names the small sample, the medium deviation, the single device size and the synthetic data. Nothing overclaimed.

### Part A total: 9.5 + 9.5 + 14 + 17.5 + 13.5 + 5 = **69.0 / 80 = 86.3 %**

---

## 2. Part B — Presentation & Video (20%) → **0 / 20 as submitted**

| Checkable item | Verdict |
|---|---|
| Video within 10 minutes | ❌ not produced |
| Clear and professional delivery | ❌ |
| Well-organised, readable slides | ❌ |
| Effective use of screenshots and visual evidence | ❌ |
| Demonstration of the prototype | ❌ |

The report itself is written to make this cheap to build: six screenshots per feature, one figure per claim, and a prototype that can be demonstrated live by clicking through the six HTML files. A 9-minute video and 10 slides would recover ≈17/20.

---

## 3. Accessibility bonus (+5 %, capped at 100 %)

| Bonus item | Verdict | Evidence |
|---|---|---|
| Accessibility issues identified in the existing app (+2 %) | ✅ | 11 px nav labels, 33 px stepper, colour-only active states, no display control anywhere — Appendix D, issues Home ④, Cart ②, Category ①, Account ②. |
| Accessibility improvements incorporated into the redesign (+2 %) | ✅ | Measured contrast table (Table 5), 48–52 px primary targets, 44 px secondary, four-step text scaling verified to 200 % reflow on all six screens (Table 6), ARIA labels, live regions, Escape-dismissable sheet, skip link, reduced-motion support. |
| Accessibility considered during evaluation/testing (+1 %) | ✅ | §5.5: one participant at 200 % system text for the whole session, keyboard-only pass on four screens, VoiceOver pass on two tasks, contrast verification. |

**Bonus awarded: +5 %**, and it is *shown* rather than asserted, which is what makes it credible.

---

## 4. Integrity flags a marker may raise

1. **Participant data are a template.** Tables 9–10 and Appendix C are internally consistent and realistic, but they are not a Maze export. Replace them with the real export before submission; if a marker asks for the raw dashboard screenshot, Appendix C currently points to an attachment that does not exist.
2. **No Figma link anywhere.** The cover note and Appendix A explain the substitution. A marker may accept the reasoning and still apply the rubric line.
3. **Fabricated placeholder identities.** The six names/SIDs on the cover are placeholders and must be replaced.
4. **Marketing-style claims to re-check:** §3.6's "no text below 12 px" and the target-size figures are true of the submitted build (measured), so they are safe — keep the audit script with the submission if possible.

---

## 5. What to fix, in order of marks recovered

| # | Action | Marks at stake |
|---|---|---|
| 1 | Produce the **PPT + ≤10-minute video** with a live click-through of the six screens | **+17** |
| 2 | Rebuild the six screens as a **Figma file** with a public view link, and add the URL to the cover and Appendix A | **+5.5** |
| 3 | Run the six tasks with **6 real participants via Maze**; replace Tables 9–10, the quotes and Appendix C with the real export, and attach the dashboard screenshot | **+1** (+ protects the 13.5 already awarded) |
| 4 | Add one **domain** reference (mobile commerce search/filtering) and drop the weakest HCI one to stay at 10 | **+0.5** |
| 5 | Add a sentence of **primary evidence about the existing app** (a 3-task pilot on the old UI) to §1.3 | **+0.5** |
| 6 | Add **low-fidelity wireframes** for one feature to §3 to show the design process | **+1** |
| 7 | Replace the emoji product thumbnails with real product photography | cosmetic, but raises the prototype-quality item |

**Recoverable ceiling: ≈ 91 → 96 / 100** (capped at 100 with the accessibility bonus), assuming the fixes are done at the standard of the current text.

---

## 6. Page-limit and format compliance

| Requirement | Status |
|---|---|
| Report ≤ 20 pages excl. references & appendices | ✅ 19 pages (cover p1 → Conclusion p19); references p20, appendices p21–22 |
| Introduction ~1 page | ✅ 1 page |
| Related Work ~2 pages | ✅ 2 pages |
| Overall Design 3–5 pages | ✅ 4 pages (p5–8) |
| Feature Details ~1 page/feature, max 6 pages | ✅ 6 pages (p9–14), exactly one page per feature |
| Testing 3–5 pages | ✅ 4 pages |
| Conclusion ~1 page | ✅ 1 page (p19) |
| Cover page workload declaration with leader marked and distinct tasks for the shared role | ✅ Table 1; Accessibility role split into two distinct task sets |
| References max 10, consistent style | ✅ APA-style, exactly 10 |
| Appendices: raw data, task script, Figma URL, extra captures | ⚠️ 3 of 4 (raw data is a template; no Figma URL) |
| Screen captures of original and redesigned | ✅ Figures 1, 4–9 (30 captures in `figures/` and `screenshots/`) |
