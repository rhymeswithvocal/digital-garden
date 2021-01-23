---
title: Lessons from Building this Site
---
In the interest of doing some [[Learning in Public]] I've decided to log all of the lessons that creating and maintaining this jekyll blog teaches me.

Once again, a truly massive thanks to [Maxime Vaillancourt](https://maximevaillancourt.com/) for use of his open source template.

## Hard-learned lessons

- Keep careful track of your files. Especially if there's a different between `_pages` and `_notes` and you're trying to make changes show up in a particular file that you've accidentally duplicated into both of them.

- Similar to the above: if you need a particular filetype on your new posts in order for them to be read, make sure you use it!

- In markdown, the titles of pages need to come after a space, otherwise it'll break the whole site deploy.
	- turns out this is true of bullet points, as well!

- Giving pages titles that will fit naturally into other sentences makes back-linking a lot easier and better-looking

- The code that generates the back-links is sensitive! If you've got links on a page that aren't to another note, but contain within their url the name of another note, it'll think that you're linking that other note! (happened on this page with Max's `digital-garden` github linking to my note on Digital Gardens)

- Do your testing on the localhost because even though netlify is free, you've got limited build minutes and you'll burn through them real fast troubleshooting.
	- Actually, it turns out that the build minutes are tracked monthly, and there's basically no way you could use them all up in that time, so go nuts!

- Hit save on your text-editor before you commit things to your git 😑

- Sublime text has a spell-check! It's activated on a by-tab basis by hitting F6

- Trying to remember and stick to a personal style guide re:headings, capitalization, etc. is difficult, so it'll probably be easier long-term to just go with whatever feels right, and over time there will probably be some consistency/consensus

- The most joyous part of publishing this blog has to be watching the map on the homepage reconfigure itself, which is great because it incentivizes creating notes that are related to many others, and creating copious links

- I! Need! To! Save! More! Links! I keep losing awesome blog content from other folks' gardens because I think "oh that's neat I'm sure I'll find it again" and then I absolutely do not. It's lost forever. Major bummer. I think the solution is to be willing to have more notes that are basically **only** a collection of links. I can circle back to them later and add my own thoughts.

- You can search all the files within a folder in Sublime Text by hitting `cmd-shift-F`