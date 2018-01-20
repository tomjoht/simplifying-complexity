---
title: Wayfinding
permalink: wayfinding.html
published: false
---

## Action 6: Hang signposts along the way

<a href="https://developer.amazon.com/public/solutions/devices/fire-tv/docs/fire-app-builder-set-up-recipes-categories"><img src="images/amazonsignposts.png"/></a>

### Wayfinding

<img src="images/wtd_doc_navigation_wayfinding.svg" class="vectorStyle"/>

In the previous section, I explored modularity and noted that it usually results in longer topics. As much as you may strive for standalone articles, it's often necessary to break content for the same general procedure or larger task into multiple pages. If so, you can implement wayfinding techniques to help users successfully navigate across the content.

<div class="bs-callout bs-callout-primary"><b>Wayfinding: </b>"The process of using spatial and environmental information to navigate to a destination.""</div>

In documentation, wayfinding techniques might include providing contextual links, workflow maps, next steps, and breadcrumbs to help orient users as to where they are in a larger system.

### Provide context before

At the start of a topic, if you expect the user to have some context or background information, add some links for that context. The links usually go to an overview page or some other conceptual foundation.

If the topic is one among multiple in a larger procedure, you can embed a workflow map at the top of the page to let the user know where he or she is in a larger process.

<a href="http://docs.aws.amazon.com/AmazonS3/latest/gsg/PuttingAnObjectInABucket.html"><img src="images/aws.png" style="vectorImage" /></a>

### On-page-TOC

As the user navigates the content, the on-page TOC lets a user see the content at a glance. It lets users click to the section they're interested in, without requiring the user to manually scroll or skim the page for the information.

Here's an example of an on-page TOC from Amazon's documentation:

<a href="https://developer.amazon.com/public/solutions/devices/fire-tv/docs/fire-app-builder-overview"><img src="images/fabtoc.png" style="vectorImage" /></a>

When you create the on-page TOC, make sure it's scannable. Avoid including too many levels, as this detail might detract from the user's ability to take in the content at a glance.

Additionally, don't try to stuff the on-page TOC into the navigation sidebar (mixing heading links with links to other pages). Doing so unnecessarily balloons the sidebar with too many options, giving the impression that your documentation contains a *massive* set of pages to navigate and learn. (Users may often feel relief to realize that the sidebar links are actually just sections.)

Users don't usually need all the information up front but can instead view more detail as they drill deeper into the site ("progressive disclosure").

### Provide Next Steps

At the end of the topic, provide a "Next Steps" section that guides users to the logical next steps.

<a href="https://www.firebase.com/docs/web/guide/saving-data.html"><img src="images/firebase.png" /></a>

Even if you're not outlining a larger process or sequence, suggest a next move for the user. What else can/should users do at this point?

### Breadcrumbs

Finally, you can add breadcrumbs so that users have a sense of where they are in a larger system. The breadcrumb can be especially helpful when users land on a page in the middle of a help system.

<a href="https://developers.facebook.com/docs/accountkit/countrycodes"><img src="images/facebookbreadcrumbs.png"/></a>

The breadcrumb helps users orient their location on a map.
