---
title: Progressive disclosure
permalink: progressive-disclosure.html
published: false
---

## Action 2: Navigate from doc set to doc set

After I right-sized the product sidebar at my company, I had a handful of different sidebars to manage. Remember I said the sidebar shouldn't be so massive that it contains endless pages of nested documentation. As a result, I had about 4 other sidebars scoped to somewhat different or related products.

Additionally, there were some other doc sets that would be relevant to users, which were owned by other writers. I put a "Related Resources" section at the bottom of the sidebar that would allow users to easily navigate to other sidebars.

<img src="https://idratherbewritingmedia.com/images/simplifying-complexity/navamongdocsets.png"/>

We also created a [doc index page](https://developer.amazon.com/documentation) that listed all the different documentation across the site.

### Design principle: Progressive disclosure

<img src="https://idratherbewritingmedia.com/images/simplifying-complexity/wtd_doc_navigation_entrypoint.svg" class="vectorStyle" />

Progressive disclosure is almost redundant from the previous section but is worth calling out here since it acts as a primary tool in your usability toolbox.

<div class="bs-callout bs-callout-primary"><b>Progressive disclosure:</b> "A strategy for managing information complexity in which only necessary or requested information is displayed at any given time."</p> &mdash; [Universal Principles of Design](https://www.amazon.com/Universal-Principles-Design-William-Lidwell/dp/1592530079)</div>

The basic idea of progressive disclosure is to layer your information at different levels. Designers creating mocks for websites regularly consider these different levels in their UI layouts. I remember the last time I evaluated some comps from a UX designer. He pointed out the type of information that would appear to users at level 1, level 2, level 3, and level 4.

In techwriterville, we usually operate at one level and don't have this multi-tiered approach to information in our list of concerns. But it's helpful to model your information by thinking about what is exposed at each level of the user experience.

The most common application of progressive disclosure is with context-sensitive help. Provide little tooltips or other on-screen text in your user interface and let the user click for more information if desired.

That's a great strategy if your product has a user interface, but if you're working with developer documentation and APIs, there may not actually be any such UI to hang this information.

The way progressive disclosure applies here is with the layers of information exposed by the sidebar. Think about the type of information shown at these levels:

* Doc portal homepage (Level 1)
* Product homepage (Level 2)
* Section homepage (Level 3)
* Page (Level 4)

You can think of these points as levels 1 through 4. What information should you show to users at each level?

Beyond layers of information, you can also start by showing basic information first and more advanced information at different stages. According to Jakob Nielsen:

> Progressive disclosure is the best tool so far: show people the basics first, and once they understand that, allow them to get to the expert features. But don't show everything all at once or you will only confuse people and they will waste endless time messing with features that they don't need yet.</blockquote>
&mdash; <a href="https://www.interaction-design.org/encyclopedia/progressive_disclosure.html">Interaction Design</a>

### Doc portal homepage

It depends on the size and scope of your products and documentation, but generally the doc portal homepage likely lists the various product documentation available.  

Here's an example with Microsoft's Azure documentation.

<a href="https://docs.microsoft.com/en-us/"><img src="https://idratherbewritingmedia.com/images/simplifying-complexity/azurehomepage.png"/></a>

The doc portal homepage should list out the documentation in a way that makes sense, such as by product and version, or by user role or goal. The grouping should be helpful for users to see what's available, to orient themselves in the right direction, and to get started.

I like to think of the doc portal homepage as a train station. It should clearly direct users on where to go.

<figure><a href="https://www.flickr.com/photos/nathancongleton/14806700660/"><img src="https://idratherbewritingmedia.com/images/simplifying-complexity/trainstation.jpg"/></a><figcaption><small>From Flickr by Nathan Congleton</small></figcaption></figure>

The homepage isn't a destination page in itself with explanatory information. Instead, it directs users to the correct "terminals" for their documentation routes.

I like the visual attractiveness of cards on the homepage. These cards draw the eye and invite you to click and explore them. They're a good way to give balance and visual appeal to what would otherwise be a list of links. The card design on the homepage is a common pattern with documentation.

That said, a list of links (such as with [AWS](https://aws.amazon.com/documentation/)) also works if you have a lot of different doc sets. The list format allows users to quickly scan the page and take in the whole at a glance, which is a principle I'll explore more later. You also don't have to scramble/brainstorm for graphic representations of your documentation.

Users start forming opinions and biases about the documentation from this first entry point. If the entry point is disorganized and doesn't help them get started, the user's confidence is already crippled as they head into the rest of the documentation.

### Product homepage

When you click into a product homepage, the navigation sidebar should show links for that product. The scope and focus of the information changes to become more specific to the product.

A *product* homepage is not so much a train station terminal for routing; instead, it's more of a welcoming party. You've already taken the train to the new city, and now you've arrived. The product homepage is like that welcoming station, with a visitor center that gives you information about the city (recommended attractions, restaurants, walking tour maps, audio tours, etc.).

On the product homepage, you might list a getting started or Hello World tutorial or other beginner task (e.g, a tour of the app, or the most popular tasks). The information should act as a progressive lure to pull users into the system. Additionally, quick reference guides or other getting started tasks would be appropriate on the product homepage.

Overall, users come to the homepage to figure out where to go, to see what's available, and to get oriented. Try to make it as easy as possible for them to do get started.

### Section homepage

Whether you have a section homepage or not depends on the size of your information. At any rate, the section homepage is a microcosm of the product homepage, except that it's more focused on a sub-topic within the product.

For example, if your product contains various widgets, your section homepage might provide an overview of the available widgets, with links to the pages for the widgets. If your sections are huge (e.g., 20-30 pages per section), you might narrow the scope of the sidebar to just show pages within that section (with navigation to go to the other sections).

### Page

Finally, we arrive at the page level. The page level should provide an on-page table of contents that let's users know the scope of information at that page. Users shouldn't have to manually scroll the page to get a sense of the information the page contains.

Manually scrolling the page doesn't let users see the h2, h3, and possibly h4 heading levels that give users a sense of the information. The on-page TOC performs the same function as the sidebar TOC in giving users a sense of the whole, except that the on-page TOC is a microcosm with a much narrower scope.
