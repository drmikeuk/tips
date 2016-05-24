---
layout:     page
title:      "SourceTree"
---

>A free Git & Mercurial client for Windows or Mac

Use SourceTree as a graphical tool to transfer files to/from Github (& other respositories).

Install
-------

[Download here](https://www.sourcetreeapp.com/), and install.    
Then drag to your dock for easy access.

Usage
-----

[This tutorial](http://www.bogotobogo.com/cplusplus/Git/Git_GitHub_Source_Tree_1_Commit_Push.php) covers cloning and then pushing content to a Github repository in full detail. In summary:

### Clone a repository

1. New repository > Clone from url
1. Source url = eg `https://github.com/<username>/<repository>`
1. Destination path = local folder eg `/code/<repository>`
1. Name = label in sourcetree for this respostory eg `<repository>`
1. Click __Clone__

### Pull changes from Github

1. Click __Pull__ in the top bar

![Toolbar: Pull](/assets/media/sourcetreepull.png)

### Commit and push changes to github

When you change or add files on your local machine you have "Unstaged files"...

1. Select these to __stage__ them (select each file or tick 'Unstaged files' to select all)
2. Provide a commit message, tick "Push changes immediately to origin/master" and click __commit__

![Stage files](/assets/media/sourcetreestage.png)

![Commit](/assets/media/sourcetreecommit.png)