---
title: 'I ♥ Markdown'
categories: 'DigitalLife'
header: 
  teaser: /assets/images/62073-12-Best-Markdown-Editors-for-Linux-–-Better-Tech-Tips.png
  overlay_image: /assets/images/62073-12-Best-Markdown-Editors-for-Linux-–-Better-Tech-Tips.png
  overlay_filter: 0.4
excerpt: "Marky Mark and the Funky Bunch"
typora-root-url: ..
gallery1:
  - image_path: /assets/images/241672x-de676349f28721c792a6b2454e578ed3-PFS First Choice 2.0 - WordProcessor.png
  - image_path: /assets/images/10star_trek_-_the_kobayashi_alternative1.png
gallery2:
  - image_path: /assets/images/43030IDEQB45.png
  - image_path: "/assets/images/897072x-d8a28370ccdd531036d58002d37da463-Better Working Eight In One 2.00 - Word Processor.png"
gallery3:
  - image_path: /assets/images/3843wordperfect.png
  - image_path: /assets/images/52917wordperfect-61-17.gif
  - image_path: "/assets/images/420483x-win-2d9e4fd2c3fe83e2f478e65a4864e239-Microsoft Works 3 Win - Word Processor.png"
gallery4: 
  - image_path: /assets/images/31228tenor.gif
  - image_path: /assets/images/54264source.gif
---
![Commodore](/assets/images/001.jpg){: .align-right }
Back in high school, many moons ago, we had a single computer lab full of Commodore PCs. We'd boot them up with an MS-DOS 2.11 diskette then load up the word processor off another diskette. The one we used then was called pfs:FirstChoice and that was my first exposure to writing digitally. I always wrote first drafts in pen. This transcription process between drafts was a great place to do a first-pass edit with a forced separation between writing and editing.

I'd be remiss in not admitting that the Kobayashi Alternative was a great game that I also played on those PCs.

{% include gallery id="gallery1" caption="pfs:Firt Choice & The Kobayashi Alternative" %}

In university, the first software I ever purchased for my Compaq Turbo XT was QuickBasic 4.5 and Spinnaker's Better Working Eight-in-One. Horrible name, but a fantastically popular low-end office productivity suite. I'd re-do all my Modula-2 assignments in QB and write all my papers in 8n1.

{% include gallery id="gallery2" caption="QuickBasic 4.5 & Spinnaker Better Working 8-in-1" %}

Eventually, I moved to WordPerfect 5.1 and Lotus 123. And then on Windows 3.1, I switched to MS Works (because WP6 sucked hard). 

{% include gallery id="gallery3" caption="WordPerfect 5.1, 6.0 for DOS & Microsoft Works for Windows" %}

There's a big problem with all that history though. Aside from having crap on a stack of floppies that always seemed to attract cat fur and feathers (don't ask), the real quandary was in keeping my documents converted to a format that I could open in newer software.

**Eventually all roads led to Microsoft Office.**

{% include gallery id="gallery4" %}

And that's one of the big reasons I talk about plain text as a preferred format for long-term storage.

> Document formats come and go,
> but plain text is forever.
> ~ Doug Langille

I clued in to plain text back in the basement of Nicholson Hall at StFX when I was trying to catalogue my Rush discography on a VAX/VMS system. There's not enough space in this blog post to explain, so you'll have to live with that mystery. The point is that processing text is way easier and faster than processing proprietary binary documents.

Aaaannnndddd... this ties to accessibility. Specifically screen-readers. The simpler the document format, the easier time assistive technologies have with it.​​​​​​​

**Goals for a Sustainable Document Format**

- Human readable
  - You don't need a proprietary app to read the document.
  - You do need a computer though.
- Single column
  - Defined reading path top-to-bottom.
  - ​​​Bonus points for working on different screen sizes.
- Hierarchical structure
  - Defined headings and subheadings.
  - Bonus points for making a table of contents easier.
- Semantic markup
  - Defined text styling for emphasis or strength, not decoration.
  - ​​​​Bonus points for not underlining.

**Enter Markdown**

Markdown is a way to compose in plain text that meets long-term format compatibility and lends itself to basic accessibility tenets. Markdown text is typically run through a text processor for conversion to speech or other document formats (HTML, Docx, etc.)

There are several flavours of Markdown, but [CommonMark](https://commonmark.org/) is the official standard. 

**Here's an example I made up:**

I used [Dillenger](https://dillinger.io/) to render the text. More typically, I use [PanDoc](https://pandoc.org/) to convert file formats when I need.

``````markdown
# Title Heading

And blowing into *maximum warp speed*, you appeared for an instant to be in **two places** at once. We finished our first sensor sweep of ***the neutral zone***.

## Section Heading

Fate protects fools, little children and ships named Enterprise. This is not about revenge. This is about justice.

### Subsection Heading

Maybe we better talk out here; the observation lounge has turned into a swamp. Computer, belay that order. Is it my imagination, or have tempers become a little frayed on the ship lately? Earl Grey tea, watercress sandwiches... and Bularian canapés? Are you up for promotion?

* Now, how the hell do we defeat an enemy that knows us better than we know ourselves?
* But the probability of making a six is no greater than that of rolling a seven.
* I am your worst nightmare!

***

1. You're going to be an interesting companion, Mr. Data.
2. This should be interesting.
3. I guess it's better to be lucky than good. 

Damage report! and attack the Romulans. I've had twelve years to think about it. And if I had it to do over again, I would have grabbed the phaser and pointed it at you instead of them.

> My oath is between Captain Kargan and myself. Your only concern is with how you obey my orders. Or do you prefer the rank of prisoner to that of lieutenant?

Ensign Babyface! Shields up! Rrrrred alert! We could cause a diplomatic crisis. Take the ship into the Neutral Zone.

## Another Section Heading

I'll be sure to note that in my log. The Enterprise computer system is controlled by three primary main processor cores, cross-linked with a redundant melacortz ramistat, fourteen kiloquad interface modules. The game's not big enough unless it scares you a little.

I grabbed this text from [RikerIpsum](http://www.rikeripsum.com) because... reasons.
``````

**You'll note a couple things:**

![3499ed58-8fdf-41b3-a55f-9803e21d16c9](/assets/images/3499ed58-8fdf-41b3-a55f-9803e21d16c9.png){: .align-right }

- The number of # marks determines the depth of the document structure.
  - Convention has it that the first single # is reserved for the document title.
  - Two #s are for sections and three #s denotes a new subsection.
  - You can technically go to six #s, but that seems a wee bit silly.
  - These sections can be used to generate a table of contents. This is really important for screen readers and in generating ebooks.
- Three *s by itself represents a horizontal line. Semantically, it indicates a change in context or topic, but isn't reflected in the document's overall structure.
- Use a blank line as a spacer between paragraphs. Text on adjacent lines are treated as a single paragraph. Multiple line breaks are ignored.
- Text wrapped in *s indicate emphasis (semantic) and is typically presented as italics (styling).
- Text wrapped in two **s indicates strong (semantic) and is typically presented as bold (styling).
- You can express a strong-emphasis with three *s and have it presented as bold italic styling.
- Bulleted and enumerated lists are pretty obvious.
- Quoted text is indicated by a > at the line start. If you're an old-school email person, you'll recognize this in message threading.
- Links are pretty quick to do. `[text to display](http://linktosomething.com)`

![3539a410-9ef6-4ee9-b6af-eea6628c2e99](/assets/images/3539a410-9ef6-4ee9-b6af-eea6628c2e99.png){: .align-right }

**NOTE**

There are more things you can do with Markdown for images, tables, footnotes and other fancy pants stuff. To be honest, I rarely use them. You can make Markdown more complicated if you like, but the KISS principle is best applied here.

**Next week...**

We'll tie this to HTML and Microsoft Word styles.

