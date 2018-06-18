---
layout:     page
title:      "GitLab pages"
---

>Host websites -- Just edit, push, and your changes are live.

Follow [GitLabs guide here](https://about.gitlab.com/features/pages/). You can use any static site generator but I'm using **Jekyll.**

Like Github you can have a single user site and unlimited project sites.

Project site
------------

### Create a new, local, Jekyll project
(or clone an existing)
{% highlight bash %}cd code
jekyll new helloworld{% endhighlight %}
* Add this [.gitlab-ci.yml](https://gitlab.com/pages/jekyll/blob/master/.gitlab-ci.yml) to the root of your project (this controls the build process)
* Add this [Gemfile](https://gitlab.com/pages/jekyll/blob/master/Gemfile)

### Create a new local repository
{% highlight bash %}cd helloworld
git init{% endhighlight %}
Or in Soucetree:

* Repository Browser: New repository > Create local repository with path as above eg `/code/helloworld`

### Create a new remote repository at GitLab
* Sign up for a [GitLab account](https://gitlab.com/) & login
* Create a new project and copy the url
eg `https://gitlab.com/drmikegardner/helloworld.git`

### Push your local repository to GitLab
{% highlight bash %}git add --all
git commit -m "Initial commit"
git push -u origin master{% endhighlight %}
Or in [Sourcetree](/pages/sourcetree/):

* add files
* commit to local repository
* push to remote repository

### View site
* Check on the build process at [GitLab](https://gitlab.com/) on the Ci/CD > Pipelines page
* Browse to `https://<username>.gitlab.io/<projectname>`
eg `https://drmikegardner.gitlab.io/helloworld`


<!--
Custom domain name ** TODO **
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

-->
