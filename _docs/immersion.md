---
title: Immersion
permalink: immersion.html
published: false
---

## Action 3: Allow navigation within content

Although the sidebar is important for seeing the whole, it's also important to build navigation inline within the sentences of your content itself. Users tend to navigate by clicking links inline rather than via the sidebar. I added links where appropriate in my content.

<img src="images/amazoninlinelinks.png"/>

### Design principle: Immersion

The design principle at work here with inline links might be considered immersion.

<img src="images/wtd_doc_navigation_dontleavesystem.svg"  class="vectorStyle"/>

<div class="bs-callout bs-callout-primary"><b>Immersion:</b> "A state of mental focus so intense that awareness of the "real" world is lost, generally resulting a feeling of joy and satisfaction." &mdash; [Universal Principles of Design](https://www.amazon.com/Universal-Principles-Design-William-Lidwell/dp/1592530079)</div>

Although immersion mostly refers to removing distractions from the outside world so the user can become engrossed within a system and forget the outside world, there are ties with documentation here. Users desire to be immersed in the application or system they're using rather than leaving that system to consult a separate, external system for help. Users usually feel like going into the help detracts them from the focus and progress toward their goal.

The first way to cater to immersion is to bring the help to the user. Don't require users to go to the help &mdash; through context-sensitive features and other on-screen text, bring the help to the natural location where users are at.

Of course this assumes there's a user interface for you to push the help. With developer docs, the help might best appear in the form of code comments, error messages, man[ual] pages in the terminal.

But even when a user goes to your help system, the principle of immersion still applies. Users consuming content prefer to stay within that content of the page rather than move back and forth with a sidebar nav, which exists somewhat "outside" of page content.

<img src="images/wtd_doc_navigation_usersclickinlinelinks.svg"  style="border: 1px solid #dedede;"/>

Immersed in a topic, users are more apt to click and navigate using the links within the topic itself. As such, you should also provide navigational controls within the content rather than assuming all doc navigation will take place through the sidebar nav.

### Bottom-up navigation

The idea of navigating from within your content is called "bottom-up navigation" (rather than "top-down navigation," where users would drill down into the content through hierarchies at the top, often abstract/general level). Bottom-up navigation is a principle that Mark Baker emphasizes on his site [Every Page Is Page One](http://everypageispageone.com/2015/02/10/bottom-up-information-architecture-q-and-a-part-1/).

Although Mark describes bottom-up navigation in more articulate, abstract ways in his posts and book, I like the down-to-earth description he gives in a [comment on one of my posts](http://idratherbewriting.com/2017/05/01/write-the-docs-podcast-episode-5-where-do-we-belong/#comment-3286566056). What does bottom-up navigation mean?

<blockquote>
<ul>
<li>If you tell me I can do something, link to how to do that something.</li>
<li>If you tell me I can use something, link to a description of that something.</li>
<li>If you mention a concept or an idea, link to a description of that concept or idea.</li>
</ul>
</blockquote>

These principles may seem like commonsense. In general, we link to topics as it makes sense to do so. But bottom-up navigation takes inline linking to a another level. Consider amplifying the number of links by two or three times the amount so that your pages begin to resemble the inline links in a Wikipedia article.

<img src="images/wikipedia.png"/>

Admittedly, I haven't amplified the number of links that Mark suggests. I would need to increase these links by about 5 times the amount I currently have.

Amplifying the number of inline links create some challenges:

* It can be hard to author content when your text is littered with links. (If using Markdown, use [reference style linking](https://daringfireball.net/projects/markdown/syntax#link) that uses a variable inline to reference a URL at the end of your content.)
* As you rename files, page titles, and headings, the links can easily break or list the wrong page titles.
* Inline links create decision points in your content that force users to decide whether to continue reading or to jump to a new topic. This can result in users jumping around more in your content, which might [reduce readability and increase documentation fatigue](http://idratherbewriting.com/2010/06/19/finally-convinced-about-removing-inline-links-to-increase-readability/).

Even with these challenges, don't neglect or minimize inline links. They're how many users simply navigate content. Why? The web has driven this behavior into our brains.

## How the web has taught us to navigate

The web teaches us navigate through inline links way because our searches typically follow this pattern: we google something, land on a page, become dissatisfied, jump back to google's results, click to another page, click links within the page, possibly move back to the search results, and then move to another page as we search for the right information.

Even if we don't *always* operate in this mode, the many times we do operate in this mode condition us to act this way even when we're not on the web. We rarely navigate via the sidebar because we're so used to *jumping across different websites* (clicking back and forward on different google results) instead of moving within the same system using a logical sidebar.

This kind of hit-and-miss navigation through keyword searches and search results pages is jumpy and nauseating in the long run, but because we have internalized the behavior as part of an Internet culture, we can't neglect this design pattern in our help material. Instead, we should build links into our content to help users navigate.
