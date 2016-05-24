---
title: "Dr Mikes Tips"
layout: page
tagline:
nav: exclude
---

>Some notes on using Jekyll to create static websites...

* [Jekyll introduction](pages/jekyllintro/)

Installation

* [iTerm](pages/iterm/) -- a nicer terminal
* [Sublime text](/pages/sublime/) -- the text editor you’ll fall in love with
* [Jekyll](/pages/jekyllinstall/) -- transform your plain text into static websites and blogs
* [Sourcetree](/pages/sourcetree/) -- a graphical Git client

Using

* [Jekyll basics](/pages/jekyllbasics/) -- how Jekyll works, how the different components of a site are organised, how to create and publish new sites
* [Markdown](/pages/markdown/) -- easy-to-read, easy-to-write plain text format
* [Github](/pages/github/) -- versioning / tracking changes to your files
* [Github pages](/pages/githubpages/) --- hosting your website
* [Sourcetree](/pages/sourcetree/) -- a graphical Git client to publish your site



{% for post in paginator.posts %}

<article class="home">

  <span class="post-date">
    {% assign d = post.date | date: "%d" | plus:'0' %}
    {{ post.date | date: "%B" }}
    {% case d %}
    {% when 1 or 21 or 31 %}{{ d }}st,
    {% when 2 or 22 %}{{ d }}nd,
    {% when 3 or 23 %}{{ d }}rd,
    {% else %}{{ d }}th,
    {% endcase %}
    {{ post.date | date: "%Y" }}
  </span>

  <h2>
    <a href="{{ site.BASE_PATH }}{{ post.url }}">{{ post.title }}</a>
  </h2>

  <div>
    {% if post.fullview %}
    {{ post.content }}
    {% else %}
    {% if post.shortinfo %}
    {{ post.shortinfo }}
    {% elsif post.description %}
    {{ post.description }}
    {% else %}
    {{ post.excerpt }}
    {% endif %}
    {% endif %}
  </div>

</article>
{% endfor %}


<!--
<hr/>
<ul class="pager"> 

  {% if paginator.previous_page %}
  <li class="previous">
    {% if paginator.previous_page == 1 %}
    <a href="{{ site.BASE_PATH }}/">&larr; Newer</a>
    {% else %}
    <a href="{{ site.BASE_PATH }}/{{ site.paginate_path | replace: ':num', paginator.previous_page }}">&larr; Newer</a>
    {% endif %}
  </li>
  {% else %}
  <li class="previous disabled">
    <a>&larr; Newer</a>
  </li>
  {% endif %}
  
  <li>
    <span class="page_number">Page: {{ paginator.page }} of {{ paginator.total_pages }}</span>
  </li>

  {% if paginator.next_page %}
  <li class="next">
    <a href="{{ site.BASE_PATH }}/{{ site.paginate_path | replace: ':num', paginator.next_page }}">Older &rarr;</a>
  </li>
  {% else %}
  <li class="next disabled">
    <a>Older &rarr;</a>        
  </li>
  {% endif %}

</ul>
-->