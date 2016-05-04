---
layout:     page
title:      "Jekyll basics"
---

Check out the [Jekyll documentation](https://jekyllrb.com/docs/home/) plus these [Jekyll Tips](http://jekyll.tips/guide/introduction/).

Overview
--------
Jekyll takes plain text files plus template files and spits out a functional website.  
This will create a new test site:
{% highlight bash %}cd code
jekyll new mytestsite
cd mytestsite
jekyll serve{% endhighlight %}
Now browse to [http://localhost:4000](http://localhost:4000])

When you edit or add pages Jekyll will regenerate the site and you can see the changes when you reload your browser.

Files
-----

| FileDirectory | Contains |
| ------------ | ------------- | 
| _config.yml | site config |
| _includes   | parts of templates |
| _layouts    | page templates |
| _posts      | blog posts |
| _site       | your generated site |
| about.md    | an about page |
| index.html  | the home page |




Create a new site
-----------------

Assuming that you keep your code in a directory called 'code'.

NB. Edit the <code>_config.yml</code> to change the port from 4000 to say 4001

### From scratch

To create a site called 'mytestsite' in a directory called 'code'
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
eg https://uazmjg@bitbucket.org/uazmjg/frederickdouglass.git
cd existingsite 		# or whatever the name of the existing site is
jekyll serve{% endhighlight %}
Now browse to [http://localhost:4000](http://localhost:4000])



Content
-------

Pages of your site can sit in the root eg `/index.html`

Blog posts live in `_posts`

### YAML

### Markdown

Publish / Deploy
----------------