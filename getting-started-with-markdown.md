# Getting Started with Markdown
## For Writers Coming from Word or Google Docs

---

## Overview

**Who this article is for:** Writers with basic knowledge of Word or Google Docs.

**What you will learn:**

1. [Why Writers Should Care About Markdown](#1-why-writers-should-care-about-markdown)
2. [Comparing Markdown to What You Already Know](#2-comparing-markdown-to-what-you-already-know)
3. [Core Markdown Syntax](#3-core-markdown-syntax)
4. [The Markdown Workflow](#4-the-markdown-workflow)
5. [Next Steps](#5-next-steps)

**What this article does *not* cover:**

- HTML embedded inside Markdown
- Writing README files for software projects
- Advanced Markdown tutorials or concepts

> ⏱ Estimated reading time: 10 minutes

---

## 1. Why Writers Should Care About Markdown

If you’ve ever used Word or Google Docs, you've probably encountered a situation where you spent 20 minutes, trying to fix a heading that won’t cooperate, or designing a whole layout that fell apart after pasting. Markdown works differently. The formatting is right there in the text, plain as day. And once you understand why that matters, it's hard to go back.

---

#### You stop fighting formatting

In Word, formatting is hidden from you. You can paste from another document and you'll find that the font changes, spacing is off, and you end up spending more time fixing it than writing it. Markdown eliminates this entirely. There’s only one way to create headings, bold text, or lists. When something is wrong, you know exactly what it is and how to fix it. Writing itself is hard enough but having to deal with formatting at the same time is just not practical. 

The main takeaway from this is that Markdown will put you back where your mental energy should be: on writing. 

---

#### Your formatting stays consistent across every app

A Markdown file is plain text. You can open it in Notepad, a browser, or any basic text editor — with no software dependency at all. 

A .docx file is different. It requires software that knows how to parse it. Open the same .docx in Word, Google Docs, and LibreOffice and you may come across shifted layouts, inconsistent fonts, broken tables. The content stays the same. The rendering depends on the app reading it. 

The problem isn't which app you use — it's that .docx files depend on the app to look right. Markdown doesn't.

---

#### The tech industry already speaks Markdown

In technical writing, your content lives across multiple platforms — GitHub, Confluence, Read the Docs, GitBook. Every one of these accepts Markdown directly. You write it once and it renders immediately, without conversions 
or reformatting.

Markdown is the default writing format across the tech industry. README files, release notes, API documentation, developer tools — all written in Markdown. Documentation written in clean, well-structured Markdown signals that you understand the environment you're working in. It's not just a useful skill. It's the expected one.

---

## 2. Comparing Markdown to What You Already Know

Markdown formatting can feel like a whole new universe — but you're not starting from zero. Heading levels, emphasis, and lists are identical at the *thinking* level. The concepts are identical. Only the symbols are new.

### Word vs. Markdown

| Feature | Word | Markdown |
|---|---|---|
| Headings | Toolbar → Heading 1 | `# Heading 1` |
| Bold | Ctrl + B | `**bold**` |
| Italic | Ctrl + I | `*italic*` |
| File format | `.docx` (proprietary) | `.md` (plain text) |
| Portability | Requires Word | Any device, any app |

### Google Docs vs. Markdown

| Feature | Google Docs | Markdown |
|---|---|---|
| Headings | Format menu | `## Heading 2` |
| Links | Insert → Link | `[text](url)` |
| Bullet lists | Toolbar button | `- item` |
| Collaboration | Real-time, cloud-only | Git-based, works offline |
| Export options | PDF, .docx | Renders anywhere |

### What transfers directly from your existing skills

- Headings continue to work in hierarchy (H1 → H2 → H3)
- Using emphasis to guide the reader
- List structure still works the same
- You still write clearly — Markdown won't change that. 


### What you'll need to learn from scratch

- The syntax symbols: `#`, `**`, `*`, `-`, `[`, `](`, `!`
- Editing without using a toolbar 
- Previewing your work: always double check your rendered output separately from your raw text

---

## 3. Core Markdown Syntax

### Headings

Use `#` symbols to define heading levels. One `#` is the largest; six `######` is the smallest.

```
# Heading 1
## Heading 2
### Heading 3
#### Heading 4
```

> [!NOTE]
> Always include a space after `#` — without it, the heading won't render.

---

### Bold and Italic

Wrap text in `**double asterisks**` for **bold**, and `*single asterisks*` for *italic*.

```
**This text is bold.**
*This text is italic.*
***This text is bold and italic.***
```

> [!NOTE]
> Make sure every opening `*` has a closing one. Mismatched symbols break rendering.

---

### Bullet Lists and Numbered Lists

Use `-` or `*` for unordered lists. Use numbers followed by a `.` for ordered lists.

```
- First item
- Second item
  - Nested item

1. Step one
2. Step two
3. Step three
```

> [!NOTE]
> Keep indentation consistent. Uneven spacing breaks nested lists.

---

### Links

Wrap the display text in `[square brackets]` and the URL in `(parentheses)` immediately after.

```
[Visit Markdown Guide](https://www.markdownguide.org)
```

> [!NOTE]
> Don't swap the brackets and parentheses — text goes in `[]`, the URL goes in `()`.

---

### Images

Images follow the same syntax as links, with a `!` added at the very beginning.

```
![A description of the image](https://example.com/image.jpg)
```

> [!NOTE]
> Don't forget the `!` at the start. Without it, the image renders as a broken link instead.

---

### Blockquotes

Add `>` before a line to turn it into a blockquote.

```
> This is a blockquote. Use it for callouts, warnings, or quoted material.
```

> [!NOTE]
> Include a space after `>`. Some parsers won't render the block without it.

---

## 4. The Markdown Workflow

In Word or Google Docs, writing and formatting happen at the same time. You keep switching back and forth between typing a sentence, then clicking a menu, then adjusting a heading, then getting back to the sentence. 

Markdown, however, separates writing from formatting, making everything in the text flow better. 

Here is how that separation works in practice.

**1. Write in plain text**

When you use Markdown, you get to write in plain text. There’s no font, toolbar, or style panel to choose from. Formatting on Markdown won’t pull you away from the sentence you’re in the middle of writing. 

**2. Preview your document**

Your screen will look quite different while writing in plain text compared to the finished result. However, opening the preview pane alongside your text helps you catch mistakes early, before they become bigger problems.

**3. Use AI as an editing tool**

AI tools work better with plain text. Paste your draft, ask for feedback, and make changes. There's no formatting baggage to strip out first — what you paste is exactly what the AI reads.

**4. Publish to GitHub or your CMS**

Once your document is ready, you can upload your .md file to GitHub or paste it into your content management system. It renders it automatically, no need to export to PDF first, reformat it, or convert it. The file you wrote is the file you publish. 

---

## 5. Next Steps

You've covered the foundations. Here's where to go from here:

### Recommended tutorials

- [Google Developers](https://developers.google.com/tech-writing/one/markdown) — Contains links and basic information that will help you get started. It's easy to comprehend, not heavy on information, and completable in less than a week. 
  
- [Markdown Tutorial](https://www.markdowntutorial.com) — Beginner-friendly, step-by-step lessons, completely free. Takes 30-45 minutes. Although, I wish I had understood why Markdown is a better tool than Word before stepping into syntax, I found these activities to be extremely useful and easy to do. This is the best way to comprehend basic Markdown syntax in less than an hour. 

- [CommonMark](https://commonmark.org/help/) — The official interactive tutorial. Takes about 20 minutes. It fills the gaps, and the repetition made the new material stick. Do this one right after Markdown Tutorial.

- [Markdown Guide](https://www.markdownguide.org/basic-syntax/) — Not a course, just a cheat sheet to use day by day. This cheatsheet continues to be useful to this day. Once you are done learning tutorials and you are faced with having to work on a Markdown project on your own, the quickest way to remember how to do syntax is not searching it online, having this open in a browser tab or printed next to you.

- [GitHub Guide](https://github.com/git-guides) — Introduction to GitHub. Takes 20 minutes to read. If you want to learn about GitHub and have a quick visualization of what it is, I recommend reading this article. Good for orientation, not a complete resource.
  
- [GitHub QuickStart](https://docs.github.com/en/get-started/start-your-journey/hello-world) — Deep guide into everything you'll need to learn before using GitHub. This is extensive, long material. Can take a couple of days to read through it — but don't skip it. This guide contains everything you need to learn about GitHub. I wouldn't have known where to begin without it. 

- [FreeCodeCamp's Git & GitHub full course](https://www.youtube.com/watch?v=RGOj5yH7evk) — 1 hour YouTube video. Watch this video before the branching activity below. If you learn better by watching than reading, this is yours. It's relatively short and easy to follow.

- [Learning Branching](https://learngitbranching.js.org) — Interactive coding activity. It takes about 2 hours to complete. This one was the real challenge. Don't attempt it without completing the resources above. It's level based. I managed to get up to the last level when I did this, but my recommendation is that if you get stuck before the end, move on. 

### Where to practice

There are three useful things I did to build real Markdown fluency: 

- **First, I set up my GitHub profile and first repository.**

While working with GitHub QuickStart simultaneously, I followed each step as I was reading it. I created a GitHub profile, a repository, and a README file. 

Once you've absorbed all the information that was listed on the previous section, navigating through GitHub felt manageable. 

> [!TIP]
> The first time that I came into contact with GitHub, I didn't know why my Markdown syntax wasn't rendering. I had to Google it. It turns out that to do Markdown syntax on your GitHub, your file must end in `.md` for GitHub to recognize it as Markdown. Name your files accordingly from the start.
  
- **Second, I rewrote a real webpage in Markdown from scratch using only Markdown syntax.**

I decided to pick one of the pages from Google Developer's course and re-create it. This is the real test of your knowledge. 

It will get you to practice your fluency on Markdown syntax. It forces you to make real decisions about structure and formatting that tutorials don't require.

If one page doesn't feel like enough, do another.

> [!TIP]
> There are many Markdown apps out there but write directly in GitHub instead. Once I wrote my first Markdown practice page, it turns out there were broken links that weren't visible to me until I turned it in. After that, everything clicked. 

- **Third, I wrote my first piece on GitHub from scratch.**

This is where actual writing comes in. 

When I wrote this article, I had complete freedom. You're not just copy-pasting any information and design from any website. You can add tables, lists, blockquotes, headings, and bold text, as you please. 

I started with an outline and wrote a first draft. 

From there, the writing process stays the same: proofreading, editing, rewriting, and getting feedback. When you're ready, create a pull request. At this point nobody knows this pull request exists. Tag the person you want to review it in the comments or send them the URL directly.

> [!TIP]
> You need existing changes in your branch before GitHub will let you open one. Always remember to create your pull request at the beginning of the editing process, I've made that mistake before.  

Once you feel confident in your piece, be ready to defend it.

---

## About the Author

I completed my bachelor's degree in English and Cinema and Media Studies. After that, I spent a while wondering how to apply those skills in the real world. Technical writing was the answer. It sits at the intersection of clear communication and the tools people actually use.

My first step was learning Markdown. 

**Connect:**
[LinkedIn](https://www.linkedin.com/in/florencia-cruz-assandri) · 
[Upwork](https://www.upwork.com/freelancers/~01be3448096dd46eac)

---

*Last updated: May 2026*
