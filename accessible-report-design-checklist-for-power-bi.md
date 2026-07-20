# Accessible Report Design Checklist for Power BI

**Author:** Florencia Cruz

**Date:** July 2026

---

## Why This Checklist Matters

Approximately 15% of the global population lives with some form of disability. This means that in any organization that is large enough to use Power BI, a meaningful percentage of people are affected. When reports created with Power BI are not accessible, some people simply cannot use them.

A blind employee using a screen reader cannot read a chart with no alt text. A colorblind manager cannot tell the difference between a red and green status indicator if color is the only signal. A user with a motor disability who navigates by keyboard cannot interact with a visual that was never tested without a mouse.

An organization that publishes inaccessible reports is signaling — whether intentionally or not — that some users do not matter. 

The checklist ensures that before a report is published, every person who needs to read it can actually read it.

---

### Section 1 — Color and Contrast


- [ ] Text and background color contrast ratio is at least 4.5:1
for all visual titles, axis labels, and data labels
(WCAG 2.1 Success Criterion 1.4.3)
- [ ] Text and background contrast in all textboxes meets the
4.5:1 minimum ratio
- [ ] Color is not the only means of conveying information —
text, icons, or patterns supplement or replace color coding
- [ ] The following color combinations are avoided together in
charts or on the same page:- Green and red - Green and brown - Blue and purple - Green and blue - Light green and yellow - Blue and grey - Green and grey - Green and black
- [ ] Report has been tested with a color blindness simulator
such as Coblis or Vischeck
- [ ] Color contrast has been verified with a tool such as Color Contrast Analyzer, WebAIM, or Accessible Colors
- [ ] A Power BI accessibility-friendly built-in theme has been
applied or the custom theme has been checked for contrast

---

### Section 2 — Alt Text


- [ ] Alt text has been added to every non-decorative visual
on every report page
- [ ] Alt text describes the insight or purpose of the visual —
not just what type of chart it is (the screen reader already
announces the visual type and title)
- [ ] Alt text for each visual is under 250 characters
 Alt text has been added to all non-decorative images
and shapes that convey information
- [ ] Decorative images and shapes have been excluded from
alt text (leave alt text blank for purely decorative elements)
- [ ] All textboxes have their content added to the alt text
field so screen readers can access them
- [ ] Where data is dynamic, conditional formatting for alt text
has been considered using DAX measures

---

### Section 3 — Tab Order


- [ ] Tab order has been set in the Selection pane (View →
Show panes → Selection → Tab order)
- [ ] Tab order follows the logical visual flow of the report —
matching the order a sighted reader would process the visuals
- [ ] All decorative shapes and images are hidden from the
tab order so screen readers do not announce them
- [ ] Tab order has been tested using keyboard navigation only
(Tab key) to confirm the experience is logical

---

### Section 4 — Titles and Labels


- [ ] Every visual has a clear, descriptive title that makes
sense without context
- [ ] Titles avoid acronyms and jargon — or spell them out
on first use
- [ ] Axis labels are readable and clearly described
- [ ] Data labels are positioned to avoid overlap —
above or below the series as appropriate
- [ ] Legend values are easy to read and understand
- [ ] The same font size is used consistently for all visual
titles across the report
- [ ] The same font size is used consistently for all data
labels and axis titles across the report
- [ ] Font color and style are consistent across all visual
elements throughout the report

---

### Section 5 — Markers


- [ ] For Line, Area, Combo, Scatter, and Bubble visuals,
markers are enabled (Visualizations pane → Format →
Shapes → Show Markers → On)
- [ ] Each series uses a different marker shape — not just
a different color
- [ ] Marker shape, color, and size are customized per series
using Customize Series
- [ ] If both data labels and markers are enabled, the visual
has been reviewed to ensure it is not cluttered or
distracting — consider turning off data labels if markers
are sufficient

---

### Section 6 — Slicers


- [ ] All slicers use consistent design across report pages —
same font, colors, and spatial position
- [ ] Slicer placement is the same on every page where the
slicer appears

---

### Section 7 — Keyboard Navigation


- [ ] The entire report can be navigated using keyboard only
(Tab, arrow keys, Enter, Escape)
- [ ] All visuals support keyboard navigation — this is built
into Power BI and does not require configuration
- [ ] Bookmarks used for navigation have been tested with
keyboard-only navigation
- [ ] Key information is not only accessible through hover
or interaction — pre-filter or rearrange visuals so
important conclusions are visible without requiring
additional steps

---

### Section 8 — Screen Reader Compatibility


- [ ] Screen reader has been tested on the report — open the
screen reader before opening Power BI Desktop for
best results
- [ ] Scan mode or browse mode has been turned off when
using a screen reader with Power BI
- [ ] Visual titles, visual types, and alt text are announced
correctly when navigating by keyboard
- [ ] The accessible Show Data table (Alt + Shift + F11)
displays meaningful data for each visual

---

### Section 9 — Sort Order


- [ ] Sort order has been purposefully set for each visual
- [ ] The sort order makes sense in the accessible Show Data
table — the table reflects whatever sort order is set
on the visual

---

### Section 10 — Tooltips


- [ ] Important information is not conveyed through tooltips
only — users with motor disabilities and non-mouse
users cannot reliably access them
- [ ] Tooltips are used only for ancillary or supplemental
information
- [ ] Tooltip content is included in the Show Data table
for each visual

---

### Section 11 — Video and Audio


- [ ] Video does not autoplay when the page renders
- [ ] Video has captions or a transcript is provided
- [ ] Audio does not autoplay when the page renders
- [ ] A transcript is provided for any audio content

---

### Section 12 — Shapes and Images


- [ ] Decorative shapes are hidden in the tab order
- [ ] Decorative images are hidden in the tab order
- [ ] The number of decorative shapes and images is kept
to a minimum to avoid distraction
- [ ] Shapes used to call out data points have alt text
explaining what they are calling out
- [ ] Images used to call out data points have alt text
explaining what they are calling out

---

### Section 13 — Power BI Visuals


- [ ] The accessible Show Data table for each visual shows
sufficient information — if not, consider a different
visual type
- [ ] If the Play Axis custom visual is used, it does not
autoplay — it is clear that the user must press
play/pause to start or stop

---

### Section 14 — High Contrast


- [ ] Report has been viewed in high contrast mode to
confirm readability (Windows Settings → High contrast,
or Power BI service → View → High contrast colors)
- [ ] High contrast colors from Windows are automatically
detected and applied by Power BI Desktop — verify
this is working correctly before publishing

---

### Section 15 — General Design


- [ ] Report is as simple as possible — each visual
shows one clear thing
- [ ] The number of visuals on each page is kept to a
minimum to avoid cognitive overload and
performance issues
- [ ] The report has been reviewed with a low-vision test
— lower screen brightness or use a browser squint
test extension to simulate low vision
- [ ] The report has been shown to a real user for feedback
before publishing

---

#### Sources


- [Overview of Accessibility in Power BI — Microsoft Learn](https://learn.microsoft.com/en-us/power-bi/create-reports/desktop-accessibility-overview)
- [Design Power BI Reports for Accessibility — Microsoft Learn](https://learn.microsoft.com/en-us/power-bi/create-reports/desktop-accessibility-creating-reports)
- [WCAG 2.1 Quick Reference — W3C](https://www.w3.org/WAI/WCAG21/quickref/)


---

*Built as part of the 8-Week Accessibility and UX Writing Learning Path
Florencia Cruz | July 2026*
