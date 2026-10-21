# Examples

Ten Markdown files from my blog, each shown exactly as it is on the server, with a few words about what each one illustrates.

### Example 0: Untitled, plain text

The file is at https://dave.writersweb.org/2024/03/31/a164241.md.

* A post with no title: there's no `title` line, so the browser shows the author and date above the text and the tab says the first words of the text.
* `author`, `pubDate`, `generator` and the two arrows, `urlPrev` and `urlNext`, the lines every post has.
* `pubDate` is in RSS 2.0's date format, readable by people and by software.
* `urlPrev` and `urlNext` are relative to the file, the way links in HTML are; here both neighbors are in the same folder.
* The text is one paragraph of plain Markdown with one link.

```
---
author: "Dave Winer"
pubDate: "Sun, 31 Mar 2024 16:42:41 GMT"
generator: "opmlToMarkdown v0.5.9"
urlPrev: "181216.md"
urlNext: "a161730.md"
---

I start a fresh outline for this blog on the first of every month, so tomorrow I will
[archive](https://github.com/scripting/Scripting-News/tree/master/blog/opml) my blog.opml file on
GitHub, start a new month, and delete the previous month. I've been doing that since 2017, when I
finally forever gave up trying to interop with the great blogging silos (ie Twitter and Facebook
mainly). I think outlining is like double-diamond skiing, but for writing.
```

### Example 1: Titled, with paragraphs under it

The file is at https://dave.writersweb.org/2024/03/05/200550.md.

* `title` is in the front matter, not in the text; the browser draws it above the text and uses it for the tab.
* `metaImage` is the picture a social network shows when the post is shared; it isn't in the text.
* Images on a line by themselves are pictures with captions; the text in the square brackets is the caption, shown under the picture.
* Several paragraphs, nothing else special.

```
---
title: "How we learn to art"
author: "Dave Winer"
pubDate: "Tue, 05 Mar 2024 20:05:50 GMT"
generator: "opmlToMarkdown v0.5.9"
urlPrev: "171354.md"
urlNext: "201301.md"
metaImage: "https://imgs.scripting.com/2024/03/05/howWeLearnToArt.png"
---

People learn to make art by studying previous artists. Would we want it any other way?

Imagine if everyone had to reinvent everything that anyone had ever invented just to make something
new.

There is a lot of that in software, people won't put in an API so you have to rebuild the whole
house just to get a window.

We can make progress when people don't try to lock up their ideas.

Individuals live just a short time, we can't do that much in a lifetime, but we are an amazing
species, because we leave behind what we learn and we build.

![We learn by studying ourselves.](https://imgs.scripting.com/2024/03/05/selfportrait.png)

So why shouldn't our machines be able to learn too? They already can do things vastly more complex
than we can. We've invented a huge lever.

Science fiction tells us that we will lose control and be enslaved by our machines. I love those
stories, like the Matrix and Battlestar Galactica. But those are stories, they didn't happen. The
future is rarely so predictable. Things interact in unforseeable ways.

We're at dead-ends in climate and government. We need to make radical changes, and a fresh
invention as radically progressive as any that has come before is now in our hands.

![We're going to use it.](https://imgs.scripting.com/2024/03/05/weWillUseIt.png)

PS: I wrote the words, ChatGPT did the images.
```

### Example 2: Titled, with description and metaImage

The file is at https://dave.writersweb.org/2024/03/12/120111.md.

* `description` is a one-line summary; the browser shows it under the title, like a subhead.
* `urlPrev` reaches into the previous day's folder, `../11/`.
* A bulleted list, as the HTML-to-Markdown conversion writes it.

```
---
title: "AI and the NYT"
author: "Dave Winer"
pubDate: "Tue, 12 Mar 2024 12:01:11 GMT"
generator: "opmlToMarkdown v0.5.9"
urlPrev: "../11/a195157.md"
urlNext: "184321.md"
description: "How the NYT and other news orgs can create new products with their raw material --
news. "
---

Zach Seward, a friend from my days at [Harvard](https://www.niemanlab.org/about/) and NYU, got a
kickass
[job](https://www.nytco.com/press/zach-seward-is-the-newsrooms-editorial-director-of-a-i-initiatives
/), starting up the AI effort at the NYT. He's just the right guy for it. Young, curious, creative,
and very ambitious. And he has a strong startup journalism background. I couldn't think of anyone
I'd want more to be in this position.

Now that he's published
[notes](https://www.zachseward.com/ai-news-thats-fit-to-print-sxsw-2024/?ref=zach-seward-newsletter)
 for a talk he gave at SXSW, it's time to share some ideas I have for the NYT re AI.

*   Current events. This is something ChatGPT doesn't do. Not sure why. I'd like to be able to
connect to [ai.nytimes.com](https://ai.nytimes.com/) and ask it to give me a rundown on the
[lawyer](http://scripting.com/2024/03/09.html#a200615) who's testifying in Congress today about how
our president is "elderly." I don't want pointers to stories, though they should be included in the
response, I want a custom report, like the ones ChatGPT provides, that answers the questions I have
about the MAGA lawyer. Maybe the AI will just give me the story without the spin.

*   More useful NYT archives. When I was a kid I spent so much time at the [big
library](https://www.queenslibrary.org/about-us/locations/central-library) in Jamaica (Queens)
going back through microfilm of the NYT from before I was born. So far all we've done is replicate
the microfilm user experience (which is great and very useful) but the thing that ChatGPT does so
well is prepare custom reports. All that source material, used to answer very specific questions.
Answer questions like "has anything notorious happened in the neighborhood I grew up in, as far as
the NYT knows?"

*   Sell a service to your readers where you manage the archive of their blogs, and in doing so you
create a much broader archive for historians, journalists and others to study in the future, and,
in the context of AI, feed it all kinds of perspective on the time we live in. Maybe in the future
history won't be written by the winners (lotsa luck with that). Anyway, if at some point the NYT
and other journalism outlets will harness the energy, knowledge and intelligence of the readers,
why not start now?


I criticize the NYT a lot, I know. But that [means](http://scripting.com/2018/06/24/181734.html) I
care. When I stop criticizing you'll know that I've given up.

Alan Kay [said](https://www.azquotes.com/quote/707961) of the Mac, it's the first personal computer
worth criticizing. That's the spirit.
```

### Example 3: Inline pictures with captions

The file is at https://dave.writersweb.org/2024/03/15/135259.md.

* Two pictures, each on a line of its own: the browser shows each centered, no wider than 550 pixels, with its caption under it.
* The same post also has `metaImage` and `description`.

```
---
title: "Did you forget that quickly?"
author: "Dave Winer"
pubDate: "Fri, 15 Mar 2024 13:52:59 GMT"
generator: "opmlToMarkdown v0.5.9"
urlPrev: "015719.md"
urlNext: "a134635.md"
metaImage: "https://imgs.scripting.com/2024/03/15/whatKindOfMonsterIsThis.png"
description: "We tried letting Trump play president, we shouldn't have survived it, and in a lot of
ways we didn't."
---

We've noted this before.

Established facts about Trump eventually lose their currency, reporters forget and report it as big
news next time they see it happening.

Trump's [fealty](https://en.wikipedia.org/wiki/Fealty) to Putin for example. How could a reporter
forget that? Yet they seem to.

Two moments to bring you back.

![Picture 1.](https://imgs.scripting.com/2024/03/15/trumpBowsToPutinWhoGlowsWithPride.png)

![Picture 2.](https://imgs.scripting.com/2024/03/15/whatKindOfMonsterIsThis.png)

There are so many of these pictures.

Remember we tried letting Trump play president, we shouldn't have survived it, and in a lot of ways
we didn't.

Collectively we're like the main character in [The Sixth
Sense](https://en.wikipedia.org/wiki/The_Sixth_Sense) (no spoilers, but if you have seen it you
know what I mean).

So please, dear reporters and editors, try to factor actual proven facts into the context of your
reporting.
```

### Example 4: Image at the right margin

The file is at https://dave.writersweb.org/2024/03/31/a161730.md.

* An image at the start of a paragraph, with text following on the same line: the browser floats it at the right margin with the text wrapping beside it. That's the other image rule; a picture on a line of its own is a captioned picture.
* `image` names the same picture in the front matter.
* No title.

```
---
author: "Dave Winer"
pubDate: "Sun, 31 Mar 2024 16:17:30 GMT"
generator: "opmlToMarkdown v0.5.9"
urlPrev: "a164241.md"
urlNext: "a024813.md"
image: "https://imgs.scripting.com/2023/11/30/goodhumortruck.png"
---

![](https://imgs.scripting.com/2023/11/30/goodhumortruck.png)An advantage of using an outliner to
edit a blog, is that you can easily split one post into several because they're edited in one
document. Or move a paragraph from one story to another with drag and drop. In a page-oriented
editor, you get to focus on the writing for one page, but navigating outside that post is more
jarring, a writer more easily loses the train of thought. I've been
[writing](https://imgs.scripting.com/2024/03/31/outline.png) in an outliner almost exclusively for
decades, only now considering the writing world outside. Learning a lot.
```

### Example 5: Numbered list

The file is at https://dave.writersweb.org/2024/03/15/015719.md.

* A numbered list in Markdown, as the conversion writes it.
* `urlPrev` crosses into the previous day's folder.

```
---
title: "Four things about threads.net"
author: "Dave Winer"
pubDate: "Sat, 16 Mar 2024 01:57:19 GMT"
generator: "opmlToMarkdown v0.5.9"
urlPrev: "../14/a024428.md"
urlNext: "135259.md"
---

Four things.

1.  We're selling ourselves out by letting Facebook own a new social network and not putting that
energy into building something that preserves our choice.

2.  I understand that Facebook's claims of supporting the Fedisphere won't amount to anything. They
will end up controlling what interop means, which means we end up with yet another app store, with
all the nonsense that comes with. Welcome to CyberDisneyland.

3.  You know all this, as well as I do. But we have decided not to care.

4.  This is exactly how we snookered ourselves into using Twitter for 17 years.
```

### Example 6: A glossary substitution in the text

The file is at https://dave.writersweb.org/2024/03/11/124703.md.

* The writer typed `feedland.com`; the glossary turned it into a link before the Markdown was written. The file has the link; nothing in the file says where it came from.
* The glossary belongs to the writer's tools, not to the browser.

```
---
title: "Oh servers!"
author: "Dave Winer"
pubDate: "Mon, 11 Mar 2024 12:47:03 GMT"
generator: "opmlToMarkdown v0.5.9"
urlPrev: "../10/a015710.md"
urlNext: "a121116.md"
---

The other day I wrote proudly that we had better more reliable server software in 2024 than we did
the first time we bootstrapped blogging communities.

And then this happened...

We've been having serious problems on [feedland.com](https://feedland.com/) since Friday when I
made a software version mistake. At first it caused the server to crash when you tried to subscribe
to a new feed, so you'd get an awful error message, either from the FeedLand website, or the
browser, saying the server had gone away. I quickly fixed that problem and another, and restored
the server to some basic functionality. But when I did some work on my account over the weekend, I
saw that there were new errors. And then noticed that none of my feeds had updated since March 8,
they still haven't.

We're going to fix it this morning, by reverting the server software to the version as it was
before the update, and the server should return to its previous reliability, Murphy-willing. Then
we're going to upgrade the database, and then install the new software, and try again. That won't
happen today and probably not tomorrow.

Most people probably don't know that feedland.com is a project I'm doing with Automattic. It's
running in their cloud. This system should be able to scale up in ways that a Digital Ocean droplet
can't, where feedland.org and the new feedland.social are running. So when there are many thousands
of users, we should be okay. That's why I did the work to convert FeedLand so everything is stored
in the SQL database, and nothing in the file system, among other changes that had to be made last
year, like getting off Twitter for identity. That was not much fun, but it had to be done.

Anyway I am very sorry and embarrassed for the unreliable performance on our main server in the
last few days. I can't promise it won't happen again, but we learned a lot in this experience, and
in some cases re-learned.

It's even worse than it appears and as they say -- still diggin!
```

### Example 7: Podcast, with an enclosure

The file is at https://dave.writersweb.org/2024/01/21/a194147.md.

* `enclosure`, `enclosureType` and `enclosureLength` are RSS's enclosure, split into three lines: the address, the type and the size in bytes.
* `urlNext` crosses into the next day's folder.
* One line of text with a link to the audio.

```
---
author: "Dave Winer"
pubDate: "Sun, 21 Jan 2024 19:41:47 GMT"
generator: "opmlToMarkdown v0.5.9"
urlPrev: "a162425.md"
urlNext: "../22/a153158.md"
enclosure: "http://scripting.com/2024/01/21/typicalTechIndustryMess.m4a"
enclosureType: "audio/mpeg"
enclosureLength: "6374173"
---

[Podcast](http://scripting.com/2024/01/21/typicalTechIndustryMess.m4a): ActivityPub is a typical
tech industry mess. 12 minutes.
```

### Example 8: First post of a month

The file is at https://dave.writersweb.org/2024/03/01/203935.md.

* `urlPrev` reaches back into February, `../../02/29/`, so the arrows run across months and years without a gap.
* Three captioned pictures in a row.

```
---
title: "I see the bright lights of Memphis"
author: "Dave Winer"
pubDate: "Fri, 01 Mar 2024 20:39:35 GMT"
generator: "opmlToMarkdown v0.5.9"
urlPrev: "../../02/29/a205257.md"
urlNext: "145758.md"
---

My friend Brad Pettit is playing with ChatGPT's image drawing capability, and had a brilliant idea,
feed it the lyrics to a song and see what it comes back with. He tried [Low Spark of High-Heeled
Boys](https://www.youtube.com/watch?v=vDGorIWYz-A) by Traffic, a great song, and [the
image](https://www.facebook.com/bradpettit/posts/pfbid0m7TE3T5LJVr9Z5QznWdtWPS9bJxrXKnw1NX3UCeUtpqcg
9Sg6SiNphqk7Cg7dKCel) was really cool.

This game me the idea to try it with a few of my favorite songs.

![Dixie Chicken](https://imgs.scripting.com/2024/03/01/dixieChicken.png)

![A Apolitical Blues](https://imgs.scripting.com/2024/03/01/aapoliticalblues.png)

![Call Any Vegetable](https://imgs.scripting.com/2024/03/01/callAnyVegetable.png)
```

### Example 9: The newest post, no next

The file is at https://dave.writersweb.org/2026/10/20/a124722.md.

* No `urlNext`: this was the newest post when the page was made, so the browser shows no right arrow. When the next post is written, this file is rewritten with a `urlNext`.
* `generator` says which version of the build program wrote the file; a file is only rewritten when its content changes, so the version tells you when the file last changed.

```
---
author: "Dave Winer"
pubDate: "Tue, 20 Oct 2026 12:47:22 GMT"
generator: "opmlToMarkdown v0.5.10"
urlPrev: "a121241.md"
---

[Today's song](https://www.youtube.com/watch?v=SqRvJLH_-vU), for the Knicks. "And when the morning
light comes streaming in I get up and do it again." _Knicks in 5!_
```
