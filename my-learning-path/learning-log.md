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

I was very interested to hear on my first module about the different levels of success that people with disabilities have been able to accomplish through accessibility.

Making the decision of adding accessibility to your writing can have a bigger impact than you could imagine.

I thought that the level of detail on what accessibility means was very impactful to me. People generally have certain levels of learning within their senses, listening, visually, kinesthetic learners.

I myself have had to deal with ADHD as I was going to school, and I learned that my best skills are visual and kinesthetic learning, so I was able to play that to my favor as I was going to school, and managed to graduate with honors for a bachelor's degree.
And I'm sure people use this on a day-to-day basis, people who have a better time listening and like to multitask by listening to an audiobook. Or people who have a hard time reading, so they use AI for summaries.

Learning about accessibility gave me a broad idea of how the writing world works, and how impactful our decisions as writers can be.

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
— → — were being used to show sequences and directions. 
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

Several abbreviations appeared without being spelled out on first use. A screen reader user — or any reader unfamiliar with the industry — would encounter terms like these with no context for what they mean. To fix this, I spelled out every abbreviation on first use, giving the full term followed by the abbreviation in parentheses so both screen reader users and unfamiliar readers have the context they need.
I also found that "Now / Next / Later" used slash characters, which screen readers read aloud as "Now slash Next slash Later" — turning a simple heading into an awkward, confusing phrase. I changed every instance to a comma-separated list instead, so it reads naturally both visually and aloud.

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

Changing my perspective from completing a checklist and asking a set of questions changed how I felt about entering a new field of accessibility.

At different work positions that I've had before, knowing why we do things in a certain way has always made everything click.

And POUR did that for me.

The arrow characters were an operability problem. The unexplained abbreviations were an understandability problem. The missing table caption was a perceivability problem.

I am starting to see accessibility not as something separate from good writing — but as the same thing with a more rigorous standard.

---

## Resources

- [W3Cx — Introduction to Web Accessibility (edX)](https://www.edx.org/learn/web-accessibility/the-world-wide-web-consortium-w3-introduction-to-web-accessibility)
- [WCAG — Understanding POUR](https://www.w3.org/WAI/WCAG21/Understanding/)
- [Tenant Scan Article](https://github.com/florenciacruz3/florenciacruz3/blob/main/getting-started-with-tenant-scan.md)

---

## Week 2 — Entry 1: Plain Language and UX Writing

**Date:** July 17, 2026
**Resources completed:**
- UX Writing Hub — Free Course (uxwritinghub.com)
- Microsoft Writing Style Guide (learn.microsoft.com/style-guide)

---

### What I Learned

It was interesting to transition from Accessibility to UX Writing. It made me think about how accessibility is about making sure everyone can access your content. UX writing is about making sure that content is worth accessing in the first place.

I was also introduced to the idea of content-first design — the concept that you should start with 
words and build the design around them, not the other way 
around. That reframing was significant for me. I had always 
thought of writing as something that fills in a design. 
This course made me think of writing as the foundation the 
design is built on.

The Microsoft Writing Style Guide gave me a concrete set of 
principles to apply immediately. The ones that had the most 
impact on how I think about writing:

- **Use bigger ideas, fewer words** — shorter is always 
  better. If a word is not earning its place, cut it.
- **Write like you speak** — read your text aloud. If it 
  sounds stiff or formal, rewrite it until it sounds like 
  a conversation.
- **Get to the point fast** — lead with what matters most. 
  Do not make the reader wade through context before 
  arriving at the point.
- **Revise weak writing** — cut "there is," "you can," 
  and passive constructions. Start with verbs instead.
- **Use contractions** — "doesn't," "you'll," "it's." 
  They make language sound human.
- **Speak to the reader directly** — use "you" and "your" 
  instead of "organizations" and "companies."

---

### What I Applied

**Plain Language Rewrite — Tenant Scan Article**

I applied everything I learned this week to a hands-on 
activity: rewriting the introduction and executive summary 
of my Tenant Scan article into plain language, then 
documenting the before and after side by side as a 
portfolio piece.

The original opening read:

*"There is a moment every data leader fears. The Microsoft 
Fabric migration is approved, the timeline is set, and then 
the project fails."*

The rewritten version reads:

*"Most Fabric migrations fail for the same reason: the 
environment wasn't ready."*

That is the same idea in a fraction of the words. The 
original version builds to the point. The rewritten version 
leads with it — which is exactly what the Microsoft Style 
Guide means by "get to the point fast."

Other changes I made across the two sections:

- Replaced "organizations" and "companies" with "you" 
  and "your" throughout — speaking directly to the reader 
  instead of describing them from a distance
- Cut "there is" constructions and started sentences with 
  verbs instead
- Added contractions — "doesn't," "you'll," "it's" — to 
  make the language feel more natural
- Split long sentences into two shorter ones wherever a 
  single sentence was carrying two ideas
- Removed modifiers that added length without adding 
  meaning — "entire," "structured," "engagement"
- Replaced "a defined path to where they need to be" 
  with "what to do next" — plain language for the same idea

---

### In My Own Words

What stayed with me most from this week is how close plain 
language and accessibility actually are.

Last week I learned about how to remove the barriers that make content unaccessible to the reader. This week, I learned that without UX writing, content would still be unaccessible to the reader. They go hand in hand. 

I had already applied the concepts of accessiblity to my Tenant Scan article. But some of it was written to sound professional rather than 
to be useful. The rewrite did not change what the article 
says — it changed how easy it is to read. And that 
difference, I am learning, is the whole job.

---

## Resources

- [UX Writing Hub — Free Course](https://course.uxwritinghub.com/free_course)
- [Microsoft Writing Style Guide](https://learn.microsoft.com/en-us/style-guide/welcome/)
- [Microsoft Writing Style Guide — Top 10 Tips](https://learn.microsoft.com/en-us/style-guide/top-10-tips-style-voice)
- [Tenant Scan Article — Plain Language Rewrite](https://github.com/florenciacruz3/florenciacruz3/blob/main/getting-started-with-tenant-scan.md)

---

## Week 3 — Entry 1: Information Architecture Pass on the 
## Tenant Scan Article

**Date:** July 20, 2026
**Resources completed:**
- W3Cx — Introduction to Web Accessibility: Module 7 
  (Information Architecture)
- Applied to: Tenant Scan article — 
  getting-started-with-tenant-scan.md

---

### What I Learned

Information architecture made me switch my perspective on what accessibility really means. 

I used to think that accessibility meant writing for everyone. However, this exercise helped me see this differently. Accessibility means recognizing your audience, recognizing what they know, and organizing your writing according to that. 

That is a subtle but important distinction. Writing for 
everyone does not mean writing the same thing for everyone. 
It means writing in a way that works for each person 
differently — and information architecture is how you 
make that happen.

The exercise introduced me to a concept I had never thought 
about before: writing for two audiences at once. In the 
Tenant Scan article, those two audiences are a CTO — a 
Chief Technology Officer, the senior executive who approves 
the migration budget and owns the business risk — and a 
Fabric admin, the technical person who will actually run 
the scan and implement the findings.

The CTO wants to know what the problem is, how to solve it, what it costs, and how it is going to impact the business. The Fabric admin, on the other hand, wants to know how the scan works, what it examines, and what happens to their environment. Neither reader is interested in having to wade through the other's content to find their own. 

Information architecture is what makes it possible for both 
readers to get what they need from the same document.

---

### What I Applied

**Information Architecture Pass — Tenant Scan Article**

I restructured the Tenant Scan article from the reader's 
perspective rather than the writer's. The changes I made:

**1. Rewrote the section headings**

The original headings described the content from my 
perspective as the writer:

- What Microsoft Fabric Is and Why Your Tenant Matters
- Who It Is For
- What You Get
- Illustrative Scenarios
- Assessment Tiers
- Get Started

The new headings answer the question the reader is asking 
at each stage:

- The Problem — Why Fabric Migrations Fail
- Is This for You?
- What the Scan Produces
- What This Looks Like in Practice
- Choose Your Assessment Tier
- Get Started

**2. Added a reading guide**

The most significant change I made was adding a reading 
guide at the top of the article that directs each reader 
to the sections most relevant to them:

- CTO, VP of Data, or executive sponsor — Sections 
  1, 4, and 5. Section 3 if you want the deliverable 
  summary.
- Fabric admin, data engineer, or IT lead — Sections 
  3 and 5, then the FAQ for tenant access details.
- Evaluating for a client or stakeholder — Sections 
  1, 4, and 5 give you everything you need to present 
  the case internally.

I had never written for two audiences at the same time 
before. The reading guide was the tool that made it 
possible — instead of trying to serve both readers in 
every section, I let each reader skip what was not for 
them and go directly to what was.

**3. Added audience labels to each section**

I added a small label at the top of each section 
identifying who it is most relevant for.

**4. Reorganized the FAQ by reader**

I split the FAQ into two groups — one for executive and 
business readers and one for technical readers and admins. 
This way each reader can find their questions without 
scrolling past questions that do not apply to them.

---

### In My Own Words

Over the past few weeks I have learned about WCAG 
standards, assistive technologies, plain language, and 
UX writing. Each one felt like a separate skill. However, what I learned through this exercise is that IA is just another aspect of what accessibility means. For a text to be accessible, we need all components to work: 

- The content needs to be perceivable — screen readers, 
  alt text, contrast
- The content needs to be operable — keyboard navigation, 
  tab order, focus
- The content needs to be understandable — plain language, 
  clear headings, no jargon
- The content needs to be robust — consistent structure, 
  semantic markup
- And the content needs to be navigable — information 
  architecture, reading guides, audience awareness

A document can pass every WCAG checkpoint and still be hard to use if 
the information is organized in a way that does not 
match how the reader thinks.

Accessibility is not one thing. It is all of these 
things working together.

---

## Resources

- [Tenant Scan Article — IA Pass Version](https://github.com/florenciacruz3/florenciacruz3/blob/main/getting-started-with-tenant-scan.md)
- [W3Cx — Introduction to Web Accessibility](https://www.edx.org/learn/web-accessibility/the-world-wide-web-consortium-w3-introduction-to-web-accessibility)
- [Microsoft Writing Style Guide](https://learn.microsoft.com/en-us/style-guide/welcome/)

--- 

## Week 4 — Entry 1: Project Management Skills Deliverable 

**Date:** July 27, 2026
**Resources completed:**
- PMI KICKOFF Ceritificate
- Project Management Certificate - Course 1
- Applied to: PM Skills as a Content Creator — 
  PM-skills-as-a-content-creator.md

---

### What I Learned

Today I worked on developing a skill that I've been 
working on my whole life as a writer, which is 
learning how to write concisely and to the point.

After completing my two Week 1 certifications on 
Project Management (PM), I was assigned to write a 
one-page article on how the skills used in PM relate 
to content creation. But I was stuck on the — 1 page 
— part.

The skills that I used were recognizing which sections 
have earned their place in my article and which have 
not, which sentences are just redundant and need to be 
cut, and then there were the specifics, like **Do I 
want to include a "Next Steps" section, or do I just 
want a smaller "Sources" section?**

During this period of time, I also focused on how I 
can start using AI tools smartly, which is something 
that was briefly mentioned in the certifications I 
completed. So, I tried focusing on my writing itself 
before consulting Claude right away. I used Claude to 
help me brainstorm some ideas and selected what could 
be useful to add in this short space. I pasted my 
article several times, checking for writing clarity, 
good grammar, and syntax in order to help me polish 
my article in the last few steps. I also used it to 
ask its opinion on some of my thoughts, such as the 
length, what could be cut or reduced, and some of the 
formatting ideas I had in mind.

In regard to the content of my work, I thought that 
doing this exercise was interesting and helpful. I 
thought that briefly reflecting on what I've learned 
this week is a great way to absorb what I've been 
focusing all my time on.

---

### What I Applied

Some of the major changes I made were correcting 
grammar and checking for clarity, reorganizing my 
resource page — which used to be a Next Steps section 
— and managing the length of the piece, making sure 
that it fits the expectations.

- **Grammar mistakes:** They were mostly just typos 
  from quick, unrevised previous drafts.
- **Coherent sentences:** When editing, I found some 
  sentences that were cut off in the middle or read 
  awkwardly.
- **Resource page:** It was originally a Next Steps 
  page and contained descriptions for each one of the 
  websites. This was taking up too much space and made 
  it seem like I was putting too much emphasis on a 
  section that needed to be minimized. I changed it to 
  a Sources page containing only the two links I had 
  reviewed so far. I thought having only two source 
  links wouldn't be useful for the reader. So instead, 
  I brought back the original list, cut the 
  descriptions, and named it Resources.
- **Length:** I rewrote a lot of the sentences in the 
  skill descriptions to make them less redundant and 
  more to the point. I even deleted some sentences 
  completely. And as I mentioned, I reduced the 
  Resource page.

While making these changes, I made sure to commit to 
the expectations of the prompt. With so little space, 
the Next Steps section shouldn't be too long. Making 
sure there are no grammar mistakes or incoherent 
sentences is vital for the article to even be taken 
seriously. Last but not least, making sure the writing 
was concise and to the point was the most important 
aspect.

---

### In My Own Words

Learning about PM, as mentioned in my article, was a 
big step for me. I was in denial for a while, and 
taking the step to start my first certification was 
something new to me. This whole career change has been 
a big jump for me. I've always liked stability, being 
safe and cautious. Moving away from my technical 
writing field was scary but very much worth it.

Doing this activity was a great exercise in stepping 
outside my comfort zone.

And now I understand that PM makes perfect sense for 
me. Knowing how to practice time management, 
deliverable management, change management, and 
feedback delivery is what I've been preparing for my 
entire life.

While I was completing my two bachelor's degrees while 
working part time, PM was what got me to where I am 
now. PM was what was necessary to succeed.

---

## Resources

- [PMI KICKOFF](https://www.pmi.org/kickoff) 

- [Google Project Management Certificate — Course 1](https://www.coursera.org/professional-certificates/google-project-management)

- [Project Management Skills I Already Use as a Content Creator](https://github.com/florenciacruz3/florenciacruz3/blob/main/PM-skills-as-a-content-creator.md?plain=1)

---

## Week 4 — Entry 2: Writing My First Project Charter

**Date:** July 28, 2026
**Resources completed:**
- Google Project Management Certificate — Course 2: Project Initiation
- The Scrum Guide
- Applied to: Project Charter — Career Change Portfolio

---

### What I Learned

A project charter is the document that says what a project is, why it exists, and what success looks like, before any of the work begins. It is also the document a sponsor signs off on.

What surprised me most is how much of a charter is about saying no. The scope section has two lists: what is in scope and what is out of scope. Writing down what I would *not* do turned out to be just as useful as writing down what I would do.

I also read the Scrum Guide this week to get ready for the Scrum side of project management. The idea that stayed with me is that work happens in short, fixed periods called sprints, and every sprint ends with a look back at what worked and what didn't.

---

### What I Applied

**Project Charter — Career Change Portfolio**

I treated my own career change as a project and wrote a charter for it, with Gastón Cruz as the project sponsor.

- **Goals:** add at least 5 paid projects to my portfolio, land my first Upwork job by the end of the year, and move into an enterprise IT company by March 2027.
- **In scope:** accessibility audits, UX writing and plain language samples, technical writing, information architecture, project management documentation, and LinkedIn posts about my work.
- **Out of scope:** writing unrelated to these fields, client work under NDA, and personal opinion pieces.
- **Risks:** not having enough time, and not making money fast enough. For each one I wrote a plan to reduce it, like keeping a weekly schedule with daily minimums and telling my sponsor when I feel overwhelmed.

Gastón approved the charter on July 28, 2026.

---

### In My Own Words

Writing a charter for my own life felt a little strange at first. But putting my goals in a table, with dates next to them, made them feel real. It also made it easier to say no to things that didn't move me closer to them.

---

## Resources

- [Google Project Management Certificate](https://www.coursera.org/professional-certificates/google-project-management)
- [The Scrum Guide](https://scrumguides.org/)
- [Project Charter — Career Change Portfolio](../Project%20Management/project-charter.md)

---

## Week 5 — Entry 1: Agile, Kanban, and My First Sprint

**Date:** August 4, 2026
**Resources completed:**
- Google Project Management Certificate — Course 5: Agile Project Management
- Scrum.org Open Assessments: Scrum Open, Product Owner Open, Developer Open
- Applied to: Content Pipeline Kanban Board and 2-Week Sprint Calendar

---

### What I Learned

Agile is a way of working in small pieces instead of planning everything up front. Two tools made it click for me:

- **Kanban boards** show every task as a card moving through columns: Backlog, In Progress, Review, and Done. You can see at a glance what is stuck.
- **WIP limits** (work in progress limits) cap how many tasks can be in one column at the same time. I learned that starting fewer things at once is how you actually finish more.

I also practiced with the free Scrum.org open assessments to get ready for the Professional Scrum Master I (PSM I) exam.

---

### What I Applied

**Content Pipeline — Kanban Board**

I built a Kanban board in GitHub to track my own work: certifications, deliverables, practice tests and LinkedIn posts. I added a priority guide so every item gets a priority based on its deadline:

- **High:** due within 5 days
- **Medium:** important, due within 12 days
- **Low:** everything else

**2-Week Sprint Calendar**

I planned my first sprint, from July 23 to July 31, 2026, with a WIP limit of 3 items in progress at a time. The sprint goal was to get meaningful work done without burning out.

At the end, I wrote my first sprint retrospective:

| Question | My answer |
|---|---|
| What went well? | Adding some work on the weekend spread my tasks more evenly. |
| What did not go as planned? | Certifications took longer than I expected. |
| What will I do differently? | Add more work to Tuesdays, which only had two short tasks. |

---

### In My Own Words

I managed to fit two weeks of work into one. But the retrospective showed me that it only worked because I added extra hours. Next time, the goal isn't to do more. It's to plan better, so I don't need the extra hours in the first place.

---

## Resources

- [Agile Project Management (Coursera)](https://www.coursera.org/learn/agile-project-management)
- [Scrum.org Open Assessments](https://www.scrum.org/open-assessments)
- [Content Pipeline — Kanban Board](../Project%20Management/kanban-board-pm.md)
- [2-Week Sprint Calendar](../Project%20Management/2-week-sprint-calendar.md)

---

## Week 6 — Entry 1: Project Management in a Real Job

**Date:** August 2026
**Resources completed:**
- HubSpot Academy — Inbound Certification
- Applied to: Project Charter — Go-to-Market Outreach for Informed Decision

---

### What I Learned

In August, I started an Account Executive internship at Informed Decision, working with Erik Johnson. For the first time, I used project management on someone else's project instead of my own.

The hardest part was HubSpot. We run everything through it, I had never used a CRM before, and this time I had no one to ask. My first week, I spent twelve hours a day trying to make it work, weekends included.

At the end of that week, I took HubSpot's free Inbound certification, and it changed everything. Within about ten days, I had a routine: I wake up, I know exactly what to do, and I know where to go from there.

---

### What I Applied

**Project Charter — Go-to-Market Outreach: Informed Decision Client Acquisition**

I wrote a charter for the internship, approved by Erik Johnson (project sponsor) and Gastón Cruz (mentor) on August 5, 2026.

- **Goals:** land 4 calls out of every 100 emails, send 20 emails a day, and keep up with follow-ups.
- **Out of scope:** phone calls, technical questions about Informed Decision's services, and contacting prospects on platforms we didn't agree on.
- **Risk I planned for:** emails landing in spam. The fix was setting up SPF, DKIM and DMARC, the settings that prove an email really comes from the sender.

---

### In My Own Words

I've never been good at figuring things out on my own. The HubSpot certification is the one I'm most proud of, because nobody told me to take it. I went out of my way to do it, and everything after it was self-taught.

---

## Resources

- [HubSpot Academy — Inbound Certification](https://academy.hubspot.com/courses/inbound)
- [Project Charter — Go-to-Market Outreach](../Project%20Management/project-charter-informed-decision.md)

---

## August 2026 — Entry 2: When the Plan Falls Apart

**Date:** August 2026

---

### What I Learned

I failed the Professional Scrum Master I exam.

I had been rushing through my project management certifications as fast as I could, trying to make everything fit perfectly. That's how I was able to finish so many in so little time. But for this exam, speed worked against me.

---

### What I Applied

Gastón and I decided to take a break from project management and focus on my internship at Informed Decision. I'm still preparing for the exam, but at a slower pace, with time to actually absorb the material.

---

### In My Own Words

I like to be in control. I like having a schedule and knowing exactly what comes next. Failing this exam was the first time this year that my plan didn't work.

What I learned is that discipline is important, but knowing how to pick yourself up after an unexpected change is more important. If I hadn't failed, I might not have given my full attention to the internship that taught me HubSpot, sales writing and how to work with AI tools.

---

## September 2026 — Entry 1: Learning in Public with The Writing Shift

**Date:** September 14, 2026
**Applied to:** The Writing Shift, my biweekly newsletter on LinkedIn and Substack

---

### What I Learned

Having a portfolio isn't enough if nobody knows it exists. So I started writing about my career change in public.

I used to think professional writing had to be formal: no jokes, no anecdotes, nothing personal. Then Miri Rodriguez gave me feedback that changed how I write: write from the heart, be vulnerable, and be myself.

---

### What I Applied

I launched The Writing Shift, a newsletter for anyone starting over, published every other Monday:

| Date | Edition |
|---|---|
| September 14, 2026 | How I Went from Daycare Teacher to Account Executive in Four Months |
| September 28, 2026 | What I Wish Someone Had Told Me About the Tech Industry Before I Entered It |
| October 12, 2026 | Luck, Ego, and Asking for Help: A Writer's Journey |
| October 27, 2026 | From Nepo Baby to Technical Writer: Four Months of Mentorship |

Alongside the newsletter, I post on LinkedIn several times a week about my certifications, my work and what I'm learning.

---

### In My Own Words

The hard part was never opening up. It was consistency. Gastón told me, "After work, you always have the evening and the weekend." Now I see writing as the thing I do after work because I love it, not as a chore.

---

## Resources

- [The Writing Shift on Substack](https://florenciacruzwrites.substack.com)

---

## October 2026 — Entry 1: Technical Writer at Empressa

**Date:** October 2026
**Applied to:** Technical Writer & Onboarding Storyteller Internship at Empressa® | AI Women Trust

---

### What I Learned

In October, Miri Rodriguez offered me a three-month technical writing internship at Empressa® | AI Women Trust. It's the first role I've had where technical writing is the actual job.

Most of my projects involve video, and I thought my Cinema and Media Studies degree had prepared me for that. I was wrong about how much I still had to learn:

- **iMovie was never the only option.** I now use Canva, where I can also find footage for my videos.
- **AI editing tools aren't the enemy.** Tools like Riverside can generate voiceovers and music and turn a still picture into a moving video in minutes.
- **Good enough for an A isn't good enough at work.** On real projects, I want to be able to say, "I'm proud of what I built."

---

### What I Applied

- Write product video scripts and onboarding stories that explain the platform in plain language.
- Audited the company website and presented my recommended changes to the CEO. The changes were implemented.

---

### In My Own Words

School taught me the theory. A few weeks on the job taught me the workflow, and the workflow is what people actually pay for. Miri has been the one pushing me to experiment instead of falling back on what I already knew.

---

*Last updated: October 29, 2026*
