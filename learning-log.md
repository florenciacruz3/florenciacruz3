# Accessibility Learning Log
## Florencia Cruz — Technical Writer in Training

In this log, I'll be documenting my learning journey through accessibility as part of my technical writing training under the mentorship of a Microsoft MVP in Data and AI Platforms.

---

## Week 1 — What Accessibility Means and Why It Matters

**Date:** July 9, 2026
**Resources completed:**
- Microsoft Learn — Accessibility Fundamentals (Module 1: 
  Introduction to Disability and Accessibility)
- W3Cx — Introduction to Web Accessibility (Module 1)

---

### What I Learned

Something that I didn't know before completing this training that had an impact on me is that disabilities come from what the environment enables us. 
For instance, if everyone spoke in sign language, people who don't speak in sign language wouldn't be able to understand. 
Accessibility means designing products, services, and environments so that everyone can use them. 

A lot of people have the misconception that disability means permanent. However, the W3C describes three 
types:

- **Permanent** — such as being born without a limb or 
  losing sight permanently
- **Temporary** — such as a broken arm or an eye infection
- **Situational** — such as holding a baby with one arm, 
  or trying to read a screen in bright sunlight

That distinction changed how I think about accessibility. 
When I design or write content accessibly, I am not writing 
for a small minority of users. I am writing for anyone who 
might encounter a barrier — which, depending on the 
circumstance, is almost everyone at some point.

Instead of thinking of disability as a problem with the person, I like to think that disability is a mismatch between the 
person and the environment. And the way their environment is designed is what disables 
people — not the person themselves. That reframing made 
everything click for me.

---

### Why It Matters for Technical Writing Specifically

Documentation that is not accessible excludes readers who 
use screen readers, who navigate by keyboard, who rely on 
high contrast settings, or who need captions to follow 
along with video content.

As a technical writer, my job has always been to make 
information accessible to the reader — to reduce the 
distance between where they are and where they need to be. 
Accessibility gives that goal a technical standard and a 
legal framework. It is not just good practice. In many 
contexts it is a legal requirement — under laws like the 
Americans with Disabilities Act in the United States and 
the European Accessibility Act across the EU.

I also learned this week that accessibility benefits far 
more people than those with permanent disabilities. 
Accessible content helps older users whose abilities are 
changing, people using mobile devices in difficult 
conditions, people with slow internet connections, and 
people who are in environments where they cannot use 
audio. The overlap between "accessible content" and 
"well-written content" is not a coincidence — they are 
the same thing.

---

### What I Applied

**Accessibility Checker — Tenant Scan Article**

I used Claude as a tool for figuring out how to run an accessibility check on my writing, which took me through different steps:

1. Open your article on GitHub in Chrome
2. Right-click anywhere on the page and select Inspect
3. Click the Lighthouse tab at the top of the DevTools panel
4. Under Categories select Accessibility
5. Click Analyze page load
6. Chrome generates a full accessibility report with a score and specific issues

Before I ran my accessibility check, I couldn't help wondering what issues there could be in my writing. And then I realized that the main issue I found was 
a missing H1 heading. The article title was written as 
plain bold text rather than a proper Markdown heading, 
which meant screen readers had no document title to 
announce.

**What I fixed:**

| Issue | Before | After |
|---|---|---|
| Document title | Plain bold text | `# The Hidden Risks...` as H1 |
| Heading hierarchy | Started at H2 with no H1 | H1 → H2 → H3 throughout |
| FAQ questions | Listed as H3 under H2 FAQ | Confirmed correct — H3 under H2 |

The heading hierarchy now follows a logical sequence — 
one H1 at the top, H2 for major sections, H3 for 
subsections — which means a screen reader user can 
navigate the document by heading the same way a sighted 
reader scans visually.

---

### In My Own Words

I was very interested to hear on my first module about the different levels of success that people with disabilities have been able to accomplish trough accessibility. 
Making the decision of adding accessibility to your writing can have a bigger impact than you could imagine. 

I thought that the level of detail on what accessibility means was very impactful to me. People generally have certain levels of learning within their senses, listening, visually, kinesthetic learners. 
I myself have had to deal with ADHD as I was going to school, and I learned that my best skills are visual and kinesthetic learning, so I was able to play that to my favor as I was going to school, and managed to graduate with honors for a bachelor's degree. 
And I'm sure people use this on day to day basis, people who have a better time listening and like to multitask by listening to an audio book. Or people who have a hard time reading, so they use AI for summaries. 

Learning about accessibility give me a broad idea of how the writing world works, and how impactful our decisions as writers can be. 

---

## Resources

- [Microsoft Learn — Accessibility Fundamentals](https://learn.microsoft.com/en-us/training/paths/accessibility-fundamental/)
- [W3Cx — Introduction to Web Accessibility (edX)](https://www.edx.org/learn/web-accessibility/the-world-wide-web-consortium-w3-introduction-to-web-accessibility)
- [Tenant Scan Article](https://github.com/florenciacruz3/florenciacruz3/blob/main/getting-started-with-tenant-scan.md)

---

## Week 1 — Entry 2: POUR Explained with Examples from a Real Document

**Date:** July 10, 2026
**Resources completed:**
- W3Cx — Introduction to Web Accessibility: POUR principles
- Applied to: Tenant Scan article — getting-started-with-tenant-scan.md

---

### What I Learned

POUR is the framework that constitutes the Web Content 
Accessibility Guidelines (WCAG). It stands for four 
principles that every piece of digital media should follow:

- **Perceivable** — users must be able to perceive the 
  content through at least one of their senses
- **Operable** — users must be able to navigate and 
  interact with the content
- **Understandable** — users must be able to understand 
  both the content and how the interface works
- **Robust** — content must work reliably across different 
  browsers, devices, and assistive technologies

Some people see this as a checklist. I see it as a question that I ask myself when starting a new project: can every user perceive, 
operate, understand, and access this content regardless 
of how they are accessing it?

---

### POUR Applied to My Tenant Scan Article

Working through my Tenant Scan article this week gave me 
a whole new perspective on what accessibility means. There are just so many details that we tend to ignore. That's why I think that learning about accessibility is essential even to the day-to-day person. 

---

#### Perceivable

The important thing to note is that we need to consider everyone's way they can 
perceive — which means it cannot rely on a single sense 
such as sight alone.

**What I found in my article:**

The table in Section 6 — Assessment Tiers — had no 
caption. A screen reader user navigating to that table 
would hear the column headers and cell content read 
aloud, but would have no context for what the table 
was about before entering it.
It would't allow me to add an alt text, so I added a caption. 

---

#### Operable

Users must be able to navigate and interact with content 
using different input methods — not just a mouse.

**What I found in my article:**

My table of content contained links that would lead to each section. They are blue, which I checked and it's fine from a WCAG perspective.
However the list had no label explaining that the items were 
navigation links — a screen reader user landing on the 
list would hear a list of blue underlined items with 
no indication they were clickable destinations.
So, I added a note next to the title, indicating what this colored words mean. 

I also found that arrow characters throughout the article 
— `→` — were being used to show sequences and directions. 
These are read aloud by screen readers as "right-pointing 
arrow" every time they appear, which disrupts the reading 
experience for keyboard and screen reader users.
I replaced every arrow with a comma instead. 

---

#### Understandable

Content must be written and structured so that users can 
understand it — including the language, the structure, 
and any instructions.

**What I found in my article:**

Several abbreviations appeared without being spelled out 
on first use. A screen reader user — or any reader 
unfamiliar with the industry — would encounter:
To fix this mistake, I spelled out every abbreviation on first use:

```

I also found that "Now / Next / Later" used slash 
characters which screen readers read as "Now slash Next 
slash Later." I changed every instance to a comma. 

---

#### Robust

Content must be robust enough to work reliably across 
different browsers, devices, and assistive technologies 
— both current and future.

**What I found in my article:**

I ensured that my heading hierarchy follows a strict 
H1 → H2 → H3 sequence with no skipped levels, which 
ensures the document structure is interpretable by any 
screen reader or browser regardless of how the Markdown 
is rendered.

---

### In My Own Words

Changing my persepctive from completing a checklist and asking a set of questions changed how a I felt about entering a new filed of accessibillity. 

At different work positions that I've had before, knowing why we do things in a certain way has always made everything click. 

And POUR did that for me

The arrow characters were an operability 
problem. The unexplained abbreviations were an 
understandability problem. The missing table caption 
was a perceivability problem. The GitHub-specific 
callout syntax was a robustness consideration.

I am starting to see accessibility not as something 
separate from good writing — but as the same thing 
with a more rigorous standard.

---

## Resources

- [W3Cx — Introduction to Web Accessibility (edX)](https://www.edx.org/learn/web-accessibility/the-world-wide-web-consortium-w3-introduction-to-web-accessibility)
- [WCAG — Understanding POUR](https://www.w3.org/WAI/WCAG21/Understanding/)
- [Tenant Scan Article](https://github.com/florenciacruz3/florenciacruz3/blob/main/getting-started-with-tenant-scan.md)

---

*Last updated: July 2026*
