# The Markdown web

Getting started with a simpler, safer and more efficient web for writers and readers. 

### Writers and readers

The goal is to create a simple web that works better for both writers and readers. 

* Writers have full control over the written word. They can link to other Markdown pages, locally or on other sites. They can use whatever editor they like for all their writing. 

* Readers have full control over appearance -- e.g. font, size, spacing, colors -- everything having to do with how text is displayed, so there is a consistency with stories written by all authors and that is totally determined by the reader. The software they use may hardcode the style, or offer whatever user-editable options they want. 

### Markdown and YAML front matter

We define YAML frontmatter that activates features in the browser we've made. If your files have the same concepts as ours, please use the ones we've defined for maximum interop.

We strip any HTML from the files. And front matter we don't understand is ignored. 

The YAML vocabulary we use comes from RSS 2.0, including title, author, pubDate, description, generator, source and enclosure. I've added others from the CMS we use or were invented for this application including urlPrev, urlNext, image, inlineImage, metaImage. 

We've found that there's a very good match between the metadata for feed items and written documents. Not exactly surprising, we keep running into this consistency everywhere we work in the written web. 

### Examples

To get the process rolling, I've prepared nine <a href="https://github.com/scripting/markdownWeb/blob/main/examples/readme.md">example Markdown web docs</a> for you to consider. No docs yet.  

They are all the Markdown versions of posts that appeared on Scripting News sometime between May 2017 and October 2026.

### Historic context

CSS was introduced to the web in 1996. 

JavaScript was introduced in 1995.

The original web as designed by Tim Berners-Lee was just for documents, and the same is true for the Web of Markdown.

Just for writing and reading. 

### Community

I first wrote about this on October 6 in <a href="http://scripting.com/2026/10/06/005559.html?title=webOfMarkdown">The Web of Markdown</a>. 

The next day <a href="https://andrewshell.org/2026/10/the-web-of-markdown/">Andrew Shell</a> got a browser working, and all of a sudden it feels like someone else got the excitement.

A few days later, Dirk Primbs <a href="https://unprompted.dirkprimbs.de/posts/engine-update-markdown.html">wrote</a> about using <a href="https://unprompted.dirkprimbs.de/llms.txt">llms.txt</a> to provide a list of Markdown files in a site, with links and short descriptions.  

I had already been playing around with ideas for a non-HTML web browser, I got excited about this idea and wrote the original post, but when I saw the excellent ideas that Andrew and Dirk had, I rolled up my sleeves and decided to get it working with the archived content of my blog between 2017 and 2026, a period when the format was standardized, and very little breakage (I did try out a few ideas that didn't go very far, I wouldn't carry those forward).

What I hope to do by starting this repo and sharing my progress is to get something that moves quickly. Interop is what it's about. And getting back to the original idea of the web as a place for writing and reading. 

### Where we're at

We've been working on software that implements this but wanted to put the <a href="https://github.com/scripting/markdownWeb/blob/main/examples/readme.md">examples</a> out first to see what people think.

It would be especially interesting to use this framework for a "social web" application like Twitter, Mastodon or Bluesky. Then we would have agreement over what text is, and the products could interop. In the indieweb world they call this POSSE. It would realize that goal. And allow us to easily write cross-application products.

Markdown defines a very good format for text on the web without all the dangerous stuff, and the front matter metadata we define can take care of the rest. Imagine a social web where you can use whatever writing tool you like and for reading you can tweak the display for maximum comfort and ease of use. 

We've made it work for blogging, but the same tech could be used for slides, code, whatever you can think of. 

And all the while writers can still use whatever tools they want, and readers get text that is readable in ways they like to read.  

CSS and JavaScript are only supported on the client side. Writers have no say in how it looks beyond simple styling -- bold, italic. And they can't create apps with logic, as would be implemented in JavaScript or another programming language. This is a medium for reading and writing only. But you are free to add scripting to your client. Some people would like to have the ability to build new products out of the basic capabilities of the web. 

Any Markdown file will work. But it does not do anything with HTML files. This is the web of Markdown, not HTML. 

### Notes

For more context see <a href="https://textcasting.org/">textcasting.org</a>.

Obviously we're going to make this work extremely well with RSS 2.0 and OPML. 

I also love WebSockets, so expect some of that as well. 

