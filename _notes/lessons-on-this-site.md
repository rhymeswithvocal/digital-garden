---
title: Lessons from Building this Site
---
In the interest of doing some [[Learning in Public]] I've decided to log all of the lessons that creating and maintaining this jekyll blog teaches me.

Once again, a truly massive thanks to [Maxime Vaillaincourt](https://maximevaillancourt.com/) for use of his open source template that I'm using.

## Hard-learned lessons

- Keep careful track of your files. Especially if there's a different between `_pages` and `_notes` and you're trying to make changes show up in a particular file that you've accidentally duplicated into both of them.

- Similar to the above: if you need a particular filetype on your new posts in order for them to be read, make sure you use it!

- In markdown, the titles of pages need to come after a space, otherwise it'll break the whole site deploy.
	- turns out this is true of bullet points, as well!

- Giving pages titles that will fit naturally into other sentences makes back-linking a lot easier and better-looking

- The code that generates the back-links is sensitive! If you've got links on a page that aren't to another note, but contain within their url the name of another note, it'll think that you're linking that other note! (happened on this page with Max's `digital-garden` github linking to my note on [[Digital Gardens]])
	- There's something funny and meta to me about the fact that this page erroneously included a connection to the digital gardens page, but that error gave me a reason to include a real link to it.

- Do your testing on the localhost because even though netlify is free, you've got limited build minutes and you'll burn through them real fast troubleshooting.

- Hit save on your text-editor before you commit things to your git