---
title: Reconstructing the absent user -- the essential requirement for writing good documentation
permalink: reconstructing-the-absent-user.html
published: false
---

{: .principle}
To write good documentation, you have to follow the most fundamental rule of writing: know your reader. The problem in tech comm is that the reader (or "user") is absent, and there aren't any direct measurable outcomes when users interact with the documentation. Consequently, tech writers suffer from lack of user knowledge and feedback, which usually leads to a poor user experience with docs. Writing good documentation requires you to reconstruct the absent user through web analytics, embedded surveys, milestone completions, support tickets, satisfaction surveys, and more. It is an iterative process where layers of user information get added little by little to form an image of the user, like a 3D printer slowly building a face. By acquiring and processing this user-rich knowledge, you can start to create good documentation that meets user's needs.

* TOC
{:toc}

## Are your docs good?

Our team was recently re-aligned during a reorganization, and in the new structure, an upper manager, trying to feel out how to manage the doc group, asked us this question: **How do you know if your documentation is good?**

It's a straightforward question, and one that presumably we should have an answer to. But the question prompted shrugs and meandering responses. We soon started looking at different efforts &mdash; metrics, surveys, support tickets, and more. But really, we didn't have a good answer to the question. We didn't know if our docs were any good.

This question gets to the heart of many challenges with tech comm. If you don't know if your docs are any good, how do you know whether users value or despise the docs, or if they even use the docs? If you don't know your documentation's value, then how do you know *your team's* value? If your team's value is unclear in the organization, how do you get funding, and headcount, and inclusion? So much depends on measuring your documentation's value to the user.

Surely, docs are valuable, but if we can't prove or measure the impact, then how do we know? How do we evaluate the work we put in each day &mdash; are we doing any good, or are we just spinning out information that no one reads or cares about? We hope users find the docs helpful, but if we can't measure its impact or success, then ultimately the value of our efforts are uncertain.

This question of documentation's value has been an unanswerable question since the beginning of tech comm &mdash; not just the value of documentation, but by association the value of tech comm. Saul Carliner, in an in-depth article on metrics and measurement, writes:

> Since the middle of the 19th century, then, technical communicators have been concerned about the value of our work. Almost 150 years later, our concern extends beyond whether the documentation is well-received. It focuses on justifying the need for organizations to continue employing technical communicators. More than being well-received, technical communication must provide tangible value to organizations by contributing to revenues, containing expenses, or helping an organization comply with regulations. ("We Are What We Measure: Towards Quality Metrics for Learning and Communication Products Used in the Workplace" *Technical Communication*, 2004)

Why has the question of documentation's value been unanswerable for *150 years*? Yikes! We're smart people. Why can't we figure it out?

In this post, I'll argue that the reason we don't know if our docs are good is because the user is absent from the tech writer's environment. Without the user present (or without copious feedback from users), judging or measuring the impact of the docs is nearly impossible. To write good documentation, you have to follow the most basic rule of writing: **know your reader**. If you don't know your reader, your docs will likely be bad &mdash; they will miss the user's information needs, technical level, and other concerns.

Reconstructing the absent user is a complex task. But because  most interactions take place online, users leave *digital trails* to follow. Users also leave  feedback through embedded surveys and other tools that technical writers can use. Support cases, milestone completions, and satisfaction surveys can also provide clues about this absent user's wants, needs, and concerns. By reconstructing as much of the user experience as possible, we can begin to write documentation that meets the user's needs. Documentation that meets user's needs can be considered "good documentation."

## The problem: The absent user

Many professions have a tangible outcome to measure their work, often gathered through direct interaction with users or from the user's transactions. For example:

* Doctors look at the health recovery rates of patients
* Teachers look at the grades and progress of their students
* Coaches look at their number of wins their team makes
* Marketers look at conversion rates for campaigns
* Detectives look at the number of criminals they find and prosecute
* Product managers look at the adoption rates among users
* Support agents look at the number of tickets resolved
* Business managers look at the number of products that users purchase, and so forth.

What do documentation professionals look at to measure their success? Logically, the number of users helped by the documentation. The problem is that these users aren't present, and their experience isn't captured, so it's difficult to know if these users even exist, and if so, what their experience was. They are in the ether, so to speak, and technical writers often end up looking at a wide, black expanse, with little sense of the user's documentation experience.

If we could observe users consulting the documentation as they struggled through a task or scratched their heads in confusion, and then finding or not finding the answer, we could get immediate feedback about the usefulness of the documentation. But about the only time you can get this type of feedback is through a usability lab, or by asking to observe a user in action.

Even if you were to bring users into a usability lab and watch them interact with docs, the scenario would be artificial. The tasks would likely be constructed and prompted, and not natural actions (for example, you might ask users to do something they don't know how to do nor really want to do, and then invite them to look in the docs for instruction on how to do it). Thus, even with usability labs, in our attempt to measure and evaluate the user experience, we distort it.

Because the user is absent, technical writers tend to be unaware of the impact of their documentation on users. Imagine this same absence in other professions:

* A teacher provides instruction to a room full of students positioned on the other side of a dark soundproof mirror, giving instruction and tests but never hearing student questions or test results. How can the teacher evaluate his or her effectiveness?
* A sales person gives his or her pitch to mute, invisible customers behind a wall, never hearing feedback or concerns from the customer, nor learning whether the customers make a purchase. How does the sales person know whether he or she is good at sales?
* A doctor provides health advice to a patient hidden behind an invisibility wall, with no ability to ask questions or receive answers, nor learn whether the advice given had an impact. Instead, the doctor just receives a piece of paper with a short list of symptoms. Is the doctor a good doctor, providing helpful advice? How would he or she possibly know?

In each of these scenarios, it's clear that the teacher, sales person, or doctor would likely give the wrong advice or address topics irrelevant and unhelpful to users. It's absurd to even consider these scenarios. Yet this is the scenario that tech writers face, and it's why documentation so often misses the mark. The most fundamental rule of all writing is to know the user. Without a knowledge of the user, your writing can never fully meet the user's needs.

Despite the need to understand the user and write for the user, technical writers typically write in isolation. A lot of us are introverts, we despise meetings, and we spend most of our time working on documentation in our cubes. We don't go figuratively knocking door to door on user's houses.

When it comes time for release, we throw our documentation over a wall to the users, and then return to our tech writing caves to continue working on the next batch of information. But we don't really see the users consume or interact with the information we heaved over the wall. We don't know if the information lays rotting and unused on the ground, or if it was eagerly consumed, or if the information made them sick, or anything. Without this knowledge, we keep on churning out the same kind of information, waiting for the next release window to again throw our docs over the wall.

## A thousand pieces rather than one or two

Despite the need to understand the user, the technical writing profession is mostly a solitary one, separated from end users. As a technical writer, I spend the majority of my day sitting at my computer, working alone on documentation. I'm writing for a user I almost never interact with. I make decisions about the language and terms the user will speak with, the tasks the user will want to do, the questions and problems the user will encounter, the business scenario and purpose the user will follow, and more &mdash; without the user present.

The most fundamental rule of writing is that you write for a reader, but if you have very little understanding or interaction with that reader, how can you possibly hope to connect with what the reader wants and needs to know? How can you write documentation that the user considers good? Is it any wonder why technical documentation as a whole tends to be constantly degraded and dismissed by users as unhelpful? How can we close the gap between these invisible, absent readers and make them present, so that our docs can be good?

Part of the problem around reconstructing the absent reader is that we look for a clearly identifiable source of information but can't find it. We expect user information to be channeled from product teams, or from UX personas and research. What if, instead of looking for these "showcase users," the task of identifying users is much more nuanced and granular?

Consider this analogy from the field of genomics. In a recent Freakonomics podcast called [Evolution, Accelerated](http://freakonomics.com/podcast/evolution-accelerated/), the hosts discuss the emerging science of gene editing. With gene editing, genetic engineers try to identify a corrupt gene and then catalyze the body's own repair process to fix it.

In the podcast, Jason Fletcher, economist and co-author of *The Genome Factor*, explains that when the human genome was first mapped, people assumed we would quickly be able to "find single, easily identifiable genes that controlled cancer, or depression, or intelligence, or even just height" &mdash; for example, the Alzheimer gene, the Gambling Addiction gene, the Depression gene.

Fletcher says this assumption was wrong, explaining that it "turns out to be an exception rather than a rule." Instead of single, easily identifiable genes responsible for our maladies, there are actually hundreds of thousands of genes contributing in microscopic ways to the result. Fletcher explains,

> Most of what we care about, most of life’s important outcomes, are not one gene and one disease. They’re more like hundreds or thousands of genes all with really tiny effects, if you can even find them.

Thus, even though the first human genome was [sequenced in 2003](https://en.wikipedia.org/wiki/Human_Genome_Project), we still don't have gene editing. Why? Because finding the genes responsible turned out to be much more complex than initially thought.

As technical writers, we're not mapping the human genome, but we are doing something similar: we're mapping the end-user; we're reconstructing the absent user. We might initially assume that the handful of personas from the UX team might suffice, or some other general target audience description. But what if this is the wrong way to go about understanding users?

Instead, we must reconstruct the absent reader in the same way a genetic engineer looks at variant DNA strands under a powerful microscope. We're figuratively trying to understand how the user's brain chemistry and wiring work, and how that user has interacted with our docs. By following the digital trails the user leaves, we ask what the user needed to know, wanted to know, did not know. We ask what actions or behaviors and thoughts drove the user's behavior. Who are the users, what  did they do with the information in the docs? Did they find answers? Did it help them?  

By examining a thousand strands of DNA, we begin to get a clear picture of the user experience. Each user leaves a digital trail that we can follow. By analyzing the digital trail, we can reconstruct the user (like an archeologist reconstructing a Paleolithic scene) and understand this user as if present. Closing this gap between the writer and reader constitutes one of the most important tasks in technical communication. In the absence of a real user, we end up writing for ourselves.

## The digital trail visible from web analytics

Although absent, users leave digital trails through documentation, most notably captured through web analytics. Web analytics provide the first, easiest clues about the user experience. Whether using Google Analytics, Adobe Analytics, or some other web analytics service, we can collect some basic information that lets us know the following:

* Number of page visits
* Number of pages viewed per visit
* Unique visitors versus returning visitors
* Time on page
* Referring pages, and more

Though basic, these metrics at least let you know what documentation pages users are hitting. They address the relevance aspect of documentation &mdash; are the tasks and information in the docs relevant to users? Is it what the users are looking for? Metrics don't reveal whether the documentation successfully helped the users with those tasks or answers -- you only get a sense of the following:

* Which topics seem to matter most to users
* How much time users are spending on those topics
* How users are arriving at the topics
* The location the users are originating from
* Other pages the user visits

When I look at documentation metrics gathered through analytics, here's what I learn. Users are mostly interested in specification information and getting started tutorials. They mostly arrive from Google, and they come from all over the world. Users spend less time on the page than I assume, and they might visit another half a page during their visit. If search queries are available (from site search), their queries tend to be short and general.

In looking at metrics, it's tempting to dismiss them for their lack of insight, or to look toward collecting even more information, something along the lines of big data. Could we find more answers if we had gigabytes of user data rolling in?

Several years ago, there was a lot of buzz about big data and the insights it would bring. With the ability to capture so much information, the unexpected correlations and predictions were highly anticipated. If you can capture information from every page event (every click, every scroll, every eye movement, every parameter from the user's browser, every action at every decision point, and more), and then number crunch this data to look for meaningful correlations, we might "be able to predict huge areas of the future with far greater accuracy than ever before in human history, including events long thought to be beyond the realm of human inference" (["Nine large problems with big data"](http://www.afr.com/technology/nine-large-problems-with-big-data-20140410-jya9k)).

But big data doesn't seem to have delivered on its promises, and the term "big data" appears much less these days. Why? Michael Salvo and Adam Strantz explain that "Big Data remains specialized, obfuscated, and elite. There is not yet a clear way forward. There is lots of potential evident in technology and analytic methods, but no clear, direct benefit for end-users" ([Wayfinding Big Data in Technical Communication](https://www.stc.org/intercom/2015/04/wayfinding-big-data-in-technical-communication/), *STC Intercom* 2015).

Instead of looking for answers in big data, we need to do a better job acting on the basic information we already have. An article in the *Harvard Business Review* explains companies that invest a lot in big data don't realize the payoffs because they can't even make use of the basic analytic information they already have. The authors explain:

> most companies don’t do a good job with the information they already have. They don’t know how to manage it, analyze it in ways that enhance their understanding, and then make changes in response to new insights. Companies don’t magically develop those competencies just because they’ve invested in high-end analytics tools. They first need to learn how to use the data already embedded in their core operating systems, much the way people must master arithmetic before they tackle algebra. Until a company learns how to use data and analysis to support its operating decisions, it will not be in a position to benefit from big data. ([You May Not Need Big Data After All](https://hbr.org/2013/12/you-may-not-need-big-data-after-all), Harvard Business Review 2013).

Let us pause for a few extra moments at the top viewed pages and see if we can pull out more details around the user experience from this information. How can we leverage this information to make some conclusions about the absent user's experience? Here are a few questions to ask:

* Why do these popular topics matter so much to readers? Are there top problems or questions users are running into that lead them to these topics?
* Do the topics in these popular topics align with any particular user demographic?
* What can user actually do with the information on these pages? Can we get a sense of their coding workflows and scenarios based on these topics?
* Conversely, what topics are users *not* viewing? What pages have the shortest page view time and the highest bounce rates?
* Can our popular topics be expanded with more in-depth information, further serving the user's information needs?
* Can we get rid of the information no one is viewing in order to increase focus on the content that matters to users?

The most popular topic in my documentation right now is the [Fire TV specifications](https://developer.amazon.com/docs/fire-tv/device-specifications.html). But ... *why specifications*? Specifications aren't tutorials, nor do they seem all that significant in the scope of how-to tasks and other troubleshooting information. It could be that end-users (customers) are inadvertently landing on this page rather than developers. But if the users are, in fact, developers, perhaps it means my users are advanced engineers, looking only for reference material rather than tutorials that hold their hand through a process. Perhaps it means they're coding features that depend on particular specification information (Android levels, OpenGL levels, Dolby support, processing speed, and so forth). Maybe their biggest decisions are around cross-platform compatibility and having the same experience across devices despite different device specifications?

You get the point. Rather than just glancing at the top pages and shrugging our shoulders, we can dive into the reasons why the topics are popular, and also expand on this information as well. When I [comprehensively reviewed the 2017 metrics](http://idratherbewriting.com/2018/01/11/comprehensive-metrics-for-idratherbewriting-in-2017/) for my blog, I found that many users were landing on my [Swagger tutorial page](http://idratherbewriting.com/learnapidoc/pubapis_swagger.html). Because of that, I added [extensive OpenAPI tutorials](http://idratherbewriting.com/learnapidoc/pubapis_openapi_step1_openapi_object.html) and other content in this same area to deepen the focus. It seems to be paying off, because the traffic is increasing.

Despite teasing more information out of the analytics data, we still can't entirely answer the question "Are my docs any good?" But analytics does help us determine whether we're addressing the right topics. Are we correctly identifying what questions users will have, what tasks they'll want to perform based on their various business goals and needs? If we don't get the needed topics right, then no matter how well a topic explains a procedure, if users are interested in another topic, the docs won't satisfy their needs.

But beyond alignment with the user's information needs, analytics don't get us inside the user's head to assess whether the content helped the user with those needs. For that, we have to turn to additional means of user analysis: surveys.

## Surveys as a means of getting user evaluations

Web analytics give us a sense of the user's interests, but remember our primary goal is to write docs that are good, and to do that, we need to understand more than just whether the topic is relevant &mdash; does the content actually satisfy the user's needs? How do we get this evaluative feedback?

One way is to ask users directly in the same context where they're retrieving and using the information. Through simple surveys embedded in each topic, we can collect feedback from users to help answer these questions.

It's not uncommon to see "Feedback" buttons on doc pages, giving users the ability to provide thumbs-up or thumbs-down reactions, or other simple feedback. Here's an example from YouTube:

<img src="images/likeordislikebuttons.png"/>

Every documentation page should probably have some type of feedback mechanism. In addition to simply letting the users give the information a thumbs up or down, ideally a free-form response field can capture more actionable information.

Recently, we experimented by adding a simple Feedback form in some of our docs (you can see an [example here](https://developer.amazon.com/docs/fire-tv/getting-started-developing-apps-and-games.html)). In our initial implementation, we just ask if the doc meets the user's needs. In about 2 weeks, for this particular doc set (which has about 60 topics), we received 20 responses. Sure, the number is small. But at least it gives us at least *some* glimpse of the user experience.

Other survey tools are more powerful. Take a look at [Usabilla.com](https://usabilla.com), for example. When you click the Feedback button Usabilla provides, you're prompted with options to either provide specific feedback or general feedback.

<img src="/images/usabilla.png"/>

If you choose to provide specific feedback, you can then highlight an area of the page you want to provide feedback about. I don't know how well this tool works, but it seems useful and interesting.

## Generalizing results from a small sample

If we capture only 1% of the user experience on these pages, how can we draw conclusions about the overall effectiveness of the documentation? With UX testing, Jakob Nielsen says that you don't need many respondents to conduct a successful UX review. For most UX evaluations, you need about 5 people, he says. With 5 people evaluating a UX, you will typically capture 80% of the feedback that you'll get with much larger responses. There's an effort-versus-response-value tradeoff that tends to drop off in efficiency after that.

Neilsen explains, "The main argument for small tests is simply return on investment: testing costs increase with each additional study participant, yet the number of findings quickly reaches the point of diminishing returns" ([How Many Test Users in a Usability Study?](https://www.nngroup.com/articles/how-many-test-users/)).

You could schedule dozens or hundreds of users in to evaluate an interface, but if, after the 5th user, you start seeing the same responses over and over, with little variation, then you're mostly wasting your time. You're spending lots of effort to confirm the feedback from the initial sample size.

I've seen similar results from blogging metrics. I've been blogging for a decade now, and after I publish a post, I'm eager to answer an similar question: was the post any good? Was the post a dud or a home run? I mostly measure the results through link tracking.

I use [Bitly](https://bitly.com) to track clicks on shared links in my newsletter, Twitter, and Linkedin. For my previous post, [Stoplight -- creating a single source of truth to drive the API lifecycle](http://idratherbewriting.com/2018/05/11/stoplight-and-api-doc-tools/), it received 403 clicks.

<img src="images/sharedlinksbitly.png" />

Just looking at the clicks in Bitly usually tells me whether the post connected with the audience or not. For more info, I can correlate these clicks with page views in Google Analytics, but the analytics usually just confirms the popularity of the post from the Bitly clicks. Any post that gets more than 300 clicks I consider successful.

Consider that the same proportions might be true for docs. How many users do you need to evaluate documentation? Do you need the responses for hundreds of thousands of users? What if you really only need the feedback from a small percentage of people in order to arrive at a conclusion that is mostly accurate? That sample size is completely viable through embedded surveys in docs, especially if those surveys are visible and well-integrated into the user's space. And when corroborated by numbers from web analytics, you can be more certain about your conclusions from the survey's small sample size.

## Support tickets and user forums

Another way to reconstruct the absent user is by looking at support tickets. Not every support ticket means a user consulted the documentation. Many support tickets might be filed in cases where users didn't use the documentation at all. But for those tickets that do show evidence of documentation usage (by either the user or support agent), the tickets can provide a more detailed narrative about the user.

Many times, before users contact support, they feel like they should do their due diligence in figuring out the answer for themselves. They might have tried using the docs but found they could not follow the task. Maybe the task was out of date, or missed some steps, or was designed for a user in a different environment. The support ticket usually provides a detailed thread because it allows a back-and-forth dialogue with the user.

It's not always easy to get this information from support. First, you might not have access to all the support tickets. For example, when users reach out through contact email, this exchange might go right into the support's case management tool, which only the support group can access.

Even if you could sort through the tickets with perfect transparency, you'd have to weed out tickets where docs weren't a factor. Then you'd also need to decide whether the docs weren't factor because of the following:

* The answer existed in the docs but the user couldn't find it
* The answer didn't exist in the docs but it should have been included

Finally, remember that support logs show only users that had problems. There could be thousands of experiences where users found the docs helpful and did have success &mdash; hence, they didn't need to reach out to support.

Thus, support provides a one-sided picture, only partly representing aspects of the user experience. Still, the information support provides is often more valuable because of its detail and actionable information.

Even a lack of support information can be telling. Few support tickets and a low amount of doc page views usually means no one is using the product. But few support tickets and a high number of doc page views can mean people are using the product and aren't finding issues with the docs.

## Customer milestones completions

Another data point to examine is whether users completed a particular milestone with the product. For example, did the user complete the setup, submit an app, start calling the API, or finish other specific end goal that you can track or measure? In the Appstore, I receive a weekly report about newly published apps. This is what most of my documentation aims to achieve &mdash; more published apps, which leads to greater selection in the Appstore.

However, we don't know whether the users consulted the docs to publish their apps or not. Maybe they had handholding from a field engineer; maybe they figured out the process on their own. Maybe they glanced at the docs only briefly; maybe they relied on the docs from the start to end. Maybe they relied heavily on docs from another source. Exactly what value and part the docs play in these milestones is a big unknown.

When users complete the project, we could reach out to them to find out if they used the docs, how much, whether they found them helpful, and so on. This kind of outreach to customers is usually restricted to specific teams (such as Support or Sales). But you could work through these teams to request specific questions that involve docs, and in so doing, start putting together a larger picture of the user experience.

Note that not every milestone is trackable. My documentation's scope is broader than simply publishing apps. In fact, most of the field engineers work with partners who already have published apps. They simply update their existing apps with enhancements &mdash; for example, implementing recommendations, or casting capabilities, or voice-enabled playback, and so on. How do we know when users relied on this documentation for their enhancements?

Sorting through the releases that leveraged documentation versus releases that didn't would be quite time consuming. Additionally, this approach neglects all the users who never reach the milestone because they failed. How do you even identify those users?

Although tracking milestones can provide more details about the absent reader of your docs, this method can't be relied on for a full and complete picture. But again, it is another strand of DNA that you add to the user picture you're continually drawing.

## Customer satisfaction scores

Another common area of feedback useful for reconstructing the absent user is the customer satisfaction survey. In these surveys, outreach groups ask developers a bundle of questions about their experience. You can often include some documentation-related questions here.

Note when you collect feedback from users, users will invariably mix any feedback about the docs with feedback about the general product, process, and other details. Saul Carliner explains that looking at customer satisfaction surveys as an attempt to get at measuring documentation has a lot of flaws. Carliner explains,

> ... many of the prevailing definitions of quality do not lend themselves to easy measurement if they lend themselves to measurement at all. For example, one group of definitions of quality pertains to customer satisfaction. But whose? Should technical communicators measure the satisfaction of the sponsors who commission the technical communication products (after all, these are the ones who authorize payment), of the executives who purchase the products and services that the technical communication products describe, or of the content's end users, who often have little or no say in the choice of the products and services they use? Or do technical communicators assess the satisfaction of all these groups, even though such an approach would be time consuming?

In other words, a customer might not be satisfied with the product. These satisfaction responses &mdash; even if specifically about documentation &mdash; are hard to separate from overall product feedback, which is beyond the control of the technical writer. Users rarely isolate their feedback to the documentation only. What would you imagine users would say? *Although I hated your product, I did feel that the grammar in the documentation was exquisite!*

Further, many tech writers have their hands tied about what they can and can't say in the docs. I've had product managers regularly edit out any sections on "Known Limitations" or bugs, and then we receive feedback from users who complain about a [lack of transparency](http://idratherbewriting.com/2017/07/13/transparency-in-documentation/). Product teams tend to have ownership over documentation, and simply overrule any honesty or transparency that tech writers want to "sneak in" to the docs.

## Conclusion

Unlike other professions that have more direct interactions with users, technical writers have to go out of their way to gather and interpret user data. Web metrics, embedded surveys, customer support, customer milestones, and customer satisfaction surveys can all help you construct the absent user. Understanding the users and their experience with docs is essential for determining whether the documentation is any good.

One or two methods in isolation might provide distorted results, but the combined picture across these five approaches will fill in gaps and corroborate data in a more balanced way. Especially as you look at this information through multiple iterations and feedback cycles, you'll begin to feel more confident about the user's experience. When you know your user, you can then write good documentation.

If you need a specific measurement, you could quantify the responses in each of these areas, projecting a kind of scorecard for a product's documentation. This scorecard, which draws upon web metrics, embedded surveys, customer support, customer milestones, and customer satisfaction surveys, will give a more reliable and comprehensive view of the user experience than any single metric or variable alone.
