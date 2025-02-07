---
title: "How to Improve Your Site's Typography"
date: 2025-02-07T14:54:31-06:00
tags: [design]
summary: Simple tips to give your readers a better experience.
toc: false
draft: false
---

Good typography is the foundation of a well-designed website, especially for personal sites and blogs like this one, where words are the main focus. You don't need fancy layouts or complex design systems (unless you want that, then knock yourself out by all means). Even just paying attention to well-set text, specifically chosen fonts, and proper spacing can elevate your site from something amateurish to something polished with minimal effort. Plus, while the reader may not be able to consciously pick out the difference, good typography is really meant for *them*, the readers of your work. It creates an overall better experience for them.

Many folks overlook typography when setting up a personal site or blog, but it directly impacts readability, user experience and, sometimes, even the credibility of your content. Poorly chosen fonts, too-tight spacing, or sprawling line lengths can make reading uncomfortable, leading discerning readers to click away before they've even engaged with your work. On the other hand, clean and intentional typography makes reading effortless, encouraging visitors to stay longer and enjoy more of what you have to say.

## Core Principles of Good Web Typography

Don't worry. You don't need to be a trained or professional designer to get typography right. The good news is that we can learn from people who *are* trained in these things. Here are some golden "rules" to get started off on the right foot:

### 1. Choose the right fonts
[Serif fonts](https://fonts.google.com/?categoryFilters=Serif:%2FSerif%2F*,%2FSlab%2F*) have a more classic and elegant feel, while [sans-serif fonts](https://fonts.google.com/?categoryFilters=Sans+Serif:%2FSans%2F*) look more modern and minimal.

Stick to two fonts, max. If you use more than one, keep one for body text and one for headings. Mixing too many fonts leads to visual clutter.

Prioritize readability by avoiding overly stylized or novelty fonts for body text (or preferably, at all). If a font looks "cool" but strains the eyes, it's a bad choice.

Be mindful of font sizing. Using adequate font sizing that won't strain the reader's eyes. Don't be afraid of going bigger if it improves legibility. But of course, all things in moderation.

## 2. Create a clear visual hierarchy

Headings should stand out. Use font sizing that is slightly larger than your body text, and optionally bold weights, as well as spacing from the body text to make sections distinct and easy to find.

Contrast is important, so ensure enough difference in size and weight between heading and body text to avoid monotony.

## 3. Optimize readability with proper spacing

60-80 characters per line is the sweet spot for readability. You can adjust this by setting an appropriate `max-width` attribute in your text's container CSS (I usually set anywhere between 650-700px).

The `line-height` CSS attribute for your text should be set between 1.5 and 1.75 for smooth reading flow.

Avoid walls of text by adding a little extra space between paragraphs.

---

The above are general guidelines. When making any changes, the best judges of which settings are right are your eyes. Make tiny adjustments and see where the sweet spot is in terms of readability, which is the most important thing if you haven't picked up on that already. There is certainly an art to it.

## Simple CSS Example for Better Typography

```css
body {
    font-family: "Charter", serif;
    font-size: 18px;
    line-height: 1.6;
    max-width: 700px;
    margin: auto;
    padding: 20px;
    color: #333; /* Softer black is 
                better for readability. */
}
h1, h2, h3 {
    /* font-family: "OtherFont" (if pairing fonts) */
    font-weight: 600; /* Experiment for h2, h3... */
    margin-top: 1.5em;
    margin-bottom: 0.5em;
}
p {
    margin-bottom: 1em;
}
```

The setup above:
- uses a clean serif font for body text and headings,
- ensures adequate line spacing and comfortable reading width, and
- adds additional spacing to prevent things from feeling cramped.

## Tools to make typography even easier

Don't feel the need to tweak every detail and get stuck in analysis paralysis. Here are some reasources that I often use:

- [Butterick's Practical Typography](https://practicaltypography.com/) for expert advice on typography for everyday life
- [Google Fonts](https://fonts.google.com/) for free fonts
- [DaFont](https://www.dafont.com/) even more free fonts
- [Typescale](https://typescale.com/) a tool for setting typographic scale for consistent sizing
- [Fonts in Use](https://fontsinuse.com/) has inspiration from real-world examples of good typography

In closing, I want to emphasize that good typography isn't just about aesthetics, it's about usability, readability, and the overall experience of your site. More likely than not, by making a few small adjustments you can instantly improve how your site or blog feels to your readers. Keep it simple, be intentional, and let your words stand out.