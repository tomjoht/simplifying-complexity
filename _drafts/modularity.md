---
title: Modularity
permalink: modularity.html
published: false
---

### Design principle: Modularity {#modularity}

The design principle behind consolidating information into longer, more complete topics is modularity.

<img src="https://idratherbewritingmedia.com/images/simplifying-complexity/wtd_doc_navigation_modularity.svg"  class="vectorStyle"/>

<div class="bs-callout bs-callout-primary"><b>Modularity:</b> "A method of managing system complexity that involves dividing large systems into multiple, smaller self-contained systems." &mdash; [Universal Principles of Design](https://www.amazon.com/Universal-Principles-Design-William-Lidwell/dp/1592530079)</div>

Applying modularity to documentation means breaking up content into independent topics that can be viewed, understood, and updated independent of the whole. A topic or chunk should not be so interconnected with the whole that it cannot stand on its own.

Modularity also provides efficiencies for the authors, because it means we can work on an individual part without having to adjust the whole.

### Users read non-sequentially

Modularity in documentation has some of its origins with John Carroll, who argued that users should not be required to read the whole manual but instead be encouraged jump around to the topics they're interested in. Carroll explains:

> You can just read the sections about the tasks you want to do. <br />
&mdash; John Carroll, <a
href="http://faculty.washington.edu/farkas/dfpubs/Farkas-Williams-CarrollsNurnbergFunnel.pdf">The Nurnberg Funnel</a>

Because users skip around and are impatient to act, we have to design our help material to support entry at any point. Help topics that are modular can stand alone and function as independent entities without requiring users to read a lot of before-or-after topics to make sense of the content.

Usually when you create standalone, modular topics, the topics end up being somewhat long. Don't be afraid of long topics. Some Wikipedia articles are so long they could be printed as ebooks.

<img src="https://idratherbewritingmedia.com/images/simplifying-complexity/wtd_doc_navigation_topiclength.svg"  class="vectorStyle"/>

Most of us agree with this modularity in theory, but it's hard to implement in practice, in part due to the information structures we may be following.

### Don't assume building blocks == presentation

You may be writing in a documentation structure that separates content into tasks, concepts, and reference topics. If so, remember that these structures are a way of chunking content so you can re-use it. The re-use reduces your word count, lowers translation costs, avoids duplication, and provides other efficiency benefits.

However, remember that these information chunks are *building blocks only*. Like legos, you can arrange the blocks into more lengthy creations.

<img src="https://idratherbewritingmedia.com/images/simplifying-complexity/usercentered_buildingblocks.svg"  style="border: 1px solid #dedede;"/>

You aren't required to have a two-sentence topic that stands as its own page because it's a concept. You don't need a topic that is just 3 steps and nothing more because it's a "task." Users don't think in terms of topic types but rather goals and problems.

If you fragment your information into a [million little content pieces](https://idratherbewriting.com/2013/04/22/does-dita-encourage-authors-to-fragment-information-into-a-million-little-pieces/), you force users to jump around from topic to topic, like a pinball bouncing off of different side walls and backstops, looking for the information they need. That design leads to a disjointed, tiring experience. Instead, combine these chunks into more comprehensive "articles."

Continuing with more analogies, consider each chunk of content as a rock. You can certainly store and manage the rocks as individual chunks. But if you want to convey meaningful information to users, stack the rocks into various combinations to create more elaborate and purposeful displays.

On trails in the wilderness, these stacks of rocks are called "cairns" and serve as guide posts to users on trails that often lack clear boundaries or pathways.

<img src="https://idratherbewritingmedia.com/images/simplifying-complexity/cairns.png" style="vectorImage"/>

Not all help information can stand <i>entirely</i> on its own. Frequently one concept or task builds on another topic, or requires knowledge of another topic. But there's usually a logical boundary line between topics. You can decide how large to draw the boundaries.

When content becomes unwieldy or hard to follow because it's all listed on the same page, break it up into multiple pages. Just make sure your users aren't bouncing from one topic to another trying to get answers for a single task or goal they're trying to achieve.

Although I shy away from actual word count numbers, I think a good-sized page can range anywhere from 800 to 3,000 words. It mainly depends on whether the topic is complete. Beyond 3,000 words, I usually start chunking the information. But again, these are rough word counts. How much information you can fit into a page depends on the navigation mechanisms on your site.

### Going overboard with modularity

It is possible to go overboard with modularity. In [version 3 of Bootstrap's component documentation](https://getbootstrap.com/components/), the authors listed all components on the same page. As a result, the content was approximately 8,000 words long.

In [version 4 of Bootstrap's component docs](https://v4-alpha.getbootstrap.com/components/alerts/), the component documentation is more broken up. For example, this [doc page on alerts](https://v4-alpha.getbootstrap.com/components/alerts/) has just 800 words. I don't know the reasoning behind Bootstrap's documentation decisions, but it's clear that they felt the previous organization in putting all content on the same page had some downsides.
