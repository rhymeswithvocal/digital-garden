---
title: Git & Github
status: branch
---

This isn't one of the direct [[Lessons from Building this Site]] but it's definitely come up a lot, and I want to keep track of my resources and make some notes.

## Cloning

Git repos can exist in remote (online) and local states, so a lot of using git is concerned with keeping those versions aligned and up-to-date. To add an existing remote repository to your local machine, it's just a simple

`git clone <link>`

## .Gitignore

- gitignore tells git what files to exclude from tracking BUT if a file has been previously tracked, adding it to gitignore won't remove it from tracking. To do that, you need to use `git rm --cached <file>`

---
### Sources, resources, links

A very handy [cheat sheat](https://gist.github.com/cferdinandi/ef665330286fd5d7127d) of commands.

How to [override local changes](https://stackoverflow.com/questions/1125968/how-do-i-force-git-pull-to-overwrite-local-files).