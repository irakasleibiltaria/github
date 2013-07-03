###GitHub Pages
http://irakasleibiltaria.github.io

[GitHub Pages](https://help.github.com/categories/20/articles). 

one example: [backbone book](http://addyosmani.github.io/backbone-fundamentals/)

###Syntax
README.md syntax: 'M' key. 

https://help.github.com/articles/github-flavored-markdown 

https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet

###Backup
http://addyosmani.com/blog/backing-up-a-github-account/

https://github.com/joeyh/github-backup

http://stackoverflow.com/questions/1251713/backup-of-github-repo

```bash
To create the mirror:
$ git clone --mirror git://github.com/user/project.git
To update:
$ cd project.git
$ git remote update
```

###download files from GitHub
go to the file you want to dowload and push the **view raw button** <> and copy the URL and use **curl** to download
it.
```bash
$ curl https://raw.github.com/irakasleibiltaria/startup-engineering/master/README.md
```
from gists:
```bash
$ curl https://gist.github.com/irakasleibiltaria/5875179/raw/9156a226d26971a239d2d6d66c9cc0e80d0ed6ee/grub-recovery.sh
```
you can download and execute:
```bash
$ curl https://gist.github.com/irakasleibiltaria/5875179/raw/9156a226d26971a239d2d6d66c9cc0e80d0ed6ee/grub-recovery.sh | sh
```

Other option: https://rawgithub.com/

###GitHub API
http://developer.github.com/v3/
```bash
# List public repositories for the specified user.
# GET /users/:user/repos

$ curl -i https://api.github.com/users/irakasleibiltaria/repos
```
The response is a Json file. To obtain only repositories names:

[github-repos.js](https://gist.github.com/irakasleibiltaria/5922660)

