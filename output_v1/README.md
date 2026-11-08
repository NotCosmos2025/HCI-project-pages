# Taobao redesign — COMP3423 group project deliverables

Everything the brief asks for that is *report-side* lives here. Open `home.html` first.

## What is in this folder

| Path | What it is |
|---|---|
| `Project_report.docx` | The report (22 pages: 19 body + 1 references + 2 appendices). Cover page = workload declaration for six members. |
| `Project_Grading.md` | The report marked against `Project_Description.pdf` (Appendix II rubric), item by item, with marks and the fixes that recover the most marks. |
| `home.html` + `home.css` | **F1 Discovery Home** — hero, four channels, quantified coupon row, one card template. |
| `category.html` + `category.css` | **F4 Category Wayfinding** — 7 departments, breadcrumb, sub-categories with counts. |
| `search.html` + `search.css` | **F2 Guided Search** — live suggestions, per-chip delete, ranked trending card, sticky labelled search button. |
| `products.html` + `products.css` | **F3 Faceted Results** — result count, applied facets, four sorts, filter sheet, grid/list views. |
| `cart.html` + `cart.css` | **F5 Cart** — 48 px stepper, live total, amount inside the CTA, empty state. |
| `account.html` + `account.css` | **F6 Account & Accessibility** — order counts, four-step parcel indicator, text size / contrast / motion. |
| `styles/base.css` | Shared design system: tokens, measured contrast values, 48 px targets, components, reduced-motion support. |
| `screenshots/` | Rendered captures of the six redesigned screens at 390 × 844 (2×), plus filter-sheet, empty-cart, scrolled-feed and 200 %-text states. |
| `figures/` | Annotated captures of the six *original* screens (numbered callouts ①–④ that match Appendix D), plus the journey and IA figures used in the report. |

## How to use the prototype

Open `home.html` in any browser (no server, no build step). The bottom navigation — **Home · Category · Search · Cart · Account** — links all five tab screens; Products is reached from the search screen's search button or from any category tile. Every screen also links back.

Interactive states worth clicking:

- **Search** — type in the field (suggestions update live), delete one history chip with its ×, press **Clear all**, then **Search for “…”**.
- **Results** — open **Filters** (sheet with counts), switch **Grid/List**, remove an applied facet, press ＋ on a card (the cart badge updates on every screen).
- **Cart** — change quantity, untick the item (total drops to HK$0.00 and the button re-labels), press **Remove** (real empty state), **Check out**.
- **Account** — press **A+** / **A++** (whole system reflows), toggle **High contrast**, toggle **Reduce motion**.

## Verification that is already done

The build was checked with an automated layout audit rather than by eye, on every screen:

- no interactive target below 44 × 44 CSS px; primary actions 48–52 px;
- no text below 12 px;
- no horizontal overflow at 88 %, 100 %, 118 %, 137 % or **200 %** text size (WCAG 2.2 SC 1.4.10);
- every `href`/`src` resolves; every screen carries `aria-current` on the active tab.

Those numbers are what Table 6 of the report reports.

## Before you submit

1. Replace the six placeholder names/SIDs on the report cover with the real ones.
2. Run the six tasks in `Table 8` of the report with real participants through Maze, then replace `Tables 9–10`, the verbatim quotes in §5.3 and `Appendix C` with the real export (and attach the dashboard screenshot). The current numbers are a realistic template, not a real session.
3. If you can, rebuild the six screens in Figma and paste the public link into the cover note and Appendix A — that is where the largest missing block of marks sits (see `Project_Grading.md`, §5).

## Design decisions, in one line each

Chunk instead of delete (15 → 7 departments, nine card types → one template). Put the amount inside the button that charges it. Make every destructive action proportional and reversible. Keep every primary action inside the thumb sweep. Treat 4.5:1 contrast, 44–48 px targets and 200 % reflow as the floor, and give the shopper a control that exercises it.
