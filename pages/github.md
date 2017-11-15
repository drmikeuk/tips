---
layout:     page
title:      "Github"
---

[Github](https://github.com/) is a web-based repository hosting service. You can use it to host source code plus documentation, wikis, issue tracking & more. Public (ie open) projects are free.

You can also use [Github pages](/pages/github/) to host static websites directly from your Github repository.

Github hosts __Git__ repositories - these are a way of versioning / tracking changes to a set of files.


Git basics
----------

This is just for background information, you might want to skip straight to [Github pages](/pages/github/).

### Create

To create a new local repository simply create a new directory and type `git init`
eg

{% highlight bash %}
cd code
mkdir helloworld
cd helloworld
git init
{% endhighlight %}

### Clone

To grab a copy of a remote repository use `git clone <url>`
eg

{% highlight bash %}
cd code
git clone https://github.com/username/somerepository
cd somerepository
{% endhighlight %}

### Commit

To tell Git which files to version, first __add__ them to the repository using `git add <filename>`.  
Then you need to __commit__ these __staged__ files using `git commit` and providing a brief __commit message__ explaining whats changed.  
And finally you can __push__ these to a remote repository with `git push` eg

{% highlight bash %}
cd code
cd somerepository
git add file1.txt file2.txt
git commit -m 'Initial commit, adding new files'
git push
{% endhighlight %}

![Diagram of git stages](/assets/media/gitbasics.png)
