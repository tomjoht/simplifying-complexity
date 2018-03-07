---
title: Ensuring information harmony in the larger documentation landscape
permalink: ensuring-information-harmony-in-the-larger-documentation-landscape.html
---

In [Overcomplicated: Technology at the Limits of Comprehension](https://www.amazon.com/Overcomplicated-Technology-at-Limits-Comprehension/dp/0143131303), Samuel Arbesman explores why technology has become increasingly complex. He covers a variety of factors throughout the book, but two factors I want to call attention are **specialization** and **interconnectedness**, as these two factors have a direct relevance to documentation.

Both specialization and interconnectedness contribute to a high degree of complexity in a system. When these two elements are pushed to extremes, the result is a scenario where no one understands the full scale of how something works, nor how one system affects or influences the other systems it interacts with. Disaster scenarios can develop swiftly and catastrophically.

With documentation systems, when subject matter experts contribute specialized articles into a larger system without understanding how their individual article interacts with other information in the system, the result is often a redundant, contradictory, and ever-increasing jumble of content. In this article, I'll explore ways to solve this problem through better metadata.

* TOC
{:toc}

## Specialization and interconnectedness

Let's start with the trend of specialization, as this is already a familiar concept. (Later, we'll show how specialization combines with interconnectedness to create complex problems.) Arbesman explains:

> As knowledge grew beyond the bounds of any one continent, or culture, or mind, to have confident grasp of the systems around us we would have to specialize&mdash;to understand a small field very well, say, advanced weaponry, or some subfield of science .... knowledge has grown far beyond any single person's capacity to master it. To build models of the world and new technological systems at the frontiers of what we know, we have had to learn "more and more about less and less"&mdash;to specialize in different domains.  

I'll give an example of specialization by describing one of the domains I document at work &mdash; app development for Fire TV. Fire TV is based on the [Android operating system](https://developer.android.com/index.html), which provides a rich, robust landscape of Java-based APIs for developers to build apps for all types of devices.

<figure style="max-width: 200px; float: right; padding: 0px 20px">
<a class="noCrossRef" href="https://www.amazon.com/Overcomplicated-Technology-at-Limits-Comprehension/dp/0143131303"><img src="images/overcomplicated.png"></a><figcaption>Overcomplicated explores the complex entanglement that technology has become, where no one understands all the pieces yet they are all interacting together as a whole.</figcaption></figure>Apart from the Android foundation, Fire TV itself has various components that have different specializations. Some specialists are responsible for audio focus handling. Understanding how apps handle audio focus when you change from app to app is critical, especially when you introduce voice commands that have to interrupt the app that is currently handling audio. Playing Pandora, asking what the weather is like, and then playing Netflix all within the same sequence require a complex understanding of how to manage audio focus within your app. (If you've ever had a situation on your smartphone where the audio wouldn't stop playing after you closed the app, you know what failure in this area looks like.)

Another area of specialization involves how apps can populate the Fire TV home screen through recommendations. Apps can leverage Android's recommendations API to send recommended titles, but Amazon also provides a host of "extras" for additional information, such as rating and IMDB information. How does the Fire TV home screen decide which recommendations to handle, the limits of recommended tiles, the order, placement, and other handling of content on the home screen? What algorithms drive the content that different audiences see on the home screen, from the featured media, the ads, special rows for Netflix and HBO, and more (including both Prime and non-Prime audiences, the U.S. and international audiences, etc.)? How do you decide what content to highlight in the top banner for users across regions and marketplaces? Again, this involves another layer of specialization.

When you link your Echo or another Alexa-enabled device to your Fire TV, this creates more complexity. Voice commands transition into directives passed through a middleware layer to your Fire TV device, and so on. Voice commands can initiate from near-field (your remote) or far-field (an Alexa-powered device like an Echo). Suppose you have both an Echo and Echo Dot, and both are linked to your Fire TV. What logic decides which Echo responds?  How does the microphone array inside each Echo decide determine which device is closer to the sound source?

These are just a few examples of specialized knowledge around a single device, but there are hosts of others. Consider the hardware elements (the system on chip and graphics properties), the physical elements of the device, such as its size and the way it connects to your TV, which in the case of Gen 3 models was a dongle ["pendant"]), and more. The multimedia team has an extremely geeky knowledge of codecs, refresh rates, bit rates, media players, and other details. They ensure correct audio/video syncing with 4k content and more. If you're ever watching a movie and the sounds don't match the actor's mouth movements, the audio/video is out of sync.

Fire TV is one example of a product that involves many different specialists all providing deeply technical input that is not understood in depth by any single team. A complex product might involve 20 different specialist teams each contributing to it in important ways. Commonly, each specialist joins a stage of other actors working in a carefully choreographed play rather than giving a solo, independent performance. Each specialist must act *in harmony with the other actors* on stage, but each specialist usually has only a superficial understanding of the other actors' roles and parts.

To gain **in-depth** knowledge, the specialist has to sacrifice **breadth** of knowledge. The ability to go both deep *and* broad (playing the Renaissance role where you're a master of everything from physics to art to medicine and poetry) ended long ago. We live in an era of specialization, and this specialization contributes to scenarios where systems become complex.

## When specialists contribute to docs

To provide documentation for a complex product, one strategy is to have the specialists contribute the content related to their area of expertise. For example, the audio focus engineer contributes best practices for handling audio within an app, the multimedia team contributes best practices for syncing audio-video streams with playback rates, the Alexa team handles the voice interactions, the localization team handles the language preferences and string options, and more.

However, here's where this model breaks down. If each expert team contributes their knowledge in a siloed, independent way, how do they know if their contributions overlap, contradict, or harmonize with the contributions that the other experts make?

This is the problem with any kind of multi-authored documentation effort &mdash; contributing experts have tunnel vision in the system. They often look (in a myopic way) at their own piece of the information landscape, because that's the area they understand in depth. When the engineer contributes a specialized article, does he or she read the other information on the developer portal to understand if the content he or she is contributing harmonizes with other information on the site? Does the contributor even read the information on the site in any depth? Suppose the site has thousands of pages of documentation. How does the contributor even know what other pages are relevant, and whether the information he or she is contributing contradicts, harmonizes, or integrates well with the other information?

A contributor's myopia would be acceptable if each of the documentation components functioned independently of each other. For many topics, this is indeed the case. But increasingly, one element interacts with other elements, one system interacts with other systems, and so on. The nature of the web is trending toward an interconnected web of APIs, where multiple systems interact and influence each other. This is where specialization and interconnected systems create a risk of unpredictability and lack of interoperability.

Arbesman explains,

> Specialization is required in order to understand more and more about the intricate systems around us, such as the human body, now divided up among numerous specialties in medicine. But at the same time, the systems we are building&mdash;the technologies that run our world&mdash;are not only intricate and complicated, but also stitch together field after field. We have systems in the world of finance that require an understanding physics; there are economists involved in the development of computer systems. The design of driverless cars is a good example, requiring collaboration among those with expertise in software, lasers, automotive engineering, digital mapping, and more.
>
> In other words, even as specialization aids us in making advances, we are ever more dependent on systems that draw from many different areas, and require an understanding of each of these. Yet a single person can no longer possess all the necessary knowledge. To any one person, these systems as a whole are truly incomprehensible.

Arbesman says that it's not uncommon for unexpected interactions to result when these systems (which no single individual understands) interoperate. When this happens, there's a high risk of massive failure that few can solve. As an example, Arbesman describes a day in 2015 when both the United Airlines grounded its planes and the New York Stock Exchange halted trading, both due to separate computer glitches that were thought to be related. Arbesman later explores the value that generalists bring, and how necessary it can be for an individual to have several areas of expertise.

From a documentation point of view, I'm concerned about solving the issue of content interoperability, that is, finding a way to ensure content harmony within a vast system of information, especially when engineers act as contributing authors (as if often the case with developer portals). When the expert wants to contribute a topic, how can we look into our documentation landscape and know what else has been said about that topic? What other topics does this new topic affect? How can we know if the new topic will contradict, overlap, or otherwise influence these other topics?

You can be sure that readers bounce from topic to topic, landing on search results that list all pages with the common keyword the user searched for (from docs to blog to forum and more). For example, suppose a user searches for "MediaSession," and the results return topics from 6 different areas of the site. What is the user's experience in navigating all of this [potentially conflicting] information?

We can't expect contributing experts to be familiar with all the documentation on a site, but couldn't we present a list of related topics for the specialist contributor to consult? By surfacing all content written on a similar topic, the contributing expert can get an enlarged view of the context for the information he or she is contributing to.

Additionally, if we know the owners of the other topics, they can evaluate the appropriateness of the new information being added. Like an elephant herd deciding to accept a new elephant to the herd, this group of content owners, connected by a similar topic theme, can choose to accept or reject the new [content] elephant.

## Metadata strategies to surface similar-themed content

The ability to surface similar information returns us to the topic of metadata, which we touched on in the previous topic ([Discoverability through metadata &mdash; strategies to guide users through complex, non-linear systems](discoverability-through-metadata.html)). In that previous section, I kept the discussion fairly high-level, but now we'll get a bit deeper. We might need at least two metadata properties to help interconnect information:

* `owner`
* `tags`

The owner is easy enough to identify. For each topic, we must merely identify a primary person who takes ownership of the content. This owner can help be identified in a gating workflow with the introduction of new content. Tags are trickier because tags must align with a controlled vocabulary to prevent them from going in 10 different directions. For example, without a controlled vocabulary, content related to "media session" could be tagged as "media-session," "MediaSession,", "Media Session," "mediasession", "mediaSession," and more.

What strategies do you use for tags? If the topic has just one tag, what purpose does that serve? And how do tags differ from a keyword search with this tag? It's fine to say that we'll merely "tag" our content as a way to surface relevant topics, but this is not an easy task to implement.

I consulted the WTD community for any experiences with tagging. One community member pointed me to [Wavefront Docs](https://docs.wavefront.com/), which uses tags to provide alternative arrangements of information.

<figure><a class="noCrossRef" href="https://docs.wavefront.com/"><img src="images/wavefrontdocs.png"/></a><figcaption>The green squares in the main content window are tagged content. The tagged content provides an alternative view of the same information arranged hierarchically in the sidebar.</figcaption></figure>

In this example, tags are multipurpose, combining information type (e.g., "getting started") with the topic (e.g., "query language"). Ideally, we want to combine tags together in compound ways to filter the information (such as "getting started" paired with "query language"). But I also want to see how "query language" might be addressed in other sources *outside* the documentation, such as the Wavefront blog, forum, white papers, and other information sources.

## Complexities of tagging

A coherent tagging system needs to establish a controlled vocabulary for tags, but that's not all. There are many other questions to answer:

* How many tags should a site have? How granular should the tags be?
* Should tags repeat product titles? Should tags include information types (e.g, getting started)?
* On a technical level, how can you dynamically return the tags the user wants to know about?
* How do tags differ from a search with these same keywords? Are tags just an older practice of topical indexing that was replaced a decade ago with keyword search?
* How can we implement a tagging system if each author creates content in separate projects? Can we implement tagging across docs, forums, and blogs? If so, don't we need an enterprise-wide taxonomy?
* If we have an enterprise-wide taxonomy, how do we manage the terms? What process do we agree on to decide on the terms, updates to terms, and more?

There are a lot of questions around tagging. This is because I'm scratching the surface of other disciplines here &mdash; the practice of taxonomy and classification gets us into library science, information architecture, and knowledge management. Do I need a specialist degree in these fields to provide meaningful tags in my content?

One WTD member said her experience with tagging required a tremendous amount of work for a relatively small doc set (100 pages) and didn't seem worth the effort. This leads me to wonder whether tags are worth it, or if I should just default to keyword searches for information?

I'm just speculating here, but I think tagging gets interesting when the tags cross boundaries in interesting ways. When a tag for "mediasession" returns documentation content across different product doc sets, blog articles, and forum knowledge-base articles, the list of items is a lot more interesting than tags that return documentation alone (especially documentation for just one product). When tags pull in content across boundaries, we start to see more purpose behind the tagging. Maybe we discover that the marketers refer to "MediaSession" as "Android Media APIs," and perhaps their blog article on the topic surfaces information that is outdated or contradictory with the docs. With the forum, we have support agents and engineers providing help related to this topic. How do their responses align with the doc content and the blog?

Tagging within the same system isn't nearly as interesting as tags across systems. This kind of activity would open up dialogue and collaboration across these groups. It would also help increase awareness about just what these groups are doing (it's easy to just ignore marketing content and support articles). If tags do nothing other than break down silos between these other groups, establish communication about terminology, and help us connect owners with the topics as they participate in various circles, that alone is a huge win. It does also expand the effort. Tags become more than just a metadata activity. Tagging becomes a cross-department dialogue.

## A filtering interface powered by tags

I have been diligently working on a coding solution for these tags within our Jekyll project. This post is already long, so I won't bury it in technical details here. However, when I have a functional prototype in publicly accessible docs, I'll revisit this article and provide a link.

[DocToolhub](https://doctoolhub.com/) is an interface that provides filters users can toggle to mix and match the information they want to see, letting users select the information type, product, topic, version, and more.

<figure><a class="noCrossRef" href="https://doctoolhub.com/"><img src="images/doctoolhub.png"/></a><figcaption>DocToolHub lets you select filters that determine which results are shown.</figcaption></figure>

What would a DocToolHub type of site look like in a Developer Portal? Again, my purpose here isn't to lay out the technical details, but to ponder a solution to this scenario of complexity. I want to know how a new piece of information fits and harmonizes with the rest of the information on the documentation landscape. Topic-based tags are just one idea for achieving that.

## Search versus tags

I'm somewhat mixed about the value of tags. Most documentation systems don't have carefully developed taxonomies or tags across topics. The default way that users find content is through search. Consequently, perhaps the efforts around building tags will ultimately be like creating [Yahoo's Directory of the Web](https://searchengineland.com/yahoo-directory-close-204370)? Maybe the number of keywords and topics is too vast to comprehend using a definitive list of descriptive tags.

As a user, yes I would appreciate seeing topical indexes of content, but I'd like these filters built directly into search as well, and I will likely not trust that a tag page showing all instances of the topic actually contains all known instances of that topic. I would still search for the content.

In an ideal world, one meticulously tags content *and* ensures search surfaces the content. But with limited bandwidth, perhaps tagging requires too much effort? I'm not sure. Most likely, I will experiment in this area and see what I discover.

If you have feedback you'd like to share about tagging strategies, please use the comment form below.
