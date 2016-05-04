---
layout:     page
title:      "Markdown"
---

> An easy-to-read, easy-to-write plain text format that can be converted to HTML

[Kramdown](http://kramdown.gettalong.org/quickref.html) is Jekylls default flavour of [Markdown](https://daringfireball.net/projects/markdown/). You can mix in vanilla HTML too.

This code
=========

{% highlight markdown %}
A Header
--------

### Sub-heading

A paragraph of text with __bold__ and _italic_

Another paragraph

> A blockquote.

* Bulleted lists
* are easy
	* tab in for indents

1. Numbered lists are easy too
1. No need to number correctly!

> A big blockquote with a source
> <footer><cite>Source</cite></footer>

[link title](url) eg [link to google](http://google.com/)

![Picture of Albatross](/assets/media/albatros.jpg)
<span class="caption text-muted">Albatross ahoy!</span>

Add footnotes using placeholders like this: [^1]. 
Alternatively you can use ‘n’ rather than numbers [^n] so you don’t have to worry about which number
you are on. At the very end of your post, you can define your matching footnotes as shown below:

[^1]: This is my first footnote
[^n]: A final footnote

Use backticks for inline code: `some command here` within a paragraph

For longer blocks and different language syntax highlighting:
{% highlight bash %}cd somedir
xcode-select -p {% endhighlight %}

{% endhighlight %}

Becomes
=======

A Header
--------

### Sub-heading

A paragraph of text with __bold__ and _italic_

Another paragraph

> A blockquote.

* Bulleted lists
* are easy
	* tab in for indents

1. Numbered lists are easy too
1. No need to number correctly!

> A big blockquote with a source
> <footer><cite>Source</cite></footer>

[link title](url) eg [link to google](http://google.com/)

![Picture of Albatross](/assets/media/albatros.jpg)
<span class="caption text-muted">Albatross ahoy!</span>

Add footnotes using placeholders like this: [^1]. Alternatively you can use ‘n’ rather than numbers [^n] so you don’t have to worry about which number you are on. At the very end of your post, you can define your matching footnotes as shown below:

[^1]: This is my first footnote
[^n]: A final footnote

Use backticks for inline code: `some command here` within a paragraph

For longer blocks and different language syntax highlighting:
{% highlight bash %}cd somedir
xcode-select -p {% endhighlight %}