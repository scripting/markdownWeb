# Examples of Markdown text with YAML front matter

How the pieces fit together in our web of Markdown files.  

### Writers and readers

The goal is to create a simple web that works for both writers and readers.

* Writers have full control over the written word, and can link the story with other pages on other sites, and give it an optional title, and use whatever editor they like for all their writing. After using the web for over 30 years, this is what I want, what I insist on.

* Readers have full control over font, size, spacing, colors -- everything having to do with how text is displayed, so there is a consistency with stories written by both of us. The software they use may hard-code the style, or offer whatever user-editable options they want.

We've been working on software that implements this, it's not ready to be deployed yet, but I wanted to share the basic principles of the project, provide examples that work, and field comments and questions.

We've made it work for blogging, but the same tech could be used for slides, code, whatever you can think of.

And all the while writers can still use whatever tools they want, and readers get text that is readable in ways they like to read.  

### Markdown and YAML front matter

Any Markdown file will work. It's the HTML of the Markdown web.

We define YAML frontmatter that activates features in the browser we've made. If your files have the same concepts as ours, please use the ones we've defined for maximum interop.

We strip any HTML from the files. And front matter we don't understand is ignored.

We use the nomenclature of RSS 2.0 for our front matter, but we plan to read the values put there by other popular software. We want the maximum interop possible.

Following are examples.

### Example 0

```
---
author: "Dave Winer"
pubDate: "Sun, 31 Mar 2024 16:42:41 GMT"
generator: "opmlToMarkdown v0.5.9"
urlPrev: "181216.md"
urlNext: "a161730.md"
---
```

I start a fresh outline for this blog on the first of every month, so tomorrow I will [archive](https://github.com/scripting/Scripting-News/tree/master/blog/opml) my blog.opml file on GitHub, start a new month, and delete the previous month. I've been doing that since 2017, when I finally forever gave up trying to interop with the great blogging silos (ie Twitter and Facebook mainly). I think outlining is like double-diamond skiing, but for writing.
