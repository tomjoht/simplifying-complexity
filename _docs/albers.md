---
title: Guiding users through complex, non-linear systems
permalink: guidance-through-non-linear-systems.html
published: false
---

In the previous tutorial, we looked at embedding maps to help guide users through larger processes. But all the maps I showed were *linear* maps. What about maps for non-linear, complex systems? In this section, we'll explore ways to guide users when defined paths don't exist.

* TOC
{:toc}

## Adaptive information systems for complex systems

A complex system isn't merely one that is technical or which contains many parts; it's not simply a system that is "complicated." A complex system is one that defies linear processes by including branching, conditions, feedback elements, many decision points, recursive processes, and ever-changing variables that affect the user's paths and decision points.

In "Complex Problem Solving and Content Analysis", Michael Albers characterizes a complex system as follows:

> Each new piece of data the user uncovers affects the path taken and the eventual outcome. ... it does not lend itself to being performed with a defined set of tasks nor can those tasks be performed in a fixed order. ... the step-by-step route to completing a task simply does not exist. ... instead of following a set path, the user continuously adjusts their mental path as new information presents itself. ... attempts to describe step-by-step actions break down because no single route to a solution exists. ([Content and Complexity](https://www.amazon.com/Content-Complexity-information-Technical-Communication/dp/0805841415))

In another article ("Dynamic Usability") in the same book, Barbara Mirel depicts a complex system with an example of a retail category manager trying to answer these two questions:

* "what mix of products should I stock to maximize profits and market share?"
* "what new product offering is likely to succeed in this market?"

The manager might run various reports, weigh different factors against each other, analyze trends and other conditions against the company's budget constraints, and perform other hard-to-describe tasks to arrive at a conclusion. Each analytical activity can change the path the user takes. There's a constant feedback loop with each input that affects the user's next steps through a system &mdash; hence, no linear map is available for this journey.

In these systems, presenting the user with a linear map that consists of specific tasks won't help much. Albers suggests that for these scenarios, the topics in the information system need to dynamically adhere together around the user's specific and constantly changing context. By decoupling the information into separate, semantically identified pieces, Albers says these pieces can be dynamically assembled to address the context the user needs at a particular moment in her or her journey.

Again, this context and the user's information needs constantly change as the user makes his or her way through the system (with feedback loops and inputs changing the path, or other chosen variables influencing the results). In this complex system where the context constantly changes, what information model can support the user? Only an information model that can adapt and change in similar ways to meet the evolving user context.

Albers says that a good way to understand this information model is with the analogy of "sintering" in ceramics. Sintering is the chemical process whereby individual components begin to naturally cohere into a connected structure. Watch this one-minute video to see the sintering process:

<iframe width="560" height="315" src="https://www.youtube.com/embed/NzCeMxq0bPs" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

How might sintering be implemented in an information system? Albers says that XML gives promise as an approach to decoupling information and dynamically assembling it. Albers wrote his article 15 years ago, when XML was still emerging as a common technology (so keep that context in mind). He writes:

> Only recently, with technologies such as XML, has information design gained the underlying tools to actually support complex problem solving in a general manner. With these new technologies, we finally have the means to break up the old contextual elements, recombine them at will, and present information uniquely focused on a problem. However, although the need to support complex problem solving is indisputable, we lack a clear methodology to support capturing the information requirements, reordering and dynamically constructing information to fit a situational context, and designing the interface for such a system. ([Content and Complexity](https://www.amazon.com/Content-Complexity-information-Technical-Communication/dp/0805841415))

In short, Albers wants to decouple information into small pieces and combine them as needed based on the user's changing context in real-time to address the user's complex needs. However, he isn't clear about a specific design or approach to actually pull this off. You won't find sample links to information systems that would provide an example. He doesn't include prototypes or more technical details on the implementation. It's an academic idea, but one that has a strong appeal.

Albers continues:

>...the requirements analysis cannot focus on defining a single path; nor can it define exactly which information is desired. Instead, the analysis must uncover potential information requirements and presentation methods.

What design most closely adheres to the information system Albers describes? Faceted navigation and filtered browsing designs provide one model. Another model might involve dynamically surfacing content based on the user's content. I'll explore each of these in the next sections.

## Faceted filtering and dynamic assembly

Step outside the documentation scenario for a moment and think of retail sites that contain thousands of products. It's now a common design pattern to provide filters the user can select to dynamically narrow the products. For example, in this shoe site, [sportsshoes.com](https://www.sportsshoes.com/products/shoe/), you can filter by about a dozen product attributes.

<caption><a href="https://www.sportsshoes.com/products/shoe/" class="noExtIcon"><img src="images/sportsshoesfacets.png"/></a><figcaption>You can filter by gender, sport, product type, brand, type, size, price range, sport, gender, size, price, color, terrain, and features. Faceted filters have been critical in helping users find and buy the right products.</figcaption></caption>

You see some faceted filters in documentation websites, but it's not as common. Common filters might be based on versions, languages, or platforms. Here's an [example from Antidot's Fluid Topics platform](https://discover.fluidtopics.com/search/all?query=overview), which provides a robust documentation interface for facets by leveraging content attributes.

<a href="https://discover.fluidtopics.com/search/all?query=overview" class="noExtIcon"><img src="images/fluidtopicsdemo.png"/></a>

I suspect this design pattern would be more commonly implemented if the tooling were more available. However, beyond the attributes described here (version, language, platform), information systems tend to lack clear facets around which you can pivot the information. You mostly end up with keywords and tags.

In earlier posts on my blog, I explored adaptive displays of information through semantic tags quite a bit. For example, I based my 2013 keynote to the User Assistance conference on faceted classification (see [Making Cotnent More Findable When Users Browse and Search](http://idratherbewriting.com/2013/06/24/recording-of-making-content-more-findable-when-users-browse-and-search-ua-europe-presentation/)). I drank the Kool-Aid to excessive sugar highs ways when I read Dave Weinberger's book, [Everything is Miscellaneous](http://www.amazon.com/gp/product/B0029PSOOS/ref=as_li_qf_sp_asin_il_tl). Weinberger argues that most everything we have defies classification; it fits into a category of "miscellaneous." The classification schemes we use (from encyclopedic information to planets, libraries, and other supposedly objective knowledge systems) really just represent our own beliefs and priorities. As time changes, we see how our own thinking at that time inclined us to organize the information that way.

In reality, things in the world don't have such clear-cut categories and ordered absolutes. The world around us is ultimately miscellaneous, meaning, without clear division and order. Each thing has characteristics that overlap with other things &mdash; a classification that makes sense to one person doesn't make sense to another.

Rather than classifying things in absolute ways, or deciding what to include and exclude in systems, Weinberger argues that we should strive to add as much metadata to things as we can, and then manipulate the information in ways that make sense to each of us. (See my previous post, [On Metadata and Help Content](http://idratherbewriting.com/2013/05/27/on-metadata-and-help-content/) for a summary of Karen McGrane's presentation and emphasis on the same strategy.)

Weinberger isn't an XML consultant for documentation projects; in fact, he doesn't even mention documentation systems in his book. His concern is at a higher level, with the general Internet as the playing field. But certainly the idea of pushing and pulling content through metadata, based on a user's specific needs (with the context of their profile, language, location, and other details) has made its way into the documentation landscape and serves as a key message in documentation conferences.

For example, a previous theme in an [Intelligent Content Conference](http://www.intelligentcontentconference.com/) was to deliver "the right content in the right format to the right person," etc. In [How to Get the Right Content to the Right People at the Right Time](http://contentmarketinginstitute.com/2015/09/right-content-right-time/), Michele Linn explains that "this is what today's content creators must aim for." He lists the following ways content must align with the user:

> The right person to get
> The right content
> At the right place
> At the right time
> In the right format
> In the right language
> On the right device

These messages often accompany XML-related conferences, tools, or websites because XML's key selling point is its support for semantic tags. You can leverage these semantic tags for dynamic assembly of your information. As such, XML provides an incredible degree of flexibility and robustness to potentially meet the needs of complex documentation scenarios.

Semantic tagging is key to manipulating content into different arrangements at will. I explored this idea in more depth in a previous post on [the importance of chunking for sorting information](http://idratherbewriting.com/2011/04/18/the-importance-of-chunking-for-sorting).

Consider a work that is one large book, with no chunks at all. In that case, it would be impossible to sort anything differently, because you have just one object (one order, one sequence, one path). With one object, the only pattern you can configure is itself. But if you have a handful of objects, you can arrange those objects into as many patterns as you want.

Take 1,000 small rocks &mdash; the potential number of patterns you can configure is infinitely greater than the patterns you can configure with just a few rocks. If you walk along the trails in Moab (where the sandstone and dirt ground makes it difficult to see a defined path), you'll find many rock piles ("cairns") that act as guide points. The cairns can be stacked and arranged in many ways, because they consist of little chunks of granite:

<img src="/images/cairns.png" alt="cairns" width="449" height="449" class="alignnone size-full wp-image-22671" /></p>

But the big rocks are much more pattern-limited. They mostly just sit there, alone:

<img src="/images/bigrocks.png" alt="bigrocks" width="451" height="152" class="alignnone size-full wp-image-22672" />

Thus, if your goal is to manipulate content in a variety of nimble ways, pulling out bits and pieces to fit a specific user context at a specific time, you need to not only tag your content with the right metadata to surface such content, the content also needs to granular enough that it can be extracted and inserted elsewhere. This brings me to the most modern application of this idea &mdash; chatbot design and digital assistants.

## Chatbots

Today there's a lot of excitement around chatbots. A chatbot provides an automated response to a message the user submits. You ask the chatbot a question, and it magically returns the right information.

Try try out a chatbot, check out Verizon's "digital assistant" on their [Contact page](https://www.verizonwireless.com/support/contact-us/). Ask a question such as "do i need a sim chip"?

<a class="noExtIcon" href="https://www.verizonwireless.com/support/contact-us/"><img class="small" src="images/verizondigitalassistant1.png"></a>

Or "how do i activate my phone":

<a class="noExtIcon" href="https://www.verizonwireless.com/support/contact-us/"><img class="small" src="images/verizondigitalassistant2.png"></a>

Or even something specific to your account, such as "am I eligible to upgrade"?

<a class="noExtIcon" href="https://www.verizonwireless.com/support/contact-us/"><img class="small" src="images/verizonchatbot.png"></a>

The chatbot provides conversational AI for you to ask your questions. In order for the chatbot to return the right information for your context, your information must be chunked and tagged. The responses are the length of a tweet and often include links for more information.

Chatbots don't have a standard format for structuring information. There isn't a DITA or OpenAPI specification for chatbot information. There are dozens of different structures, much of them in JSON. Chatbot platforms often use an API to request information based on specific attributes. In designing the chatbot, you have to map the user's input to the returned information. The information is often returned through JSON and incorporated into the chatbot interface. (See [wit.ai](https://wit.ai/) for more details here.)

Here's my main point: *The chatbot model only works if your information is chunked into granular pieces and that tagged with the right metadata. Then it can be summoned at will and inserted into the chat user interface.*

Chatbots are mostly used in sales scenarios to provide simple information on websites. You won't find complex procedures returned in a chatbot UI. For example, the Verizon digital assistant won't return instructions on how to activate your phone. Likewise, you wouldn't need to chunk information on how to set up a router on a chatbot. Instead, you most likely submit the summaries or descriptions and include a link for more information.

Whether chatbots take off or not in documentation scenarios remains to be seen. Tech writers are in a good spot if their information is already chunked and tagged in a useful way.

Chatbots might be current hype, but the direction is not. The next trend after chatbots is pure voice interaction, such as with Alexa and the Echo. Alexa is a chatbot without the little chatbot window or other screen. The interface is ultimately your house or the objects around you (Internet of Things). You can ask Alexa questions such as:

* What's the weather like today?
* What movies are playing?
* Who was Abraham Lincoln?

Or if Alexa is integrated into other objects, such as your bathroom mirror, your car, your scale, and more, the information returned in a similar way. Alexa is the platform for an interactive voice interface.

We're in the early days of AI, but there's no reason to think the direction towards AI will change, especially as more inanimate objects come online through the Internet of things, voice interactions will be the norm. When you walk by your thermostat and say "I'm cold, can you turn up the heat a bit?" -- what should the object respond? When you turn on your TV and say, "What new shows are available?" how should the object respond? When you walk by a historical site and see a landmarker and ask "What was here 100 years ago?" how should the object respond?

Internet of things (IoT) is all about bringing objects that were traditionally offline online. Not just bringing them online, but enabling them to interact with each other. In the world of IoT, how will we design the responses of these interactions? Information will need to be chunked and granular, ready to be identified and returned at will based on the context the user presents.

## Challenges to writing chunked, tagged information

Conceptually, writing in small chunks that you tag and store as individual units seems like a great idea. But it's hard to implement. It can be challenging to write coherent, rich content with this approach. If you chunk everything up into little bits, then you end up storing those bits separately. Your page just has references to each of the little bits. As such, you can't easily read the page. You have to read the compiled version of the page to see the flow as a whole.

More difficult, you have to ensure that each chunk can have a consistent, understandable meaning when it's dynamically assembled into any new contexts. This makes you think deeply about the context of each chunk, and you might end up making the content more generic.

For example, chunking in a granular way constrains your ability to use links. Will the links always point to the right pages? What if the links point to the same page as the chunk itself?

Antecedents (references to other elements) can also be problematic. Can you say, "The code samples shown earlier demonstrate this approach." You'd have to only use this chunk on the same page where "this approach" is explained. Depending on the granularity of the chunks, making sure the chunks always make sense in their embedded context can be a mind-bender.

With content development hampered, the resulting content might not have the same rich story arc and flow as with long-form content. It depends on how granular you've chunked your content.

Overall, in your chunks of content, you might have hundreds of little chunks (whether single elements or entire topics) that exist in a large database, and each topic would contain an assembly of those chunks, or each map would contain an assembly of topics. But this wasn't the end goal we were aiming for. We wanted *dynamic* assembly of the chunks, not pre-built assemblies of chunks or topics.

One problem with a purely dynamic assembly is in how the search engines reliably index your content. If chunks live independently and pages are dynamically assembled, search engines can't index the pages because the pages as such don't really exist &mdash; they're just templates where chunks get dynamically assigned to appear on the fly. If there aren't fixed pages to index, how does the search engine crawl your content? 80% of hits on a web page typically come from search engines, so if users can't find your content through search engines, they might never find it.

Suppose you don't have a large database of individual floating chunks of content that are meaningless alone, but rather you have more mature, lengthier, standalone topics. And these topics are re-used in various locations based on different user contexts, journeys, workflows, and needs. Again, what does the search engine surface?

Google doesn't show the same topic multiple times in the search engine results page. Instead, it shows the "canonical" topic (which has a canonical link tag in the header). If that's missing, it shows the most popular topic (which might not be the version of the topic the user is searching for). Multiple instances of the same content repurposed in different guides and journeys might work in print-based media (common pre-2000), but it doesn't work so well online. Online, Google promotes only one instance of the page.

I'm not trying to undercut this model. I'm fully persuaded that in the future, content must be chunked and tagged to be usable by various systems. But it's a harder model to adopt and work in.

## Metadata

Let's jump more into the topic of metadata. You can't push and pull your content without metadata. Ideally, you should start out by identifying all the scenarios where you want to present the user with specific topics in a way that will help him or her wade through complexity. The more attributes you can pull from, the more intelligent your scripts can surface that content for the specific condition.

Here are a few scenarios:

* Show the user getting-started topics for the product
* Show troubleshooting topics for a product
* Show all versions of a topic
* Show topics related to the current topic the user is viewing
* Show the right programming code snippets based on the user's platform

You might have other tasks for metadata less related to user scenarios as well:

* List the time a topic was last reviewed, and by whom
* List all topics, by product, that require translation or which haven't been translated in the past year

Here are some ideas for metadata that a chunk of information might contain:

* title
* author
* product
* platform
* audience
* version
* last_reviewed
* product_owner
* reviewers
* other_languages
* last_translated
* content_type
* tags
* keywords
* description

Different metadata makes sense for different products, but this is a good start.
The challenge is adding all of this metadata to each of your pages in a consistent way. Even with static site generators that use Markdown, you can add custom metadata to each page through YAML syntax in the page's frontmatter. Then you create complex logic and algorithms to determine what pages surface. The challenge with static site generators is in ensuring the metadata is consistently tagged and applied. Authors need to be on board with the same approach both with labels and their values.

Some values, such as keywords, might make sense as arrays while other values can work as comma-separated values or single values. Some values need to be integers (to work in scripts) while others can be strings. It depends how you want to manipulate the data.

Typically, in platforms such as Jekyll, you can add semantic properties to a page in the page's frontmatter, which is set off by 3 hyphens, like this:

```yaml
title: My page
url: mypage.html
keywords:
- eggs
- bacon
- toast
description: A short description of the page
last_reviewed: 2018-01-20
```

You can also include properties in your configuration file that apply to all pages in a particular directory. For example, `product` or `author` might be more directory-applied properties like that.

(I'm just giving an example of how to add metadata to content. I work regularly with Jekyll, so it's what I'm most familiar with. If your platform is XML-based, you could probably add metadata to topics in a more robust way that you validate and enforce.)

With metadata available, you can then develop scripts to surface the content as appropriate for the context. One simple, concrete application of semantic tagging is to surface relevant related results based on this metadata. For this, you must tag your content with the right metadata to support the surfacing of content you want.

For example, suppose you wanted to show all pages containing the keyword "mac" that also have the keyword "getting started" and which were authored less than 1 year ago. You could add the appropriate metadata to your content and then write the scripts you need to surface the content.

## How does tagged, chunked content simplify complexity?

Let's return to our original problem: how do we simplify users paths in complex systems that define linear order? A lot of these metadata tags, such as author or content_type, won't necessarily simplify complexity. The trick is to figure out the right metadata that will allow you to surface the right content to users as they need it. Albers says,

> All the information possibly relevant to support addressing the user's goals and information needs simply cannot be dumped onto the screen. Nor can a hierarchy of links solve the design problem of effective information presentation.

In other words, you don't want to dump 25 links that all have the tag "configuration" onto the screen in front of the user. That approach is no better than if the user simply searched for "configuration." Instead, you need to use metadata intelligently to provide a refined, short list of highly relevant content in the right context. I know that I've only scratched the surface here, but hopefully I've pointed the discussion in the right direction.
