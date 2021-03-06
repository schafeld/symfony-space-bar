# symfony-space-bar
Fun tutorial project with PHP Symfony.

Based on https://symfonycasts.com/screencast/symfony4/setup

Work in progress...


## Basic Symfony setup

Preparation

`composer self-update`

Install Symfony 4 boilerplate

`composer create-project symfony/skeleton my_project_name '4.4.*'`


Put project under version control

```bash
cd my_project_name

git init
git add .
git commit -m "initial commit"

# create Github project repository "my_project_repo"

git remote add origin git@github.com:my_github_account_name/my_project_repo_name.git
remote -v
git push -f origin master

git branch --set-upstream-to=origin/master  master
git push
```

### Install a (better) local server

You can run a local PHP server

`php -S 127.0.0.1:8000 -t public`

or for local development just

`php -S 127.0.0.1:8080`

But after

`composer require server`

there's a _better_ server at your disposal which is started like this:

`bin/console server:run`

### Add tools

For more comfortable route creation via annotation:

`composer require annotations`