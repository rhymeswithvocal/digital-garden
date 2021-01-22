---
title: Liquid
---

One of the [[Lessons from Building this Site]] is picking up a general familiarity with Liquid, which according to their site is

> an open-source template language created by Shopify and written in Ruby

I know all of those words separately, but in that string, not so much. Nevertheless! Jekyll (which runs this blog) uses liquid for variables and conditionals, which are super useful.

## General notes to myself

- stop forgetting to put the second `%` at the end of the brackets.

- the whole site will kinda break when you've messed some liquid up. Don't panic, just scroll up in the terminal and find the bug it identifies.

- all functions that come after a `|` get a colon before the argument

## Variables

Liquid is mostly useful because it's got all sorts of info stored within little libraries like `notes` and `pages`. For example:

`{% raw %}{{note.title}}{% endraw %}` will give the titles of pages, and helps to format things in `layouts` which determines, you guessed it, the layout of certain types of pages

`{% raw %}{{note.url}}{% endraw %}` will give the link to a note

`{{note.last_modified_at}}` is pretty nifty as well, but it's more useful when you append the `date:` function, which allows you to format things a bunch of different ways

## Conditionals and loops

---
### Sources, resources, links

Liquid's [documentation](https://shopify.github.io/liquid/)

One [source](https://www.tetchi.ca/liquids-capture-tag-and-numbers) for the string-to-number trick

A great [calculator](http://strftime.net/) for the funky date-time formatting.

A liquid [search function](https://shopify.dev/docs/themes/theme-templates/search-liquid) that I'd like to play with at some point