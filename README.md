# Name Hover

A name where every letter reacts on its own, from [miguelclavel.com](https://miguelclavel.com/?utm_source=github&utm_medium=name-hover).

<img src="assets/demo.gif" width="720" alt="A name where every letter reacts on its own: a screen recording">

**[Try it live](https://miguelclavel.github.io/name-hover/)** · one file, `index.html`, no libraries, no build step.

Here's the actual trick behind the hover effect on my name. Steal it.

I wanted the first thing you touch on the page to feel alive, without turning my own name into a toy. So the rule was simple: react to the exact letter under your mouse, never the whole word.

Each of the 12 letters in "Miguel Clavel" gets its own animation, and neighbours never share one. One squashes like jello. One tips over and swings back. One drops, then springs up past where it started. One flips right over in 3D. The rest shiver, pop, hop, or slide. Eight in total.

Here's the bit I had to fix by hand. They kept firing while the name was shrinking up into the header on scroll, which looked broken. One check stops a letter animating once the name starts moving.

If you build this, send it to me. I'd genuinely like to see it.

## Use it on your site

Split any heading into letters and give each one its own move. Copy the `<style>` block (the eight `@keyframes`) and the `<script>` from `index.html` into your page, and change `id="name"` to your heading. Everything turns off for people who prefer reduced motion.

## Or build your own from the prompt

Copy it as it is and paste it into Claude, or any AI coding tool.

```text
Split this heading into individual letters, each in its own element. Write eight short hover animations: a squash and stretch, a tip over that swings back, a drop and spring up, a 3D flip, a sideways slide, a shiver, a scale pop, and a hop. Cycle them across the letters so neighbours never match. Each runs between half a second and two seconds, and plays only when the mouse enters that one letter. Give each a sensible transform origin. Turn it all off for reduced motion.
```

More like this in [interaction-recipes](https://github.com/miguelclavel/interaction-recipes).

---

MIT licensed. Made by [Miguel Clavel](https://miguelclavel.com/?utm_source=github&utm_medium=name-hover) with Claude Code. If you build one of these, send it to me. I'd genuinely like to see it.
