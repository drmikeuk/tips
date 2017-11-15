---
layout:     page
title:      "Jekyll install"
---

Jekyll is supported on Linux and Mac OS X. [Official installation instructions are here](https://jekyllrb.com/docs/installation/).  
I'm assuming you have a Mac with Yosemite (you can check this via Apple > About This Mac). 

<i class="fa fa-exclamation-circle fa-alert" aria-hidden="true"></i> NB. Update re El Capitan -- /usr/local/bin [ref](https://jekyllrb.com/docs/troubleshooting/#installation-problems)



Prerequisites
-------------

1. Xcode 
2. Xcode command line tools 
3. Ruby
4. RubyGems

You also need to use __Terminal__ to type/paste in code. eg code is displayed in this guide like this:
{% highlight bash %}ls{% endhighlight %}

### Xcode
Install from the mac app store.
Once it’s installed, open Xcode to agree to the terms and conditions.

### Xcode command line tools
{% highlight bash %}xcode-select -p {% endhighlight %}
will test to see if they are installed and show the location if they are

If they are not installed then use this to install:
{% highlight bash %}xcode-select --install{% endhighlight %} 


### Ruby
I'm using the already installed version of Ruby.
{% highlight bash %}ruby -v{% endhighlight %}
will confirm that its installed and the version

### RubyGems
To confirm installed & show the version:
{% highlight bash %}gem -v{% endhighlight %}



Installation
------------

At the terminal prompt type:
{% highlight bash %}sudo gem install jekyll{% endhighlight %}
and enter your password if prompted.

### Troubleshooting

See the [official troubleshooting guide](http://jekyllrb.com/docs/troubleshooting/)

I updated both the xcode command line tools and Ruby gems:

{% highlight bash %}xcode-select --install
gem update --system{% endhighlight %}


### Hello world
Create a new Jekyll site just to see if everything works

{% highlight bash %}cd code
jekyll new myblog
cd myblog
jekyll serve{% endhighlight %}

Now goto [http://localhost:4000](http://localhost:4000)



