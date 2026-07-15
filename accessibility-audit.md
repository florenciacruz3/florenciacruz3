# Mini Accessibility Audit
## Website: Half Price Books (hpb.com)
**Auditor:** Florencia Cruz

**Date:** July 2026

**Tools Used:** WAVE browser extension, Chrome DevTools Lighthouse, keyboard navigation testing

---

## Overview
Half Price Books is a bookstore, famous for selling used books at half price. Their website provides not only books, but movies and TV, music, collectibles, textbooks, games, and audiobooks. This audit evaluates a selection of pages against WCAG 2.2 Level AA success criteria using automated tools and manual testing.

**Pages evaluated:**
- Homepage (hpb.com)
- Books page
- Music page

---

## Findings

### 1. Links do not have a discernible name

- **Where:** Site-wide footer (Instagram, Facebook, YouTube icons)

- **Issue:** The Instagram, Facebook, and YouTube footer icons render as empty links — no alt text on the icon image and no aria-label on the link itself. A sighted mouse user recognizes the icon shape, but a screen reader announces only "link" with no name, so there's no way to know where it goes.

- **WCAG reference:** 1.1.1 Non-text Content (A), 4.1.2 Name, Role, Value (A)

- **Severity:** Critical

- **Fix:** Add aria-label="Half Price Books on Instagram" (and equivalents) to each icon link, or visually-hidden text inside the link.

### 2. Image elements have [alt] attributes that are redundant text

- **Where:** Site-wide — flagged by Lighthouse across the Books and Music product grids

- **Issue:** Several <a> elements have no discernible accessible name — no visible text, no aria-label, and no meaningful alt text on a wrapped image. Lighthouse also flagged image alt attributes that duplicate the adjacent link text (redundant alt text), which creates noise for screen reader users rather than adding information. In practice this overlaps with the wishlist icon and product-thumbnail links already noted above: a link wrapping only an icon or image with no text, and an unlabeled/duplicated alt, both leave the link's destination or purpose unclear when read out of context.

- **WCAG reference:** 4.1.2 Name, Role, Value (A), 2.4.4 Link Purpose (In Context) (A)

- **Severity:** Serious

- **Fix:** Every link needs a discernible name — either visible text inside the link, an aria-label on the <a>, or meaningful alt text on a wrapped image (not alt="", unless the image is truly decorative and the link already has a text name elsewhere).
Where an image and adjacent text link to the same destination, don't duplicate the text in alt — mark the image alt="" and let the adjacent text carry the accessible name, so screen readers announce it once instead of twice.

### 3. Touch targets do not have sufficient size or spacing

- **Where:** Site-wide — flagged by Lighthouse on the search icon/field and product tile links (button.fa.fa-search, input.form-control.search-field, a.link, a.author-name)

- **Issue:** Several interactive controls are too small and/or packed too closely together to reliably tap on a touchscreen — including the search icon button, the search input, and the product title/author links on the Books and Music grids. This is a problem for anyone with limited fine motor control, tremor, or larger fingers, and it also causes accidental mis-taps for the general population on mobile.

- **WCAG reference:** 2.5.8 Target Size (Minimum) (AA) — targets should be at least 24×24 CSS pixels, or have enough spacing to prevent adjacent-target overlap when smaller

- **Severity:** Moderate

- **Fix:** Increase the tappable area of the search icon and field (padding counts, not just the visible icon/text), and add spacing between the stacked author-name and link elements on product tiles so adjacent targets — e.g., title link and author link, sitting close together — don't compete for the same tap.

### 4. Heading elements are not in a sequentially-descending order

- **Where:** Books and Music product grids — h5.book-cover-head.font-weight-bold (used for product titles on category/listing pages)

- **Issue:** Product titles are marked up as `<h5>` elements, but the page's surrounding heading structure jumps to that level without passing through `<h2>`, `<h3>`, and `<h4>` in order (e.g., a section like "Rock/Pop" may be an `<h3>` immediately followed by `<h5>` product titles). Screen reader users frequently navigate by jumping heading-to-heading to build a mental map of the page; a skipped level suggests a nested subsection exists when it doesn't, making the page's structure harder to predict and scan.

- **WCAG reference:** 1.3.1 Info and Relationships (A) — heading order is called out explicitly as a best practice under this criterion

- **Severity:** Minor

- **Fix:** Adjust the heading levels so they descend one step at a time (e.g., page title → h1, category section → h2, product title → h3), reserving visual size/weight styling (font-weight-bold, etc.) for CSS rather than for choosing which heading tag to use.

---

## Summary

| Severity | Count |
|----------|-------|
| Critical | 1     |
| Serious  | 1     |
| Moderate | 1     |
| Minor    | 1     |

**Suggested priority:** Start with the footer social icons (Finding 1) — it's a small, contained fix,and the footer appears on every page. From there, the redundant/missing link names on product tiles (Finding 2) are worth tackling next, since they touch the shared product-tile template and affect every listing page across Books, Music, and likely Movies & TV and Collectibles as well. Touch target spacing and heading order are lower urgency but still worth scheduling, since both compound the experience for the same groups of users already affected by Findings 1 and 2.

---

## Closing Thoughts

These are some of the typical issues that tend to show up on almost any large catalog and don't require a redesign to fix. These four findings have one thing in common — they live in shared templates, the footer, the product tile, the search bar. This means that a fix in one place propagates across the whole site. These findings are not a one-off typo, it's a pattern repeated on every page that reuses that component.

The important thing to take from this is: accessibility gaps here are rarely about whether someone can shop for a book online — they're about a mismatch between how the interface was built and how different people actually navigate it, whether that's by touch, by keyboard, or by screen reader. Closing that mismatch wouldn't just clear WCAG checkboxes; it would make search, browsing, and checkout more predictable for every HPB customer, disabled or not.








I recently completed WAI0.1x: Introduction to Web Accessibility, offered by the W3C Web Accessibility Initiative — and I wanted to share a few reflections on what I learned.



I went in thinking accessibility was a checklist. I came out realizing it's a whole new way of seeing design.



That distinction changed how I think about accessibility. When I design or write content accessibly, I am not writing for a small minority of users. I am writing for anyone who might encounter a barrier — which, depending on the circumstance, is almost everyone at some point.



Instead of thinking of disability as a problem with the person, I like to think that disability is a mismatch between the person and the environment. And the way their environment is designed is what disables people — not the person themselves. That reframing made everything click for me.



I was very interested to hear on my first module about the different levels of success that people with disabilities have been able to accomplish trough accessibility. Making the decision of adding accessibility to your writing can have a bigger impact than you could imagine.



I thought that the level of detail on what accessibility means was very impactful to me. People generally have certain levels of learning within their senses, listening, visually, kinesthetic learners. I myself have had to deal with ADHD as I was going to school, and I learned that my best skills are visual and kinesthetic learning, so I was able to play that to my favor as I was going to school, and managed to graduate with honors for a bachelor's degree. And I'm sure people use this on day to day basis, people who have a better time listening and like to multitask by listening to an audio book. Or people who have a hard time reading, so they use AI for summaries.



Learning about accessibility give me a broad idea of how the writing world works, and how impactful our decisions as writers can be.



This course was a strong foundation, and I'm looking forward to applying what I learned — and continuing to build on it — in my day-to-day work.



If you're working in product, design, or engineering and haven't looked into accessibility yet, I'd genuinely recommend starting here. It changes how you think about building for people.



#WebAccessibility #A11y #ContinuousLearning #InclusiveDesign #WCAG
