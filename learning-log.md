# Accessibility Learning Log
## Florencia Cruz — Technical Writer in Training

In this log, I'll be documenting my learning journey through accessibility as part of my technical writing training under the mentorship of a Microsoft MVP in Data and AI Platforms.

---

## Week 1 — What Accessibility Means and Why It Matters

**Date:** July 2026
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

My writing is meant for everyone with a technological device. 

I myself often look back at when I first moved into the US and wanted to go to the movies with my grandmother. However, soon I discovered that there were no subtitles available for those who don't speak English. 
By not providing subtitles, the content on the screen excludes my grandmother and me from going to the movies, same way documentation that is not accessible excludes readers who 
use screen readers, who navigate by keyboard, who rely on 
high contrast settings, or who need captions to follow 
along with video content.

As a technical writer my job is to make information 
accessible to the reader — that has always been my goal. 
Accessibility gives that goal a technical standard and 
a legal framework. It is not just good practice. In many 
contexts it is a legal requirement under laws like the 
Americans with Disabilities Act and the European 
Accessibility Act.

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

*Last updated: July 2026*
