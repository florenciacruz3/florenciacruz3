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

If you’ve ever used Word or Google Docs, you've probably encountered a situation where you spent 20 minutes, trying to fix a heading that won’t cooperate, or designing a whole layout for your article and that after pasting fell apart. Markdown works differently. The formatting is right there in the text, plain as day. And once you understand why that matters, it's hard to go back.

---

#### You stop fighting formatting

In Word, formatting is hidden from you. You can paste from another document and you'll find that the font changes, spacing is off, and you end up spending more time fixing it than writing it. Markdown eliminates this entirely. There’s only one way to create headings, bold text, or lists. When something is wrong, you know exactly what it is and how to fix it. Writing itself is hard enough but having to deal with formatting at the same time is just not practical. The main takeaway from this is that Markdown will put you back where your mental energy should be: on writing. 

---

#### Your files outlast any app

A Markdown file is plain text. You can open it in Notepad, a browser, or any basic text editor — with no software dependency at all. 

A .docx file is different. It requires software that knows how to prase it. You will see that if you open the same .docx in Word, Google Docs, and LibreOffice, you may come accross shifted layouts, inconsistent fonts, broken tables. Even though the content stays the same, the rendering depends on the app reading it. 

The main advantage that Markdown gives you is durability. 

---

#### It works everywhere technical writers work

In technical writing, your content tends to live in different platforms, such as GitHub, Confluence, Read the Docs, and GitBook. These all accept Markdown directly. You write it once, and it renders immediately without conversions or reformatting. The file you draft is the file you publish. 

---

#### It's the industry standard


Markdown is the default writing format these days across the tech industry. The majority of platforms, GitHub, developer tools, README files, release notes, API documentation, are all written in Markdown. Documentation written in clean, well-structured Markdown signals that you understand the environment you're working in. 

---

## 2. Comparing Markdown to What You Already Know

Markdown formatting can feel like a whole new universe, but you're not starting from zero. Heading levels, emphasis, and lists are identical at the *thinking* level. You'll only need to learn some method changes. 

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
Markdown, however, separates writing from formatting, making everything in the text flow better. 

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

- [Google Developers](https://developers.google.com/tech-writing/one/markdown) — Contains links and basic information that will help you get started. 
  
- [Markdown Tutorial](https://www.markdowntutorial.com) — Beginner-friendly, step-by-step lessons, completely free. Takes 30-45 minutes. 

- [CommonMark](https://commonmark.org/help/) — The official interactive tutorial. Takes about 20 minutes. Best starting point.

- [Markdown Guide](https://www.markdownguide.org/basic-syntax/) — Not a course, just a cheat sheet to use day by day. Print it or keep it open.

### Where to practice

There are two useful things I did to build real Markdown fluency: 

-	First, I used GitHub. I created a repository and started writing directly in `.md`. 

-	Second, based on a real webpage, rewriting it in Markdown from scratch using only Markdown syntax. It forces you to make real decisions about structure and formatting that tutorials don't require. 

---

## About the Author

I completed my bachelor's degree in English and Cinema and Media Studies. After that, I spent a while wondering how to apply those skills in the real world. Technical writing was the answer. It sits at the intersection of clear communication and the tools people actually use.

My first step was learning Markdown. 

---

*Last updated: 2026*
