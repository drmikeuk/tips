---
layout:     page
title:      "Github pages"
---

>Host websites -- Just edit, push, and your changes are live.

Follow [Githubs guide here](https://pages.github.com/).

User site
----------

* Sign up for a [Github account](https://github.com/)
* Create a new repository at [github.com](https://github.com/new) named _username_.github.io
	* Add collaborators if push access required for others (Settings: collaborators)
* Goto the place where you want to store your files eg `cd code`
* Clone the repository `git clone https://github.com/<username>/<username>.github.io` (or use sourcetree)
* Add some content (eg index.html)
* Push it 
{% highlight bash %}git add --all
git commit -m "Initial commit"
git push -u origin master{% endhighlight %}
* Browse to `http://<username>.github.io`

Project site
------------

* Create a new repository at [github.com](https://github.com/)
* Create a gh-pages branch
* Make gh-pages the default branch (since the primary purpose is to serve a static website)
* Clone the repository `git clone https://github.com/<username>/<repository>.github.io` (or use sourcetree)
* Add some content (eg index.html)
* Push it 
{% highlight bash %}git add --all
git commit -m "Initial commit"
git push -u origin master{% endhighlight %}
* Browse to `http://<username>.github.io./<repository>`


Custom domain name
------------------

See [Githubs documentation](https://help.github.com/articles/setting-up-your-pages-site-repository/)

Add your custom domain name

* Create a new file in your repository called CNAME (with all caps!)
* In this file add a single domain with your custom domain name (just the name; no http://)
* Push this new file

Confirm your custom domain name on [Github](https://github.com/)

* Goto your repository on Github
* Click Settings (cog icon; top right)
* Under 'Github Pages' you should see "Your site is published at _your domain name_"

Set up your custom domain with your DNS provider

* See [Githubs documentation](https://help.github.com/articles/quick-start-setting-up-a-custom-domain/)
* eg for subdomains setup a CNAME for projectname.mydomain.com that points to yourusername.github.io
* eg for apex domains (eg mydomain.com) setup an A record to point to githubs servers (may take 24-48hrs to take effect)


