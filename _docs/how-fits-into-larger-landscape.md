---
title: Assessing how new information fits into the larger landscape
permalink: how-fits-into-larger-landscape.html
published: false
---

In [Overcomplicated: Technology at the Limits of Comprehension](https://www.amazon.com/Overcomplicated-Technology-at-Limits-Comprehension/dp/0143131303), Samuel Arbesman explores why technology has become increasingly complex. He covers a variety of factors throughout the book; two factors I want to call attention are specialization and interconnectedness, as these two factors have a direct relevance with documentation systems.

Both specialization and interconnectedness contribute to a high degree of complexity in a system. When these two elements are pushed to extremes, the result is a scenario where no one understands the full scale of how something works, nor how one system affects or influences the other systems it interacts with.

With documentation systems, when subject matter experts contribute specialized articles into a larger system without understanding how their individual article interacts with other information in the system, the result is a redundant, contradictory, and ever-increasing jumble of content.

* TOC
{:toc}

## Specialization

Let's start with specialization, as this is a concept already somewhat familiar. Arbesman explains:

> As knowledge grew beyond the bounds of any one continent, or culture, or mind, to have confident grasp of the systems around us we would have to specialize&mdash;to understand a small field very well, say, advanced weaponry, or some subfield of science .... knowledge has grown far beyond any single person's capacity to master it. To build models of the world and new technological systems at the frontiers of what we know, we have had to learn "more and more about less and less"&mdash;to specialize in different domains.  

I'll given an example of specialization by describing one of the domains I document at work &mdash; app development for Fire TV. Fire TV is based on the Android operating system, which provides a rich, robust landscape of Java-based APIs for developers to build apps for all types of devices. But apart from the Android foundation, Fire TV itself has various components that have different specializations. Some specialists are responsible for the multimedia components (the media playback). For example, understanding how apps handle audio focus when you change from app to app is critical, especially when you introduce voice commands that have to interrupt the app that is currently handling audio. Playing Pandora, asking what the weather is like, and then playing Netflix all within the same sequence require a complex understanding about how to manage audio focus within your app. (If you've ever had an app whose audio wouldn't stop playing after you closed the app, you know what failure in this area looks like.)

Another area of specialization involves how apps can populate the Fire TV home screen through recommendations. Apps can leverage Android's recommendations API to send recommended titles, but Amazon also provides a host of "extras" for additional information, such as rating and IMDB information. How does the Fire TV home screen decide which recommendations to handle, the limits of recommended tiles, the order, placement, and other handling of content on the home screen? What algorithms drive the content that different audiences see on the home screen, from the featured media, the ads, special rows for Netflix and HBO, and more (including both Prime and non-Prime audiences, U.S. and international audiences, etc.)? How do you decide what content to highlight in the top banner for users across regions and marketplaces? Again, this involves another layer of specialization.

When you link your Echo or other Alexa-enabled device to your Fire TV, this creates another layer of complexity. Voice commands transition into directives passed through a middleware layer to your Fire TV device, and so on. Voice commands can initiate from near-field (your remote) or far-field (an Alexa-powered device like an Echo). Suppose you have both an Echo and Echo Dot, and both are linked to your Fire TV. What logic decides which Echo responds, how does the microphone array inside each echo decide which device responds and initiates the directives to the Fire TV?

These are just a few examples, but there are hosts of others. Consider the hardware elements (the system on chip and graphics properties), the physical elements of the device (such as its size and the way it connects to your TV, which in the case of Gen 3 models was a somewhat ugly dongle ["pendant"]), and more. The multimedia team has an extremely geekly knowledge of codecs, refresh rates, bit rates, media players, and other details. They ensure correct audio/video syncing with 4k content and more. If you're ever watching a movie and the sounds don't match the actor's mouth movements, the audio/video is out of sync.

Fire TV is just an example of a product that involves many different specialists all providing deeply technical input that is not understood in depth by any single team. A complex product might involve 20 different specialist teams each contributing to it in important ways &mdash; most frighteningly, each of these components joins a playing field of other actors rather than giving a solo performance. Yet each specialist has only a superficial understanding of how the other parts of the system work.

To gain **in-depth** knowledge, the specialist has to sacrifice **breadth** of knowledge. The ability to go both deep *and* broad (playing the Renaissance role where you're a master of everything from physics to art to medicine and poetry) ended long ago. We live in an era of specialization, and this specialization contributes to scenarios where systems become complex.

To provide documentation for a complex product, one strategy is to have the specialists contribute the content related to their area of expertise. For example, the audio focus engineer contributes best practices for handling audio within an app, the multimedia team contributes best practices for syncing audio-video streams with playback rates, the Alexa team handles the voice interactions, the localization team handles the language preferences and string options, and more.

However, here's where this model breaks down. If each expert team contributes their knowledge in a siloed, independent way, how do they know if their contributions overlap, contradict, or harmonize with the contributions that other experts make?

This is the problem with any kind of multi-authored documentation effort &mdash; contributing experts have tunnel vision in the system. They look (in a myopic way) at their own piece of the information landscape, because that's the area they understand in depth. When the engineer contributes a specialized article, does he or she read the other information on the developer portal to understand if the content he or she is contributing harmonizes with other information on the site? Does the contributor even read the information on the site in any depth? Suppose the site has thousands of pages of documentation. How does the contributor even know what other pages are relevant, and whether the information he or she is contributing contradicts, harmonizes, or integrates well with the other information?

A contributor's myopia would be acceptable if each of the documentation components functioned independently of each other. For many topics, this is indeed the case. But increasingly, one element interacts with other elements, one system interacts with other systems, and so on. The nature of the web is trending toward an interconnected web of APIs, where multiple systems interact and influence each other. This is where specialization and interconnected systems create a risk of unpredictability and lack of interoperability. Arbesman explains,

> Specialization is required in order to understand more and more about the intricate systems around us, such as the human body, now divided up among numerous specialties in medicine. But at the same time, the systems we are building&mdash;the technologies that run our world&mdash;are not only intricate and complicated, but also stitch together field after field. We have systems in the world of finance that require an understanding physics; there are economists involved in the development of computer systems. The design of driverless cars is a good example, requiring collaboration among those with expertise in software, lasers, automotive engineering, digital mapping, and more.
>
> In other words, even as specialization aids us in making advances, we are ever more dependent on systems that draw from many different areas, and require an understanding of each of these. Yet a single person can no longer possess all the necessary knowledge. To any one person, these systems as whole are truly incomprehensible.

Arbesman says that it's not uncommon for unexpected interactions to result after these systems (which no single individual understands) interoperate. When this happens, there's a high risk for massive failure that few can solve. As an example, Arbesman describes a day in 2015 when both the United Airlines grounded its planes and the New York Stock Exchange halted trading, both due to computer glitches. Arbesman later explores the value that generalists bring, and how necessary it can be for an individual to have several areas of expertise.

From a documentation point of view, I'm more concerned about solving the basic problem of content interoperability, or content harmony within a vast system of information. When the expert wants to contribute a topic, how can we look into our landscape of information and know what else has been said about that topic? What other topics does this new topic affect? How can we know if the new topic will contradict, overlap, or otherwise influence these other topics?

You can be sure that readers bounce from topic to topic, landing on search results that list all pages with the common keyword the user searched for. For example, suppose a user searches for "MediaSession," and the results return topics from 6 different areas of the site. What is the user's experience in navigating all of this [potentially conflicting] information?

We can't expect contributing experts to be familiar with all the documentation on a site, but couldn't we present a list of related topics for the contributor to consult? By surfacing all content written on a similar topic, the contributing expert can get a slightly enlarged view of the larger context for the information he or she is contributing to.

Additionally, if we know the owners of the other topics, they can evaluate the appropriateness of the new information being added. Like an elephant herd deciding to accept a new elephant to the herd, this group of content owners, connected by a similar topic theme, can choose to accept or reject the new elephant [content].

The ability to surface similar information returns us to the topic of metadata, which we touched on in the previous topic: [Discoverability through metadata &mdash; strategies to guide users through complex, non-linear systems](discoverability-through-metadata.html). In that previous section, I kept the discussion fairly high-level, but now we'll get a bit deeper. We need at least two metadata properties to incorporate the innerconnectedness of similar information:

* owner
* tags

The owner is easy enough to identify. For each topic, one must merely identify a single "buck-stops-here" kind of person who takes ownership of the content. Tags is much more tricky, because tags must align with a controlled vocabulary to prevent them from going in 10 different directions. For example, without a controlled vocabulary, content related to "mediasession" could be tagged as "media-session," "MediaSession,", "Media Session," "media session", "mediaSession," and more.

What strategies do you use for tags? If the topic has just one tag, what purpose does that serve? And how do tags differ from a keyword search with this tag? It's all fine to say that we'll merely "tag" our content as a way to surface relevant topics, but this is not an easy task to achieve.

## Complexities of tagging

A coherent tagging systems needs to establish a controlled vocabulary for tags, but that's not all. There are many other questions to answer:

* How many tags? How granular?
* Should tags repeat product titles?
* How can you dynamically return the tags the user wants to know about?
* How do tags differ from a search with these same keywords?
* How can you implement a tagging system if each author creates content in separate projects?

I'm a tech writer in the trenches, so I don't just speculate at theoretical levels. I experiment, I implement, I evaluate. So let's get cracking with real detail.

I decided to start my tags with one of my favorite products I document: [Fire App Builder](https://developer.amazon.com/docs/fire-app-builder/overview.html). It's a kick-ass Android-based framework for building Fire TV apps. I added a new field to my Jekyll frontmatter:

---
title: My page
permalink: mypage.html
doctags: accessibility, mediasession
---

Why not just `tags`, you ask? Well, in Jekyll-land, `tags` is a global variable used with posts (rather than pages), and so Jekyll always thinks this `tags` object is full, even when it's null. It messes up scripting logic.

We could just round up all tags on a page using a simple Liquid `for` loop, like this:

```liquid
{% raw %}<b>tags:</b>
{% for doc in site.docs %}
  {% if doc.doctags == "none" %}
    {% assign doctagsList = doc.doctags | split: "," %}
    {% for singleDoctag in doctagsList %}<a href="../tags/{{singleDoctag}}.html">{{singleDoctag}}</a>{% unless forloop.last %}, {% endunless %}
    {% endfor %}
  {% endif %}
{% endfor %}{% endraw %}
```

Here we check whether the page has a `doctags` field that evaluates truthy (isn't null). If so, we get the value and split the comma-separated values into an array. Then we iterate through each item in the array and push the tag into an HTML link with that tag name.

However, suppose each writer starts listing doctags willy-nilly, like this:

```
---
title: My page
permalink: mypage.html
doctags: accessibility, mediasession, disabled, blind users, audio focus, media-session API, audio handling
---
```

Well, here you can see the dangers of user-defined tags. These tags won't correctly surface all the other pages with these tags because the tags themselves lack consistency. So we need to implement an "allowed tags" list and check to make sure each tag is on that list before we list it as a link:

```liquid
<b>tags:</b>
{% for doc in site.docs %}
  {% if doc.doctags %}
    {% assign doctagsList = doc.doctags | split: "," %}
    {% assign projectDoctags = site.data.doctags.allowed-doctags %}
    {% for singleDoctag in doctagsList %}
      {% if projectDoctags contains singleDoctag %}<a href="../tags/{{singleDoctag}}.html">{{singleDoctag}}</a>{% unless forloop.last %}, {% endunless %}
      {% endif %}
    {% endfor %}
  {% endif %}
{% endfor %}
```

In the \_data folder, we have a yml file called `allowed-doctags.yml` that looks like this:

```yaml
allowed-doctags:
  - jekyll
  - mediasession
  - windows
  - adb
  - github
  - security-profile
  - voice
  - components
  - ui-design
  - ads
  - analytics
  - authorization
  - media-player
  - app-submission
  - in-app-purchasing
  - accessibility
  - catalog-integration
  - recommendations
  - media-feed
  - emulator
  - fire-tv-home-screen
```

These are the tags I surfaced from just one product, but there are probably 50 different products across the Developer Portal. How do we know when a tag should be a tag? What are the rules and criteria for tag formation? For naming?

I'm not totally sure, but here's what I have so far:

* Tags should not repeat the product name. Presumably the `product` is another piece of metadata already associated with the page (I didn't show it earlier, but it's there). In our scripting logic, we can let the `product` metadata interact with the `doctags` metadata in efficient ways. There's no need to contaminate `doctags` with `product` values.
* Tags should be common themes that might be apparent across multiple pages. It doesn't make sense to have a tag so granular that it appears on just one page. The whole point is to use tags as a way to grow an organic connective tissue across the site that will attach to all pages. At the other end of the spectrum, the tag shouldn't be so broad that it isn't meaningful.
* Tags shouldn't indicate the information type. I already have another tag for that called `type`. I identify whether the page is a how-to, release note, video, reference, troubleshooting, glossary, and so on. Similar to `product`, our scripting logic might potentially pull from `type` already, so there's no need to repeat the same metadata values.

Where things get interesting is when we cross product boundaries. I'm not sure how useful tags are within the same product. Presumably, all the topics related to `recommendations` are already grouped together in same folder. A user just needs to glance in the sidebar to see the other similar topics. If similar topics aren't already grouped together, that's somewhat odd.

Where it gets interesting is to see how tags surface content *across* products. What pages from other doc sets (from Fire tablets to Alexa Skills Kit to In-app Purchasing) might the `recommendations` tag be applicable, and what would the content say?

To have any consistency and uniformity with the tags, they need to be implemented across authors in a site-wide way. But it also means that, if we're going to roll-up all pages that have the same tag, all content needs to be in the same system. If we have multiple Jekyll projects, how do we get a list of pages that all have the same tag? At some point, each project would need to roll up into other projects prior to building Jekyll, but that's not how the architecture works.









---------
question;

- what is the value of a tag versus a keyword?
- what strategies do you use for the tags?
- can you use a tag in combination with a product?
- what has been said about tagging?
- tagging alone isn't going to do everything you need to do. you also need a filtering mechanism. how complex and dynamic can you make the filters? look at the doctoolshub site made with algolia. pretty amazing when you can push and pull all of these levers based on the metadata.
- can you create complex filters that look at 3 different tags?
- could you just work with these smaller records, the metadata part of them? or is that all jekyll is actually doing?
- how can you speed up filters?
- if you're going to get serious about this, should you be doing the scripts in python or hugo instead?
- should i be learning python?
