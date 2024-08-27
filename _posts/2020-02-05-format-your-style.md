---
title: 'Format Your Style'
categories: 'DigitalLife'
typora-root-url: ..
header: 
  teaser: /assets/images/58743-cm1-f.jpg
  overlay_image: /assets/images/58743-cm1-f.jpg
  overlay_filter: 0.4
excerpt: "Long live Comic Papyrus"
screenshots1:
  - image_path: /assets/images/22806Capture2.PNG
  - image_path: /assets/images/27817Capture3.PNG
screenshots2:
  - image_path: /assets/images/55315Capture5.PNG
  - image_path: /assets/images/62359Capture6.PNG
---
Okay. So the last two weeks, we've been on a plain text kick and then did the markdown thing. This week, I'm going to wrap this topic up.

![05c78b3b-6ab1-459d-869e-0dd937fc85ba](/assets/images/05c78b3b-6ab1-459d-869e-0dd937fc85ba.gif){: .align-right }

We've already established that plain text is a great sustainable, future-proof and portable document format and that markdown provides enough text formatting to convey the semantic meaning of document structure beyond the words themselves.

It's a great way to manage the "source code" of your creative works.

**Of course, life isn't lived in black-and-white and plain text isn't the final presentation.**

![f54d2013-4cf6-46bb-b34a-1312160a5a13](/assets/images/f54d2013-4cf6-46bb-b34a-1312160a5a13.gif){: .align-right }

There are many tools that are used to convert markdown-formatted plain text to other formats. Most of the apps out there use Pandoc in the background to do the heavy lifting. [Pandoc](https://pandoc.org/) is free.

The command: 

`pandoc -o fancydoc.html fancydoc.txt`

...will convert the plain text document fancydoc.txt to a web page fancydoc.html.

This command:

`pandoc -o fancydoc.docx fancydoc.txt`

...will result in a Microsoft Word document.

You can even make an ebook using Pandoc if you feel so inclined.

Anyway, the idea is that markdown can convert to a web or Word document rather readily. And just about anything else.

**How is this possible? Are you some sort of wizard?**

**Glad you asked.** No, I am not but take this little ditty:

```markdown
# Title

## Chapter 1

Call me *Ishmael*.

> A dude **walks** into a ***bar***.

* one
* two
* three
```

Here's how pandoc converts it to HTML:

```html
<h1>Title</h1>
<h2>Chapter 1</h2>
<p>Call me <em>Ishmael</em>.</p>
<blockquote>
<p>A dude <strong>walks</strong> into a <strong><em>bar</em></strong>.</p>
</blockquote>
<ul>
<li>one</li>
<li>two</li>
<li>three</li>
</ul>
```

![b142139a-1eee-4624-a77e-17b629415b07](/assets/images/b142139a-1eee-4624-a77e-17b629415b07.png){: .align-right }

You'll quickly notice how much more readable markdown is as source-code over HTML. Which is the whole reason markdown was created in the first place-- a one-to-one element conversion to HTML.

**Now...**

You can style the HTML using a thing called CSS (yeah, call acronyms anonymous). I won't make you all bleary-eyed with code, but essentially, you can style elements and classes to look differently. For example, you can make all first-level headers in the font Comic Sans, make all strongly-emphasized text become red and put a grey background behind quoted/blocked text. You do you. I won't judge. Much.

The separation of semantic content from presentation is pretty important to how the web works.

If you want to chat more about HTML and CSS, I'd be only too happy to do such. But to be honest, that's the jam of the Digitial Products and Experience team. They could talk about this stuff all day.

**So finally, now let's look at Microsoft Word.**

I converted the snippet above to Word and it looks like these screenshots.

{% include gallery id="screenshots1" %}

You'll notice all the semantic structure came across and were styled in that oh-so-unique Microsoft way. Take a look at the other screengrab. You'll see how the markdown formatting became Word styles.

What's important here to remember is that you should always be using Word styles for the semantic/structural elements of your document-- headings, blocked text, etc.

The reasons are many, but here are three:

1. **Accessibility** for screen readers and stuff. I mentioned this last week, but it bears repeating. If your document is semantically well-structured, then the screen readers will have an easier time.
2. **Theming**. If you're using Word's style functionality, then you can use the themes stuff under the Design ribbon. And, yes, you can define your own theme design. This is pretty much the same as the CSS styling for HTML documents. 
3. **Tables of Contents** link to Microsoft heading styles... automagically.

{% include gallery id="screenshots2" %}

**So that's it for now.**

If you can tweak how you layout your Word documents so that you use styles, you'll save yourself a lot of headache and possibly heartache.