---
title: How the information fits into the larger landscape
permalink: how-fits-into-larger-landscape.html
published: false
---

Both specialization and interconnectedness are two factors that contribute to a high degree of complexity in a system. When these two elements are pushed to extremes, the result is a scenario where no one understands the full scale of how something works, nor how one system affects or influences the other systems it interacts with.

With documentation scenarios, these factors become all too familiar. Subject matter experts (SMEs) may contribute specialized articles into a larger system without understanding how their individual article interacts with other information in the system. As such, the Let me unpack these ideas with more detail.

* TOC
{:toc}

## Specialization

In *Overcomplicated: Technology at the Limits of Comprehension*, Samuel Arbesman explores why technology has become increasingly complex. He covers a variety of factors throughout the book; two factors I want to call attention are specialization and interconnectedness, as these two factors have a special resonance with complexity in documentation systems.

Let's start with specialization (a concept most of us are familiar with). Arbesman explains,

> As knowledge grew beyond the bounds of any one continent, or culture, or mind, to have confident grasp of the systems around us we would have to specialize--to understand a small field very well, say, advanced weaponry, or some subfield of science .... knowledge has grown far beyond any single person's capacity to master it. To build models of the world and new technological systems at the frontiers of what we know, we have had to learn "more and more about less and less"--to specialize in different domains.  

One of the products I document &mdash; app development for Fire TV &mdash; provides a perfect example of this specialization. Fire TV is based on the Android operating system, which provides a rich, robust landscape of Java-based APIs for developers to build apps. But apart from the Android foundation, Fire TV itself has various components that have different specialists. Some specialists are responsible for the multimedia components (the media playback). For example, understanding how apps handle audio focus when you change from app to app. For example, playing Pandora, answering a phone call, and then playing Netflix require a complex understanding about how to manage audio focus.

At the same time, other specialists are experts with the voice commands and interactions. How do voice commands that flow from your Alexa-enabled device (such as your Echo) transition into directives passed through a middleware layer to your Fire TV device, and how does Fire OS handle each of these commands? Again, this involves another specialization.

Another area of specialization involves how apps can populate the Fire TV home screen through recommendations. Apps can leverage Android's recommendations API to send recommended titles, but Amazon also provides a host of "extras" for additional information, such as rating and x and x. How does the Fire TV home screen decide which recommendations to handle, the limits, the order, placement, and other handling? What other algorithms drive the content you see on the home screen, from the featured media, the ads, special rows for Netflix and HBO, and more? Again, this involves another layer of specialization.

These are just three examples, but there are hosts of others. Consider the hardware elements (the system on chip and graphics card), the physical elements of the device, and more.

Fire TV is just an example of a product that involves many different specialists all providing deeply technical input that is not understood in depth by the other teams. Let's suppose our complex product has 20 different specialist teams contributing to it. Each specialist has only a superficial understanding of how the other parts of the system work. To gain **depth** of knowledge, the specialist has sacrificed **breadth** of knowledge. The ability to go both deep and broad (playing the Renaissance role where one could be a master of everything from physics to art to medicine and poetry) ended long ago.

To support the documentation for a complex product, one strategy is to have the specialists contribute the content related to their area of expertise. For example, the audio focus engineer contributes best practices for handling audio within an app, the multimedia team contributes best practices for syncing audio-video streams with playback rates (including 4k streams), and more.

However, here's where this breaks down. If each expert contributes the knowledge in a siloed way, how do they know if their contributions overlap, contradict, or harmonize with the contributions other experts make? This is the problem with any kind of multi-authored documentation effort &mdash; contributing experts have tunnel vision in the system. They look at their own piece of the information landscape, because that's the only area they understand in depth. When the engineer contributes a specialized article, does he or she read the other information on the site to even understand if other content has been written on the topic, or if other topics are related, or if the practices fit together in a bug free, fully functional way? No, they don't.

Their myopia would be acceptable if each of the documentation components functioned independently of each other. For many topics, this is indeed the case. But increasingly, one element interacts with other elements, one system interacts with other systems, and so on. The nature of the web is trending toward an interconnected web of APIs, where multiple systems interact and influence each other. Arbesman explains,

> Specialization is required in order to understand more and more about the intricate systems around us, such as the human body, now divided up among numerous specialties in medicine. But at the same time, the systems we are building--the technologies that run our world--are not only intricate and complicated, but also stitch together field after field. We have systems in the world of finance that require an understanding physics; there are economists involved in the development of computer systems. The design of driverless cars is a good example, requiring collaboration among those with expertise in software, lasers, automotive engineering, digital mapping, and more.
>
> In other words, even as specialization aids us in making advances, we are ever more dependent on systems that draw from many different areas, and require an understanding of each of these. Yet a single person can no longer possess all the necessary knowledge. To any one person, these systems as whole are truly incomprehensible.

Arbesman says that when unexpected interactions result when these systems (which no single individual understands) interoperate, there's a high risk for massive failure that few can solve. Arbesman later explores the value that generalists bring, or how necessay it can be for an individual to have several areas of expertise. But from a documentation point of view, I'm more concerned about solving the basic problem of "interoperability" of content. When the expert wants to contribute a topic, how can we look into our vast landscape of information and know what else has been said about that topic? What other topics does this new topic affect? How can we know if the new topic will contradict, overlap, or otherwise influence these other topics?

You can be sure that readers bounce from topic to topic, landing on search results that list all pages with the common keyword the user searched for. For example, suppose a user searches for "MediaSession," and the results return topics from 6 different areas of the site. What is the user's experience navigating all of this information?

We can't expect contributing experts to be familiar with all the documentation on a site, but we can require that they understand the context of the information. By surfacing all content that has similar tags, the expert can get a slightly enlarged view of the larger context for the information he or she is contributing.

To surface similar information, we can leverage the same tags we used to surface related information for users. This again comes back to the importance of metadata, but now, the more detailed and descriptive the keywords (as well as controlled), the better, as this gives us greater accuracy about which topics are truly related in the system.




As knowledge becomes more specialized, it also becomes more deeper, as experts go further into specific areas but become less aware of other areas of the system.

At the same time, systems are become more interconnected with each other. We develop systems (for example, APIs) that interact with other systems. When you combine specialization with interconnected systems, you end up with

<!--  -->




people see info as one-off, standalone content, not as part of larger landscape of information. this is really problem of having engineers write content. or of having a crowdsourced type of approach.

this ties in with the need to see the whole customer journey.

what information is already there. how does this information fit into what's already there?

complexity. siloes. working in siloes and these are supposed to interact. fire tv is one such system.

fall prey to specialization

how do you solve this problem? each page has tags that let you know what other pages it's related to.
