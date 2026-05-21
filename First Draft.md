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

> ⏱ Estimated reading time: 15 minutes

---

## 1. Why Writers Should Care About Markdown

If you’ve ever encountered a situation where you spent 20 minutes fixing a heading that won’t cooperate or design a whole layout for your article and after pasting fell apart, you’re in the right place. 
Aesthetically Word and Google Docs are built around visual formatting, which is why one single accident can ruin your whole design. However, what sets Markdown apart from Word or Google Docs is that it takes a different approach entirely: the structure lives in the text itself, not in a layer of invisible styling on top of it.
This section breaks down exactly why that difference matters — and why it's worth making the switch.

---
#### You stop fighting formatting

I you open a Word document that someone else created, you’ll find spacing that doesn’t look right, award headline design, or you’ll ran into situations like pasting a paragraph from a different document and have the font being different, line spacing is off, and you’ll and up to spend on hour fixing it while, with Markdown, you could do it instantly. 
To simplify this, what makes Word’s formatting rules frustrating is that the format is hidden from you. There are no actual rules as to how to fix any of the problems mentioned, you’ll just have to hunt through menus and style panels. 
Markdown eliminates this entirely. As I mentioned before, when it comes to Markdown, all you need to learn is coding and troubleshooting. There’s only one way to create headings, bold texts, or lists. There’s nothing hidden in there, nothing is invisible, and nothing can drift out of alignment without you seeing it.  
Writing itself is hard enough but having to deal with formatting at the same time is just not practical. The main take away from this is that Markdown will put you back where your mental energy should be: on writing. 

---

#### Your files outlast any app

Overtime, Microsoft changes .docx format. This means that eventually the version of Word you used to create a file is no longer supported. What happens next is that you try to open in a computer with a different version of Word and the layout shifts, making the fonts and table of contents wrong. You are left with a sloppy document that you spent hours of work formatting.
Markdown files are immune to this. It is a plain text that has, and will always be, readable one very computer, no matter the device or software that you’re using. The content is content, as it should be, which matters a lot for writers who want their work to last. That's a guarantee no .docx file can make.

---

#### It works everywhere technical writers work

On practical piece of information is that, in technical writing, your content is never going to live in one place. GitHub, Confluence, Read the Docs, and GitBook, are all platforms were you can showcase your work. And they all accept Markdown directly. 
This means that when writing is done in Markdown, it requires no reformatting. The file you draft is the file you publish. 
This is not just a convenience, this is a meaningful reduction in the friction between writing and publishing. 

---

#### It's the industry standard

Markdown was invented in 1004 by John Gruber and Aaron Swartz as a way to give writers an easier time to format text for websites without writing HTML. It became successful because it was open, simple, and tool-agnostic. 
For the tech industry, Markdown is the default writing format to this day. 
The overwhelming majority of platforms, such as GitHub, developer tools, CLI documentation, README files, release notes, changelog entries — are all written in Markdown. 
The point that I’m trying to make is that Markdown matters for writers because it is recognized and expected. When it comes to entering the tech industry, candidates’ work, documentation written in clear, well-structured Markdown showcase that the candidate understands the environment they’re on. 
Some of the most common requirements when it comes to technical writing are, “experience with DITA,” “familiarity with MadCap Flare,” or “knowledge of docs-as-code workflows.” Markdown continues to appear on this list. 
For a hiring manager, seeing Markdown on a resume proves that the writer understands text workflows, has some exposure to Git, and can contribute alongside engineers without requiring a tool setup. 

---

## 2. Comparing Markdown to What You Already Know

Markdown formatting can feel like a whole new universe, but you're not starting from zero. Heading levels, emphasis, and lists are idential at the *thinking* level. You'll only need to learn some method changes. 

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
- Lists structure still works the same
- You can still continue writing clearly — Markdown won't change that. 


### What you'll need to learn from scratch

- The syntax symbols: `#`, `**`, `*`, `-`, `[`, `](`, `!`
- Editing without using a tool bar. 
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
Markdown; however, separates writing from formatting, making everything in the text flow better. 

---

**1. Write in plain text**
When you use Markdown, you get to write in plain text. There’s no font, tool bar, or style panel to choose from. The most you would be doing, in regard to formatting, would be putting ** symbols to make the font bold, or adding ## before a title to make it a heading. Formatting on Markdown won’t pull you away from the sentence you’re in the middle of writing. 

---

**2. Preview your document**
Your screen will look a lot more different while writing in plain text in opposition to the finished result. However, you can have a preview pane you can open alongside your text, where you will find: headings, bold text, and lists finalized. 

This is particularly useful when you’re still learning. I allows you to catch small troubleshooting mistake, which, if you catch them early, will save you time later.

---

**3. Use AI as an editing tool**
Using an AI assistant can make the editing process easier. 
Here’s why: 
It’s no secret, AI tools work better with plain text rather than pasting a Word document. There’s often formatting issues that can alter the content of the document. When you paste a Markdown text, AI reads it as it is. Asking AI to check for clarity works directly with what you wrote. 
It's a fast step. Paste your draft, get feedback, make changes, move on.

---

**4. Publish to GitHub or your CMS**
Once your document is ready, you can upload your .md file to GitHub or paste it into your content management system. It renders it automatically, no need to export to PDF first, reformat it, or convert it. The file you wrote is the file you publish. 
On a Word document; nonetheless, you’ll need to export, convert, strip from its document, and reformat the document in order to publish it, while at the same time, adding up time with each step. 
With Markdown, you’re just one click away from having your document submitted. 

---

## 5. Next Steps

Congratulations! You've covered the foundations. Here's where to go from here:

### Recommended tutorials

- [Markdown Tutorial](https://www.markdowntutorial.com) — Beginner-friendly, step-by-step lessons, completely free. Takes 30-45 minutes. 

- [CommonMark](https://commonmark.org/help/) — interactive tutorial with instant feedback. Takes about 20 minutes. She types Markdown on the left, sees the result on the right. Best starting point.
  
- [GitHub Cheatsheet](github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) - Print it or keep it open.

### Where to practice

There are two useful things I did to build real Markdown fluency: 

-	The first was using GitHub. I created a repository and started writing directly in `.md` If you haven’t started using GitHub before, you really should. GitHub puts you in the exact environment where Markdown is used professionally. 

-	The second was, based off a real webpage, rewriting it in Markdown from scratch. By looking at how it is structured, you should be able to recreate it using only Markdown syntax. It will force you to think outside of the box in ways tutorials never quite do, such as, which heading level fits here, does this need a list or a paragraph, how do I handle this link. 


### Connecting Markdown to real-world technical writing roles

As we explored before, Markdown fluency shows up as a requirement in most technical writer’s job postings. The fastest way to signal that to hiring committees is to write publicly — on GitHub, a personal docs site, or a platform like Dev.to.
Another way to really put yourself out there is polish all of your job recruiting platforms. Upwork, LinkedIn, and GitHub, are very recommended. 
Once you have polished accounts, and experience with practicing Markdown, it’s time to publish some of that work in your platform and show off your qualifications.  

---

## About the Author

I come from a writing background rooted in Word and Google Docs — the tools most writers start with. I moved into technical writing because I wanted to work closer to the products and systems I was already writing about.

Learning Markdown was one of the first practical steps I took. This article is both a guide for writers in the same position I was in, and a demonstration that I can write *in* Markdown, write *about* Markdown, and present it in a way that's clear, structured, and easy to follow.

If you're a writer considering technical writing, Markdown is one of the lowest-effort, highest-return skills you can add right now.

---

*Last updated: 2026*
