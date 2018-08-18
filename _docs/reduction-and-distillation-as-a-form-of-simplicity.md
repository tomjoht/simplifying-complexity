---
title: "Principle 4: Reduce and distill information to its essence"
permalink: reduction-layering-distillation.html
redirect_from:
 - /reduction-as-a-form-of-simplicity.html
 - /hiding-complexity.html
---

{: .principle}
Layering information on your site (reducing it in places and expanding it in others) can help simplify complex topics. Also, distilling large amounts of information into concisely worded titles, summaries, headings, mini-TOCs, and topic sentences can facilitate information consumption and comprehension. Quick reference guides can also help users internalize vast information quickly. When you can't reduce information, you can hide it.

* TOC
{:toc}

## The focus here is on distillation, not integration

In the previous article, [Ensuring information harmony in the larger documentation landscape](https://idratherbewriting.com/simplifying-complexity/ensuring-information-harmony-in-the-larger-documentation-landscape.html), I argued for the importance of integrating new information into a larger documentation landscape. I explained that it's easy to create a new article and publish it to a documentation site but much harder to assess whether the new information harmoniously fits in with all the other information on a site (not just harmony with other docs, but with existing forum posts, blog posts, and other information assets). Integrating a small piece of information into a larger body of information requires wide reading and information analysis to determine information fit and harmony.

Conversely, the opposite activity &mdash; taking an existing body of information and distilling its essence down into a smaller information unit (whether that smaller unit is a title, overview, heading, topic sentence, quick reference guide, or some other compressed form of information) also requires cognitive prowess. Crystalizing large information into a brief distillation that captures the main point in as little a space as possible can be a difficult skill that rivals a poet's astuteness with language and articulation. Despite the difficulty with the task, this distillation is worth it as it can go a long way towards simplifying a complex system.

<figure><img class="medium" src="images/distillation_and_integration_distillation.svg"/><figcaption>Distilling a summary from a larger body of information requires you to compress a high amount of meaningful information into a small space. </figcaption></figure>

## Reducing information bloat

In the [Laws of Simplicity](http://lawsofsimplicity.com/), John Maeda explains that reduction is the easiest way to simplify complexity:

> The process of reaching an ideal state of simplicity can be truly complex, so allow me to simplify it for you. The simplest way to achieve simplicity is through thoughtful reduction. When in doubt, just remove. But be careful of what you remove. (See [Law 1: Reduce](http://lawsofsimplicity.com/los/law-1-reduce.html))

Maeda isn't specifically focusing on documentation in his book, but rather speaking generally, such as with product design. If your TV remote control is too complex, reduce its number of buttons. Reduction simplifies the user experience because it removes the number of choices.

With documentation, the tech writer's first task is usually to translate descriptive information into concise, actionable steps that align with the user's goals. This work usually involves reducing the amount of information, whittling it down to the bare bonds of actionable steps. Mike Hughes captures this perfectly in this short graphic:

<figure><img src="https://idratherbewriting.com/images/actionableinformation.png"/><figcaption>Hughes argues that technical writers don't just fix grammar and format information; they actually create new knowledge assets that become the lifeblood of the company's success. Many times, the knowledge assets reduce information bloat from engineers. See "Moving from Information Transfer to Knowledge Creation: A New Value Proposition for Technical Communicators" (Technical Communication, 2002)</figcaption></figure>

When some engineers write, they have a tendency to over-explain the details of how something works, rather than providing the minimal amount of information the user needs to accomplish their task. For example, an engineer might explain the intricacies of architecture and design even though the user just wants to know which button to press. Reducing the information that falls outside of the user's task needs is usually the first step a tech writer takes to simplify content.

Reducing information bloat is actually a byproduct of minimalism, a concept put forward introduced by John Carroll. Carroll's emphasis on action-oriented instructions usually results in a reduction of secondary, non-task-based content in docs. Hence, the docs end up being briefer due to the task-based focus. In a recent *Intercom* interview, Carroll explains:

> ...brevity is more a consequence of minimalism than a principle of minimalism. If you go back to what I was saying earlier about trying to facilitate the learner’s initiative and goals and aspirations and impede them less, you will most likely end up with a briefer design, or it might be layered. ([Minimalism Revisited: An Interview with John Carroll](https://www.stc.org/intercom/2013/03/minimalism-revisited-an-interview-with-john-carroll/), *STC Intercom* March 2013)

In other words, by focusing on the information users need to complete a task, tech writers often reduce the other fluff that is unnecessary. We carve this information away to let users focus on the information they need to complete a task. What happens to the other information? If it's not eliminated, it sometimes gets layered at secondary or tertiary levels, as I'll explain in the next section.

## Progressive disclosure to hide secondary information

The effort to simplify complexity by reducing content can be too extreme. It can, at times, be counterproductive for users. Have you ever ordered a product and found that it doesn't come with any instructions? Or if it does, the simple one-pager included in the box is hopelessly insufficient for your goals, and so you end up being even more frustrated? I have a pair of Bluetooth headphones that, in the name of simplicity, have minimal documentation. I think the product owners wanted to convey to users that they just need to turn the earbuds on and pair them &mdash; an easy, simple, hassle-free experience!

But in my experience, sometimes one earbud pairs and not the other; sometimes turning one off turns the other off as well. Sometimes one earbud won't connect even when the other is connected. It's unclear if pairing mode is required for both earbuds or just one, and so on. I would gladly welcome more detail about how these mysterious Bluetooth earbuds work.

Rather than delete the extra information, tech writers often shift information around. We decide to put secondary information in less visible spaces &mdash; perhaps in collapsed sections, or in less visible topics (the equivalent of footnotes in an academic paper). Carroll refers to this as "layering" the information. Others call it "progressive information disclosure." It's the idea that different information should be made available at different layers in a system, or that information can be revealed to the user little by little (instead of all at once).

Perhaps at the end of a topic, users might see a link for more info that takes them to another section where the architectural intricacies are explained, or where they can read the details about the many path options they can take, or maybe they find information for older versions or techniques for older API levels. Commonly, in user interfaces, a tooltip provides some brief detail followed by a Learn more link where the additional information appears. Here's an example from the WordPress UI:

<figure><img src="images/wordpress_pd.png"/><figcaption>The WordPress UI shows an example of progressive disclosure: The user sees some information in the UI followed by a link for more detail if desired.</figcaption></figure>

Web designers often consider progressive information disclosure in deciding how to layer information on a website. A website might begin with a few large category choices on the homepage. At the second level (which appears after users select a homepage category), more information is presented. At the third-level, additional information is made available, and so on. But you don't overwhelm the user with all information choices up front. The same layering strategy can be used directly in documentation (not just in user interfaces or commercial sites).

(By the way, I'm not a huge fan of the term "progressive information disclosure." I prefer the term "layers" or "progressive information detail," since "disclosure" suggests that you find out unwanted or negative information little by little. Like a doctor who lets you know little by little the details of a debilitating disease, or an insurance agent who slowly explains what is not covered, or a kid who wrecked his or her parent's car and slowly discloses that he not only dented the bumper, but also took out the neighbor's fence, injured a dog, and broke one of the windows ... and lost the keys ... and was slightly intoxicated ... and also failed a math test.)

While progressive information is a valuable principle for UX, it's not exactly reduction. It's more like "information re-organization." Sure, we reduce information in places and expand it in others, but we still have the same amount of information. True information reduction is an act of reducing the amount of something. At any rate, deciding *where* to reduce information and where to expand it is a useful skill to develop.

## Keeping the sidebar navigation consumable at a glance

Most tech writers will readily agree with the concept of layering or progressive disclosure but then create a sidebar navigation for their docs that contains hundreds of topics in deeply nested folders. When deciding on where to reduce/re-organize information, my preference is to keep the sidebar navigation **consumable at a glance**. I don't try to pack every topic in the documentation in the sidebar, making it a massive navigation tree that users can expand and collapse all afternoon. This runs counter to the purpose of the sidebar navigation.

What exactly is the purpose of the sidebar navigation? Surprisingly, its job isn't so much to facilitate navigation (users still get to topics via search). Instead, the sidebar serves a psychological / cognitive need. One of the first steps in unraveling complexity is to break complex systems down into a list of numerable parts. The sidebar provides this list of parts that users can view. If there are too many parts listed to be meaningful to users, break up these parts into several distinct sidebars.

<figure><img src="images/wtd_doc_navigation_listofparts.svg"/><figcaption>Breaking down complex systems into a list of parts helps us understand the complexity better. The sidebar in a doc set essentially acts as a list of parts that help users make sense of a larger, more complex system.</figcaption></figure>

When the sidebar is consumable at a glance, it helps users understand all the parts that make up a complex system. I typically give each product its own sidebar (usually one product has between 25-75 topics). Below the sidebar, links for related doc sets allows users to select another product and its sidebar. Again, by providing users with information consumable at a glance, they can see the big picture of the system and better understand how each part fits together. Additionally, because the sidebar shows a hierarchical grouping of the parts, the sidebar can help users understand the system as a whole.

## Distillation of information

Now let's move on from progressive information / layering strategies to **information distillation**, which is actually more useful. Distillation is not necessarily information elimination or re-organization. Distillation involves compressing meaning into a shorter space. When you distill the meaning of a section into a descriptive section heading, you aren't eliminating information but rather distilling the main point into a short phrase and allowing readers to consume the information at a glance.

A good structure in a doc page usually provides a title, summary, headings, mini-TOC, and topic sentences that lets users take in the information at a glance rather than reading the content line by line. These elements are simple, but they are the bread-and-butter of information usability. Let's go into more detail for each element.

### Titles

A title should capture the essence of the information in a clearly understandable way. Titles should not be vague or fuzzy but should communicate as much as possible in as little space as possible. The title must broadly convey the main point of the content. The title probably has the most influence on the content's visibility in Google, so the title must not only communicate meaning but do so using the keywords a user is looking for.

### Summaries

The summary provides several sentences that capture the content in the document and compresses it into a brief paragraph. In DITA, this element is the `shortdesc`. The short description of a document can act as metadata for the entire content, and it's much more portable and usable than the entire document. (For example, a section overview might list summaries of all pages in that section, providing the user a good sense of what that section contains at a high level. You can see an example here in the [Roku developer documentation](https://developer.roku.com/develop/guides).). The summary lets the user know if the information promised in the title is indeed the information the user wants in the document. In other words, the summary elaborates more on the title and main ideas in the topic.

A couple of years ago, while browsing information on [Jakob Nielsen's site](https://www.nngroup.com/articles/), I became converted to the benefit of summaries in content. Seeing this summary allowed me to quickly process whether the article contained the information I was looking for.

<figure><a class="noCrossRef" href="https://www.nngroup.com/articles/moderated-remote-usability-test/"><img src="images/nielsonsummaryexample.png"></a><figcaption>A good summary lets you know immediately what the content is about and whether it matches your information needs.</figcaption></figure>

In almost all my blog posts, you see a short summary at the top that usually tries to capture the main point of the article. On this Simplifying Complexity site, I've put this information into a "Principle" at the top.

The summary is arguably the most important part of the entire topic because most articles have a high bounce rate and short view time from visitors. A user clicks the title, thinking the content would answer his or her needs, and then quickly jumps to another page after scanning the content. In the digital age, users jump from one document to another looking for the right information. In fact, a Time, Inc study found that "Consumers in their 20s (‘digital natives’) switch media venues about 27 times per nonworking hour—the equivalent of more than 13 times during a standard half-hour TV show" ([The Evolving Role of the Technical Editor](https://www.stc.org/intercom/2012/09/the-evolving-role-of-the-technical-editor/), *STC Intercom*, Sep 2012). The summary provides an efficient way for users to judge whether they're on the right page.

Interestingly, this summary is one of the hardest elements to write. I've been including summaries on my blog posts for a while, and it is extremely difficult to compress meaning into a few sentences that describe the whole in a useful, informative way. The ability to reduce a large amount of information into a few sentences that distill the meaning in a clear way is a skill that few possess. The more topics and ground your content covers, the harder the summary is to write. In fact, if your content doesn't have a clear focus, it will be nearly impossible to write a summary.

Also, after working for so long on the content body, we're usually ready to be done with it, so this most important element often doesn't get the attention it deserves.

### Section headings

Section headings also incorporate the same principles as the title and summary but on a section-by-section level. Each heading should neatly capture the essence of that section in a way that, if the reader didn't read the section, he or she could still get the gist of the content. A reader should be able to glance through the section headings and understand the gist of the content.

All too often, section headings are meaningless verbiage, their only real purpose to provide some structural division of the content. A good heading is hard to write because it forces you to clearly identify the main point of that section. As with the summary, the section heading is hard to write if the main point of that section is fuzzy or wanders in multiple directions.

I was recently editing some content an engineer had written. I added headings on a variety of sections and then attempted to distill the point of each section into the heading. He said I'd made the headings technically inaccurate, and changed them back to more general titles. When I asked him to sharpen the headings to capture the point of the paragraphs below each heading, he said it wasn't possible. He said a user will just need to read the details to understand that section.

I lost this battle, but the experience underscored the challenge of writing good headings. It's not easy to capture the meaning of a larger body of information in a small, tight space where you only have 10 words or so, especially when one small shift in the heading might make the content inaccurate on a technical level. For more on headings, see my post [Subheadings: Perhaps the Most Useful Technique in Technical Writing](https://idratherbewriting.com/2013/08/23/subheadings-perhaps-the-most-useful-technique-in-technical-writing/).

### Mini-TOC (table of contents)

The mini-TOC simply pulls together all headings on the page and provides the user with a quick summary of the page's contents. This quick summary lets the user see more detail about what the page will cover, without scrolling down the page to read each heading section by section. If the headings are good, the mini-TOC should informative and helpful.

Beyond just consolidating the headings, the mini-TOC establishes the relationships between headings. Nesting headings inside other headings (creating hierarchy) tells the reader how the information is related. Hence, the mini-TOC helps increase the meaning of the section headings and lets the user understand how the information in each section fits together.

While analyzing a topic's mini-TOC, you may find that some headings should be grouped. Just as a single task with too many steps can be improved by breaking it into multiple tasks, a long list of h2 headings should be broken up into some h3 headings and grouped. Lists alone don't tell us the relationship between the sections except that they're related. But if some headings are hierarchically arranged in groups, this grouping provides cognitive meaning to the user and makes the content as a whole easier to consume.

### Topic sentences

Finally, topic sentences are also an important information usability technique. When I'm scanning a document, I often read the first sentence of each paragraph. When the writer has a clear focus, topic sentences come naturally. Topic sentences apply more to conceptual and narrative information than task-based information, but they're still worth noting here.

{{site.data.alerts.note}}The whole process of distilling information into a title, summary, headings, and topic sentences is a form of layering or progressive information. The user starts with the title, and if interested in more information, reads the summary. If the user wants more detail, the user reads the headings in the mini-TOC. If the user wants more detail, the user usually jumps into that section and reads the topic sentence. I realize these mechanics are the basics of good technical documentation, but they are overlooked and often done poorly. They are also not always described as a method for progressive information disclosure.{{site.data.alerts.end}}

## Quick reference guides

One final, key deliverable for compressing information is the quick reference guide. A quick reference guide provides a 1-2-page guide (in an attractive magazine-style layout) that provides a brief summary of the core tasks and features in the system. Here's an example:

<img src="images/watershed6101.png"/>

The quick reference guide should provide the user with just enough information to get the gist of what the system is about, how to do key tasks, and get going. Almost invariably, you write the quick reference guide near the end of your documentation project, when you can see the whole and compress it accordingly.

The information in the quick reference usually can't be single sourced, since it's not just an excerpt from the docs but rather a more briefly written summary of the entire system. As a result, many times it seems like yet another deliverable we don't have time to write. But for the best user experience, the quick reference guide provides incalculable value to users.  

I've written quite a bit about quick reference guides before. See [Quick Reference Guides](https://idratherbewriting.com/quickreferenceguides/) for a list of articles. Probably the best article is [Quick Reference Guides: Short and Sweet Documentation](https://idratherbewriting.com/2009/04/10/quick-reference-guides-short-and-sweet-documentation/).

## Minimal viable documentation

I'd like to mention one more strategy related to information reduction, layering, and distillation: minimum viable documentation. Technical writers usually care deeply about documentation and prefer it to be thorough and complete, answering all users' questions. As a result, it's hard to even contemplate a strategy of minimum viable documentation. But let's start with the idea of a "minimum viable product."

The idea of pushing out a minimum viable product is that, because products are hard to develop, you want to get a lightweight product out there for users to test, and then iterate based on the feedback. This is the whole idea of agile. Through the constant feedback and iterative development, you ensure that you're building the product in a way that users want (rather than building the product in a vacuum for two years and then emerging for the first time to show it to users, only to find that you went off course long ago). You can read more about minimum viable products in this [WTD write-up on minimum viable documentation by Andrew Spittle](http://andrewspittle.com/2014/05/05/write-the-docs-matthew-lyon-minimum-viable-documentation/) and [Matthew Lyon's talk](https://speakerdeck.com/mattly/minimum-viable-documentation-write-the-docs-na-2014).

Applying the same principle to docs, we could say that docs are hard to write. How do we know that we're even creating the right information &mdash; the information that users need, the questions they're asking, addressing their actual problems? We could save ourselves a lot of guesswork and time by simply putting out a minimum amount of documentation at release. Then we listen to forums and support cases to better understand user feedback. Based on that feedback, we iterate on the docs. In this way, we make sure the information we're adding aligns with user needs rather than just adding all the information we *think* users might want to know about.

## Techniques for hiding less-used information

If you can't delete information to reduce complexity, look for ways to hide less-used information on the screen through JavaScript techniques, such as show/hide elements, expand/collapse toggles, navtabs, tooltips, and more.

While troubleshooting a recent support case, I looked over documentation I'd written nearly a year ago, trying to identify where the user got stuck. I was shocked at how confusing the docs now seemed. The documentation tried to explain query syntax for targeting elements in a media feed that could be either JSON or XML. If the feed was JSON, developers would use one type of query syntax; if the feed was XML, they would use another. The documentation discussed the two approaches in sections one right after another.

This scenario is common in developer docs because you often have multiple languages to account for. You might have a process for calling an API that you need to explain using PHP, Java, .NET, or other languages and frameworks. The general approach might typically be the same, but the code samples and specific technical details will differ.

In these scenarios, a common approach in documentation is to hide the languages users don't need. As I revised the JSON/XML documentation, I started separating out the languages into navtabs, like this:

<a class="noCrossRef" href="https://developer.amazon.com/docs/fire-app-builder/set-up-recipes-categories.html"><img src="images/navtabsseparatinglangs.png"/></a>

Previously, I had these sections stacked on top of each other, which lengthened the page and increased the visual clutter. By incorporating navtabs like this, users who care only about JSON or XML can select the corresponding tab and avoid seeing the irrelevant material.

As technical writers, when we try to simplify information, our first assessment should be to consider whether we can delete the information. But in many cases, product teams want the information included, even if it applies to just a minority of users. In these cases, we can rely on interactive JavaScript techniques for hiding this less-used information. Hiding these details can help simplify our docs because users won't have to sort through potentially irrelevant information in order to read the instructions.

### If you can't delete it, hide it

In user interface design, hiding complexity is a standard approach taken to simplify applications. User interface designer Tyler Tate explains:

> If you can’t kill a complex feature, the next best thing is to hide it. Too often, rarely used yet complex features take up more screen real estate than frequently used yet simple features. This shouldn’t be. A good user interface should make the most common tasks the most prominent and then hide rare tasks so that they don’t get in the way. &mdash; [Minimizing Complexity In User Interfaces — Smashing Magazine](https://www.smashingmagazine.com/2009/10/minimizing-complexity-in-user-interfaces/)

Hiding complexity is one way to simplify the information experience for users. Although most UI principles apply to interface design, we can equally apply them to documentation. Here's the same passage above but adjusted to target documentation:

> If you can’t kill a complex *explanation*, the next best thing is to hide it. Too often, rarely used yet complex *explanations and processes* take up more screen real estate than frequently used yet simple features. This shouldn’t be. *Good user documentation* should make the most common tasks the most prominent and then hide rare tasks so that they don’t get in the way.

When Tate designs a UI, he considers the 80/20 rule, where 80% of people use just 20% of the features. He makes the 20% of features occupy prime real estate while either removing or hiding the other less-used features.

### Sample JS techniques for hiding information

We can use a number techniques to hide complex information. Here are a variety of techniques along with examples:

* **Navtabs to separate information above the fold.** [GitHub Pages Docs](https://pages.github.com/) let users choose their path and then shows information related just to that path. [Intuit](https://developer.intuit.com/docs/00_quickbooks_online/1_get_started/00_get_started) also separates out different steps into sidebar tabs to keep all information readily visible.
* **Navtabs to load different information on the page.** My [Fire TV Device Specifications](https://developer.amazon.com/docs/fire-tv/device-specifications.html) provides a good example. Instead of 8 separate pages, all specs are available from the same page, hidden until you choose the device with the specs you want to see.
* **Expand/collapse functionality for sidebar menus.** [Apple's Home Pod](https://help.apple.com/homepod/) documentation provides a good example of expand/collapse features in a sidebar. You can even hide the entire sidebar.
* **Expand/collapse buttons in the main body of content.** [Twilio's tutorials](https://www.twilio.com/docs/authy/tutorials/account-verification-csharp-mvc) reduce complexity by only showing the next step in a tutorial after you click Next at the bottom. The next content loads on the same page. Impressively, the code in the right side pane shows the relevant code in focus and blurs the other code. [Google Play Console's help](https://support.google.com/googleplay/android-developer/answer/7159011?hl=en&ref_topic=7072031) also regularly collapses documentation into expandable sections.
* **Glossary tooltips that appear when you click a term.** I incorporated glossary tooltips on some unfamiliar terms in the [Login with Amazon documentation](https://developer.amazon.com/docs/login-with-amazon/documentation-overview.html#understanding-login-with-amazon). This reduces the visual clutter of a definition in the main body of text.

### Design decisions: stacked or adjacent?

It might not always be appropriate to hide information. Designer Ryan Singer explains that sometimes it's better to stack information while other times it's better to position it adjacent in space. Singer says that he learned this distinguishing principle from Edward Tufte:

> I once saw Tufte give a workshop in Chicago where he introduced a valuable concept. He said information may be displayed adjacent in space or stacked in time. Take a book for example. If two dots are on the same spread, they are adjacent in space. All it takes to switch between them is movement of your eye. Compare that to a dot on one page stacked above a dot on another page. You can’t see them at once. You have to flip back and forth between pages to see one dot versus the other.”
>
> The trade-offs between elements adjacent in space versus stacked in time are always in the mind of a UI designer. Placing many elements on the same screen reduces the need for navigation and gives users a comprehensive feeling of “it’s all at my command.” Moving focus from one element to another is instant and seamless. On the flip side, separating elements onto different screens slows things down with navigation while increasing clarity. There is more room for explanation and luxurious space when fewer elements occupy the page. The eye has less to filter through. The course of action is more obvious.[Learning from “bad” UI – Signal v. Noise](https://signalvnoise.com/posts/1128-learning-from-bad-ui)

In short, if placing elements side by side creates a sense of confusion (because the user needs both types of information), consider stacking instead. But if users don't need both sets of information, consider stacking because it allows users to more easily focus on the material and stay immersed in it.

In cases where you're showing code for different programming languages, stacking would be better. There's no need for the user to take in multiple code languages at once.

### Using JS in docs makes PDF and XML problematic

One consequence of implementing JS techniques to hide complexity is that the information becomes harder to generate to PDF. You pretty much end up with a web-only output. If you have requirements to deliver PDF, you might be limited in the number of JS techniques you can implement, or you'll have to code the content more carefully.

Implementing JS techniques also poses challenges for authors following structured authoring schemas like DITA or Docbook. If you want to implement some show/hide elements with JS, you probably can't, as that code won't validate with the schema. Given that the number of authors who must conform to a given XML schema constitute a large number of tech writers, it's no surprise that JS isn't more commonly used in docs. This is part of the reason tech doc interfaces tend to feel outdated in comparison to modern website UIs. If we want to embrace modern web interfaces that give us greater control to simplify the information shown to users, we will probably start ditching PDF and XML.

Finally, many tech writers feel that hiding elements on the page reduces the user's ability to quickly find information, such as after landing on a search results page or when pressing Ctrl+F. If users can't quickly locate information because the content is hidden by default, they might quickly lose patience and leave the page. Because of this, you probably want to limit the number of hidden elements on the page so that users don't play guessing games in opening various doors to see where the information might be hidden. On the other hand, with clearly labeled section headings, locating the information should be fairly intuitive. And because of the reduced visual clutter, users might be able to see the section more quickly.
