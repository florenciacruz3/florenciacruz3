# Accessibility Audit — Store Sales Power BI Report

**Auditor:** Florencia Cruz

**Date:** July 2026

**Tool:** Accessible Report Design Checklist (self-authored)

**Pages evaluated:** Store Sales Overview, District Monthly Sales, New Stores

---

## Page 1 — Store Sales Overview

**Finding 1** — Color used as the only signal on the bubble chart

The bottom-right scatter/bubble chart uses teal and grey bubbles to distinguish New Store from Same Store. The only way of telling this apart is using color — no shape, pattern, or label distinguishes the two series for a colorblind user.

Checklist reference: Section 1 — Color and Contrast
Color shouldn't be the only means of conveying information

Severity: Serious

Fix: You can either add data labels or direct labels to each bubble group, or use different marker shapes alongside the color coding.

---

**Finding 2** — Pie chart uses color as the only differentiator

The "This Year Sales by Chain" donut chart distinguishes Fashions Direct from Lindseys using teal and dark grey. Some users may not distinguish these reliably. Percentage labels are present but in order to distingush Fashions Direct from Lindseys, we need to rely on color matching alone.

Checklist reference: Section 1 — Color and Contrast
Color shouldn't be the only means of conveying information

Severity: Moderate

Fix: Add direct labels inside or adjacent to each segment showing the chain name, removing the need to match differentiating colors to segments.

---

**Finding 3** — No visible titles on two visuals

The card showing $22M and the card showing Last Year Sales and New Stores have no visible chart title — only the data values. A screen reader user that relies on titles to navigate would have no context for what these numbers represent.

Checklist reference: Section 4 — Titles and Labels
Every visual has a clear, descriptive title that makes sense without context

Severity: Serious

Fix: Add descriptive titles to all card visuals — for example "Total This Year Sales" and "Year-Over-Year Comparison."

---

## Page 2 — District Monthly Sales

**Finding 4** — Line chart uses color and shape together — partial pass

The chart "Last Year Sales, This Year Sales and Total Sales Variance % by FiscalMonth" uses bars to distingush these. However, they rely on color matching. The bars are grey and teal with no direct labels.

Checklist reference: Section 1 — Color and Contrast / Section 5 — Markers

Severity: Moderate

Fix: Add direct data labels to the line series so users do not need to match them by color. Consider adding markers to the line for additional differentiation.

---

**Finding 5** — Bubble chart category labels are small and may overlap

The scatter chart "Total Sales Variance %, Avg $/Unit TY and This Year Sales by Category" has category labels directly located on the bubbles — some overlap or are positioned inconsistently. A low-vision user may struggle to read the smaller labels.

Checklist reference: Section 4 — Titles and Labels
Data labels are positioned to avoid overlap

Severity: Minor

Fix: Increase label font size and review positioning to ensure no two labels overlap. 

---

**Finding 6** — Bar chart store names are cut off 

The "TotalSales by Chain and Name" bar chart on the right cuts off most store names with ellipsis — for example "Fashions Direct Charleston Fash..." A screen reader may announce the full name from alt text or the data table, but a sighted low-vision user zooming in cannot read the full names.

Checklist reference: Section 4 — Titles and Labels
Axis labels are readable and clearly described

Severity: Minor

Fix: Widen the visual or reduce font size to allow full store names to display, or add tooltips with the full name visible on hover and ensure the Show Data table contains the full text.

---

## Page 3 — New Stores

**Finding 7** — Red and green used together on the variance chart

The "Total Sales Variance % by FiscalMonth" waterfall-style bar chart uses green for positive variance and red for negative variance. This is the most common color combination in data visualization — and the most problematic for colorblind users. 

Severity: Critical

Fix: Replace red with a blue or orange series for negative variance, or add text labels showing + and — directly on each bar so the sign is conveyed through text, not color alone. 

**Finding 8** — Percentage labels on the variance chart are very small

The percentage labels on the variance bars — -10%, 32%, -25%, etc. — are small relative to the chart area. At standard screen resolution a low-vision user would struggle to read them without zooming.

Checklist reference: Section 4 — Titles and Labels / Section 15 — General Design

Reviewed with a low-vision test

Severity: Minor

Fix: Increase data label font size on the variance chart. Test at 150% and 200% zoom to confirm readability.

---

### Summary of Findings

| Finding | Page | Checklist Section | Severity |
|---|---|---|---|
| Red and green color coding on variance chart | New Stores | Section 1 — Color and Contrast | Critical |
| Missing titles on card visuals | Store Sales Overview | Section 4 — Titles and Labels | Serious |
| Color-only differentiation on bubble chart | Store Sales Overview | Section 1 — Color and Contrast | Serious |
| Color-only legend on donut chart | Store Sales Overview | Section 1 — Color and Contrast | Moderate |
| Color-only legend on combo chart | District Monthly Sales | Section 1 — Color and Contrast / Section 5 — Markers | Moderate |
| Overlapping bubble chart labels | District Monthly Sales | Section 4 — Titles and Labels | Minor |
| Truncated bar chart store names | District Monthly Sales | Section 4 — Titles and Labels | Minor |
| Small percentage labels on variance chart | New Stores | Section 4 — Titles and Labels / Section 15 — General Design | Minor |

---

### Priority Order for Fixes

1. Red and green on the variance chart — Critical. It affects colorblind users. This can be fixed by replacing with blue or orange for negative values, or add +/— text labels.
2. Missing card titles — Serious. A screen reader user cannot understand what $22M refers to without a title.
3. Color-only bubble and donut differentiation — Serious. Both affect the Store Sales Overview page and can be addressed together.
4. Combo chart legend — Moderate. Add direct labels to the line series.
5. Label size and truncation — Minor. Schedule for a visual polish pass across all three pages.

---

### What the Checklist Caught

All eight findings map directly to sections in the Accessible Report Design Checklist. The most significant finding — Finding 7, the red and green variance chart — is specifically called out in Section 1 as a color combination to avoid. The checklist worked exactly as intended.

#### What passed:

Navigation structure — three clearly labeled pages with descriptive names
The combo chart on District Monthly Sales uses both a line and bars to distinguish series — a good accessibility practice
Data tables are present on the New Stores page providing an alternative way to read the numbers
