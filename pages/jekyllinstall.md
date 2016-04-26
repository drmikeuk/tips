---
layout:     page
title:      "Jekyll install"
---

https://jekyllrb.com/docs/installation/

http://digitalshore.io/how-to-install-jekyll-mac-osx-yosemite/


Prerequisites
-------------
Jekyll is supported on Linux and Mac OS X. I'm assuming you have a Mac with Yosemite or El Capitan (you can check this via Apple > About This Mac).

You also need to use __Terminal__ to type/paste in code which is displayed in this guide like this:
{% highlight bash %}ls{% endhighlight %}

1. Xcode 
2. Xcode command line tools 
3. Ruby
4. RubyGems

### Xcode

### Xcode command line tools
xcode-select -p will confirm that its installed and the version
if its not installed then install using xcode-select --install

### Ruby
I'm going to use the already installed version of Ruby. ruby -v will confirm that its installed and the version

### RubyGems
gem -v will confirm that its installed and the version







Installation
------------
https://jekyllrb.com/docs/installation/
The best way to install Jekyll is via RubyGems. At the terminal prompt:
$ gem install jekyll

Requirements



1. Xcode - http://stackoverflow.com/questions/15371925/how-to-check-if-command-line-tools-is-installed
			xcode-select -p 	-> dir 				-> is installed on macbook (osx 10.10.5 Yosemite)
2. Ruby		ruby -v 			-> ruby 2.0.0p481 	-> is installed
3. RubyGems gem -v 				-> 2.0.14 			-> is installed
4. NodeJS

http://digitalshore.io/how-to-install-jekyll-mac-osx-yosemite/
sudo gem install jekyll

http://jekyllrb.com/docs/troubleshooting/ suggests sudo gem update --system
but still fails

try xcode-select --install

