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

The "This Year Sales by Chain" donut chart distinguishes Fashions Direct from Lindseys using teal and dark grey. Some users may not distinguish these reliably. Percentage labels are present but in order to distinguish Fashions Direct from Lindseys, we need to rely on color matching alone.

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

**Finding 4** — Combo chart relies on color matching with no direct labels 

The chart "Last Year Sales, This Year Sales and Total Sales 
Variance % by FiscalMonth" uses bars and a line to present 
multiple series. However, the legend relies on color 
matching alone — the bars are grey and teal with no direct 
labels on the series, and no markers on the line to 
differentiate it visually from the bars.

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

**Checklist reference:** Section 1 — Color and Contrast
*The following color combinations are avoided together in 
charts or on the same page: Green and red*

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
| Combo chart relies on color matching with no direct labels | District Monthly Sales | Section 1 — Color and Contrast / Section 5 — Markers | Moderate |
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

--- 

# Live Accessibility Audit — Store Sales Power BI Report

**Auditor:** Florencia Cruz

**Date:** July 2026

**Tool:** Accessible Report Design Checklist (self-authored)

**Pages evaluated:** Store Sales Overview, District Monthly Sales, New Stores

---
## Page 1 — Store Sales Overview

**Finding 1** — Bubble chart supports non-color identification through interactive filtering

The bottom-right scatter/bubble chart uses teal and grey 
bubbles to distinguish New Store from Same Store. While 
color is the primary visual signal at rest, the chart 
supports interactive filtering — clicking a label in the 
legend isolates the corresponding bubbles and removes the 
others from view, allowing a user to identify each series 
without relying on color differentiation alone.

**Checklist reference:** Section 1 — Color and Contrast
*Color is not the only means of conveying information*

**Result:** Pass — with note

The interactive behavior provides a non-color path to 
identifying each series. This is a meaningful accessibility 
consideration because it means a colorblind user who 
cannot distinguish teal from grey can still isolate each 
group by clicking its label and reading the results 
independently.

**Note for future improvement:** The chart relies on the 
user knowing that the labels are clickable. Consider 
adding a brief instruction or tooltip — for example 
"Click a label to filter by store type" — so the 
interactive behavior is discoverable without trial and 
error.

---

**Finding 2** — Donut chart supports non-color identification through interactive filtering

The "This Year Sales by Chain" donut chart distinguishes 
Fashions Direct from Lindseys using teal and dark grey. 
While color is the primary visual signal at rest, the 
chart supports interactive filtering — clicking either 
segment isolates that chain's results across the report, 
allowing a user to identify each series without relying 
on color matching alone.

**Checklist reference:** Section 1 — Color and Contrast
*Color is not the only means of conveying information*

**Result:** Pass — with note

The interactive behavior provides a non-color path to 
identifying each chain. A colorblind user who cannot 
distinguish teal from dark grey can still isolate 
Fashions Direct or Lindseys by clicking each segment 
and reading the filtered results independently.

**Note for future improvement:** The chart still relies 
on the user knowing that the segments are clickable. 
The percentage labels present at rest do not include 
the chain name — a user navigating by screen reader 
or relying on the static view alone would still need 
color to distinguish the two segments. Consider adding 
direct labels showing the chain name inside or adjacent 
to each segment so the identity of each slice is 
visible without requiring an interaction.

---

**Finding 3** — No visible titles on two visuals

The card showing $22M and the card showing Last Year Sales and New Stores have no visible chart title — only the data values. A screen reader user that relies on titles to navigate would have no context for what these numbers represent.

Checklist reference: Section 4 — Titles and Labels
Every visual has a clear, descriptive title that makes sense without context

Severity: Serious

Fix: Add descriptive titles to all card visuals — for example "Total This Year Sales" and "Year-Over-Year Comparison."

---

## Page 2 — District Monthly Sales

**Finding 4** — Combo chart offers interactive filtering but results remain color-dependent

The chart "Last Year Sales, This Year Sales and Total 
Sales Variance % by FiscalMonth" uses bars and a line 
to present multiple series. Clicking the legend titles 
does filter the chart to show results for each series 
individually — which provides a partial non-color path 
to identification.

However, the filtered results themselves still rely on 
color to convey meaning. When a series is isolated 
through clicking, the bars and line retain their teal 
and grey color coding with no direct labels, markers, 
or text indicators to distinguish them independently 
of color. A colorblind user who clicks through each 
legend title still cannot reliably interpret which 
series they are viewing without color vision.

**Checklist reference:** Section 1 — Color and Contrast /
Section 5 — Markers
*Color is not the only means of conveying information —
each series uses a different marker shape*

**Result:** Partial pass — fails on color dependency 
within filtered results

**Severity:** Moderate

**Fix:** Add direct data labels to each series so the 
name of the series appears on the visual itself — not 
just in the legend. Add markers to the line to 
differentiate it from the bars through shape as well 
as color. These two changes would make the chart 
readable without color vision regardless of whether 
the user interacts with the legend or not.

---

**Finding 5** — Bubble chart category labels are small and may overlap

The scatter chart "Total Sales Variance %, Avg $/Unit TY and This Year Sales by Category" has category labels directly located on the bubbles — some overlap or are positioned inconsistently. A low-vision user may struggle to read the smaller labels.

Checklist reference: Section 4 — Titles and Labels
Data labels are positioned to avoid overlap

Severity: Minor

Fix: Increase label font size and review positioning to ensure no two labels overlap. 

---

**Finding 6** — Bar chart store names are cut off at rest — full names available on click but with usability limitations

The "TotalSales by Chain and Name" bar chart truncates 
most store names with ellipsis at rest — for example 
"Fashions Direct Charleston Fash..." A sighted low-vision 
user zooming in cannot read the full names from the 
static view alone.

In the live version of the report, clicking on a 
truncated bar label does reveal the full store name — 
which is a meaningful improvement over a purely static 
report. The interaction provides access to information 
that was previously unavailable without modifying the 
visual itself.

However, this solution has two practical limitations 
that prevent it from fully resolving the finding:

**1. The interaction is not discoverable.**
There is no visual indicator — no tooltip hint, no 
cursor change, no instruction — that tells the user 
clicking a label will reveal the full name. A user 
who does not already know this behavior exists will 
not find it. Discoverability is a core usability 
principle: if a feature requires prior knowledge to 
access, it does not function as an accessible solution 
for all users.

**2. The response time is slow.**
After clicking a label, the report takes several 
seconds to react and display the full name. For a 
user with a motor disability who finds repeated 
clicking effortful, or for any user expecting 
immediate feedback, a multi-second delay creates 
friction that reduces the practical usefulness of 
the interaction.

**Checklist reference:** Section 4 — Titles and Labels
*Axis labels are readable and clearly described*

**Result:** Partial pass — interaction resolves the 
information gap but introduces discoverability and 
performance barriers

**Severity:** Minor — unchanged

**Fix:** The click interaction is a useful fallback 
but should not be the primary solution. Widening 
the visual or reducing the label font size to allow 
full store names to display at rest remains the most 
reliable fix. If the truncated display must be 
preserved for layout reasons, add a visible tooltip 
on hover showing the full name — this is immediately 
discoverable and requires no click or wait time.

--- 

## Page 3 — New Stores

**Finding 7** — Red and green used together on the variance chart

The "Total Sales Variance % by FiscalMonth" waterfall-style bar chart uses green for positive variance and red for negative variance. This is the most common color combination in data visualization — and the most problematic for colorblind users. 

**Checklist reference:** Section 1 — Color and Contrast
*The following color combinations are avoided together in 
charts or on the same page: Green and red*

Severity: Critical

Fix: Replace red with a blue or orange series for negative variance, or add text labels showing + and — directly on each bar so the sign is conveyed through text, not color alone. 

---

**Finding 8** — Percentage labels on the variance chart are very small

The percentage labels on the variance bars — -10%, 32%, -25%, etc. — are small relative to the chart area. At standard screen resolution a low-vision user would struggle to read them without zooming.

Checklist reference: Section 4 — Titles and Labels / Section 15 — General Design

Reviewed with a low-vision test

Severity: Minor

Fix: Increase data label font size on the variance chart. Test at 150% and 200% zoom to confirm readability.

---

### Summary of Findings

| Finding | Page | Checklist Section | Result | Severity |
|---|---|---|---|---|
| Bubble chart supports non-color identification through interactive filtering | Store Sales Overview | Section 1 — Color and Contrast | Pass — with note | Serious → Resolved |
| Donut chart supports non-color identification through interactive filtering | Store Sales Overview | Section 1 — Color and Contrast | Pass — with note | Moderate → Resolved |
| No visible titles on two visuals | Store Sales Overview | Section 4 — Titles and Labels | Fail | Serious |
| Combo chart offers interactive filtering but results remain color-dependent | District Monthly Sales | Section 1 — Color and Contrast / Section 5 — Markers | Partial pass | Moderate |
| Bubble chart category labels are small and may overlap | District Monthly Sales | Section 4 — Titles and Labels | Fail | Minor |
| Bar chart store names cut off at rest — full names on click with usability limitations | District Monthly Sales | Section 4 — Titles and Labels | Partial pass | Minor |
| Red and green used together on the variance chart | New Stores | Section 1 — Color and Contrast | Fail | Critical |
| Percentage labels on the variance chart are very small | New Stores | Section 4 — Titles and Labels / Section 15 — General Design | Fail | Minor |

---

### Priority Order for Fixes

1. **Red and green on the variance chart** — Critical.
   The most urgent fix across both versions of the 
   audit. Interactive behavior does not resolve this 
   finding — the color combination remains problematic 
   regardless of user interaction. Replace red with 
   blue or orange for negative values, or add +/— 
   text labels directly on each bar.

2. **Missing card titles** — Serious. This finding 
   was not resolved by the live version. A screen 
   reader user still cannot understand what $22M 
   refers to without a descriptive title. Add 
   "Total This Year Sales" and "Year-Over-Year 
   Comparison" to the two untitled cards.

3. **Combo chart color dependency** — Moderate. 
   The interactive filtering helps but does not 
   resolve the issue — filtered results still rely 
   on color. Add direct series labels and markers 
   to the line so the chart is readable without 
   color vision at every state.

4. **Bar chart truncated names** — Minor. The click 
   interaction provides access to full names but 
   is not discoverable and is slow to respond. 
   Add a hover tooltip showing the full name as 
   the primary fix — immediate and requires no 
   prior knowledge.

5. **Bubble chart label overlap** — Minor. No 
   interactive behavior resolves this finding. 
   Increase label font size and review positioning 
   across the scatter chart on District Monthly 
   Sales.

6. **Small percentage labels on variance chart** — 
   Minor. Increase data label font size and test 
   at 150% and 200% zoom.

---

### What the Checklist Caught

Six of the eight findings from the static audit 
remain active in the live version — confirming that 
interactive behavior alone is not a substitute for 
accessible design at rest.

The two most significant updates from the live audit:

**Findings 1 and 2 moved from Fail to Pass** — the 
bubble chart and donut chart both support interactive 
filtering that provides a genuine non-color path to 
identifying each series. These were the only two 
findings resolved by the live behavior.

**Finding 4 moved from Fail to Partial Pass** — 
the combo chart legend titles are clickable, but 
the filtered results remain color-dependent. The 
interaction helps but does not resolve the 
underlying issue.

**Finding 6 moved from Fail to Partial Pass** — 
clicking a truncated label reveals the full store 
name, but the interaction is not discoverable and 
is slow to respond. The information is technically 
available but not practically accessible for all 
users.

**Findings 3, 5, 7, and 8 remain unchanged** — 
no interactive behavior addresses these findings 
in the live version.

The most critical finding — Finding 7, the red and 
green variance chart — is unaffected by any 
interactive behavior and remains the highest 
priority fix across both versions of this audit.

---

#### What Passed

- **Navigation structure** — three clearly labeled 
  pages with descriptive names, unchanged from the 
  static version

- **Interactive filtering on the bubble chart** — 
  clicking a legend label isolates each store type, 
  providing a non-color identification path for 
  colorblind users

- **Interactive filtering on the donut chart** — 
  clicking a segment isolates each chain's results 
  across the report, providing a non-color 
  identification path for colorblind users

- **Combo chart visual type** — using both bars and 
  a line to distinguish series is good accessibility 
  practice, even though the color dependency within 
  the legend remains unresolved

- **Data tables on the New Stores page** — provide 
  an alternative way to read numerical data for 
  users who cannot interpret the charts visually

- **Partial interactive access to truncated store 
  names** — clicking labels reveals full names, 
  which is a meaningful improvement over a purely 
  static report, even with the discoverability and 
  performance limitations noted

---

*Live Accessibility Audit — Store Sales Power BI Report*
*Florencia Cruz | July 2026*
