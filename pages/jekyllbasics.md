---
layout:     page
title:      "Jekyll basics"
---

This page outlines how Jekyll works, how the different components of a site are organised, how to create and publish new sites.

For more information check out the [Jekyll documentation](https://jekyllrb.com/docs/home/) plus these [Jekyll Tips](http://jekyll.tips/guide/introduction/).



Overview
--------
Jekyll takes plain text files plus template files and spits out a functional website.  
__When you edit or add pages Jekyll will regenerate the site and you can see the changes when you reload your browser.__

eg this will create a new test site:
{% highlight bash %}cd code
jekyll new mytestsite
cd mytestsite
jekyll serve{% endhighlight %}
Now browse to [http://localhost:4000](http://localhost:4000])


Files
-----

| File / Directory | Contains      |
| ------------     | ------------- | 
| _config.yml      | site config   |
| _includes        | parts of templates |
| _layouts         | page templates |
| _posts           | blog posts |
| _site            | your generated site |
| about.md         | an about page |
| index.html       | the home page |
{:.table}

Create a new site
-----------------

Assuming that you keep your code in a directory called 'code'.

NB. If you have several Jekyll sites then you may want to edit the <code>_config.yml</code> to change the port from 4000 to say 4001.

### From scratch

To create a site called 'mytestsite' in a directory called 'code':
{% highlight bash %}cd code
jekyll new mytestsite
cd mytestsite
jekyll serve{% endhighlight %}
Now browse to [http://localhost:4000](http://localhost:4000])

### From a template

{% highlight bash %}cd code
unzip template
cd template 			# or whatever the name of the template is
jekyll serve{% endhighlight %}
Now browse to [http://localhost:4000](http://localhost:4000])


### Clone from an existing site

{% highlight bash %}cd code
git clone existingsite
cd existingsite 		# or whatever the name of the existing site is
jekyll serve{% endhighlight %}
Now browse to [http://localhost:4000](http://localhost:4000])

eg git clone https://uazmjg@bitbucket.org/uazmjg/frederickdouglass.git


Content
-------

Pages of your site can sit in the root eg `/index.html` or subdirectories eg `/tools/index.html`.  
Blog posts live in `_posts` and should be named `YYYY-MM-DD-title.MARKUP` eg `2015-12-31-new-years-eve-is-awesome.md`

Content has two parts:

* __metadata__ in the front piece
* the visible content

### Metadata

The format is YAML between two sets of triple dashes: \-\-\-, which sits at the beginning of a file.
This metadata can specify which layout to use or variables (eg title or thumbnail image) which can be included in the page. eg:

{% highlight bash %}---
layout:     page
title:      "Jekyll basics"
---{% endhighlight %}

### Content

This can be full HTML but I prefer [Markdown](/pages/markdown/) for its simplicty and readability.

Publish / Deploy
----------------

Once your site is ready you can simply copy the files from `_site` to a webserver to make it visible to the world.

One very simple way to publish a site is to use [Github pages](/pages/githubpages/).


