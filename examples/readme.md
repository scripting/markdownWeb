# Examples

<a href="https://github.com/scripting/markdownWeb/blob/main/examples/readme.md#notes">Notes</a> are at the end of the page. 

### Example 0

An untitled <a href="http://scripting.com/2024/03/31.html#a164241">blog post</a> from March 31, 2024, explaining how I had been using OPML to write and archive my blog writing starting in 2017.   

When rendered, this is what that Markdown text <a href="screenshots/rendered0.png">generates</a>.

<img src="screenshots/example0.png">

### Example 1

A <a href="http://scripting.com/2024/03/05/200550.html">titled blog post</a> from March 5, 2024 about some of my discoveries in creating art with ChatGPT.

<img src="screenshots/example1.png">

### Example 2

An untitled post with a <a href="http://scripting.com/2024/03/31.html#a161730">right-margin image</a>, a Good Humor ice cream truck. 

<img src="screenshots/example2.png">

### Example 3

A post with two <a href="http://scripting.com/2024/03/22/025201.html?title=vermont">inline images</a> about driving to Vermont. 

<img src="screenshots/example3.png">

### Example 4

A titled post with a list of four <a href="http://scripting.com/2024/03/15/015719.html">numbered items</a>. 

<img src="screenshots/example4.png">

### Example 5

A post with a <a href="http://scripting.com/2024/01/21.html#a194147">podcast enclosure</a>. Amazing that this makes it out to the front matter, but that's the power of simple standards. We just did what made sense, probably wouldn't have done it if it wasn't really easy. :-)

<img src="screenshots/example5.png">

### Example 6

<a href="http://scripting.com/2024/03/01/203935.html">First post</a> of the month, note that it wraps back to the previous month in the urlPrev value.  

<img src="screenshots/example6.png">

### Example 7

<a href="http://scripting.com/2024/03/12/120111.html">A bulleted list</a> and a value for description. Might be useful when displaying the story in a reader app. 

<img src="screenshots/example8.png">

### Example 8

This was the <a href="http://scripting.com/2026/10/22.html#a160031">most recent post</a> on scripting.com when the screen shot was taken. Note that there is a urlPrev value in the YAML text, but no urlNext. 

<img src="screenshots/example9.png">

### Notes

To start this project I took the OPML source for Scripting News, publicly archived <a href="https://github.com/scripting/Scripting-News/tree/master/blog/opml">here</a>, and had Claude write a utility app that converted it to markdown. We iterated over that app, and at the same time built a Markdown Browser, to guide us in getting the parts to fit together. 

We took screen shots of the Markdown for several example posts, hoping to illustrate a range of features. That's what you see on the page above.  

No documentation yet. 

Because I was doing all this work with Claude we were able to ask about prior art for all the stuff we're doing. We were guided in the choice of values for the front matter by two sources: <a href="https://github.com/scripting/oldSchoolBlog">Old School</a> which is the OPML-to-HTML rendering app I've been using for my blog since May 2017, and <a href="https://cyber.harvard.edu/rss/rss.html">RSS 2.0</a>, which has names for most of the metadata you might use for a post. Not a surprise, same thing happened when I was designing the <a href="https://xmlrpc.com/storyreader/story2198.md">MetaWeblog API</a>, it turned out we were just transporting RSS 2.0 items. 

We abide by the <a href="https://this.how/standards/">Rules for standards-makers</a>. We want to interop with everyone we can. Examples include: Jekyll, Hugo, Eleventy, Astro and Obsidian.

I'm not going to release our browser, I want to give others a chance to try out ideas, and get used to working with a fairly large base of posts. According to Claude there are over 16000 posts in the period between May 2017 and October 2026. I thought it was a typo and he meant 1600. ;-)

The <i>source</i> attribute (or front matter field) provides the address of the feed it came from. When displaying a post you might want to refer to some info from the feed, such as its title, link, icon.

The readme.md on this site has some philosophy you might want to read, and if you have questions or comments, use the Issues section. 

