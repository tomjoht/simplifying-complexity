---
title: Iterative development of content
permalink: /iterative-development-of-content.html
published: false
---

# Iterations
#simplifying complexity#

layer two: the structure of story
——

# Iterate and increment to improve the quality of content
{: .principle}
Principle: Iterative development is a principle of design that applies as much to documentation as it does to software development and UX design. With iterative development, you continually improve the  content by gathering feedback and then incorporate the feedback as appropriate into new iterations of the content. You write in a shorter cycles with increased feedback reviews, working on developing content over a longer period of time rather than a short burst of writing activity in a one-and-done type effort. This iterative approach better addresses scenarios involving complex documentation where the audience, needed information, steps, and other details are uncertain and unpredictable.

## Iterating on a  doc 12 times
I recently worked on a documentation topic for a new feature that went through many iterations with product teams, stakeholders, field engineers, and others over a short period of time.  At first, I made a few revisions to the content based on reviews with the engineering team. Then when the reviewers expanded to field engineers and stakeholders, the number of iterations increased to nearly a new version every couple of days. With each iteration, we incorporated feedback to improve the document. After 12 iterations, we moved the document to the next phase of review with early release partners.

This project made me reflect on a principle that is central for nearly every type of writing project: iterative content development. Too often, people consider writing as an activity they can do once and then be done with for good. For example, students writing essays might wait until a few days before the essay is due (or worse, the night before), and then sink a few hours into content development and be done. They turn the essay in, get a grade, and then never revisit the content.  The same might be said for product teams writing docs the week before release.  After the docs have been written and product released, the doc is done.

This is not the formula for developing good content. To develop good content, you need to push the content through multiple iterations of review and edits based on incoming feedback. It’s rare that you hit the target on the first try. For example, in writing this topic, I will likely let the first draft sit a few days before editing it again. After a few rounds of initial edits, I’ll push it out for others to read. Based on the feedback, I’ll edit it some more, and then after some months I’ll return to it with fresh eyes to review and edit it again, and so forth. Each time I hope to move the content closer to perfection.

With tech comm content, the iterative process is the same as with other types of writing, but the forms of review differ. Feedback comes in through the project team, through support teams working with customers on issues, through feedback forms, metrics, and other channels. We can incorporate this feedback to iterate and increment the content, improving its value to users each time.

In an ideal world, content would improve each time it gets used, like a stiff baseball mitt becoming more worked in with each catch. The questions, issues, or other feedback from each person who uses the content would be relayed back to the writer to enhance the content  — fixing errors related to accuracy, correctness, completeness, coverage, and more.

Iteration is a central development of content, and the web provides optimal tooling for continually improving content. With printed material, including PDF, content is more static. The paradigm of printed material is that once printed, it is mostly finished/final. But with web content, you can subtly introduce incremental improvements without requiring the user to re-download or re-purchase a physical object to get the enhanced content. This is the approach I’ve used in developing my [API documentation course](/learnapidoc). I’ve been incrementally improving this content over the past 3 years. In fact, iterative improvement is one of the characteristics that separates blog posts (usually one-off writing efforts) from documentation content (which is supported, maintained, and improved over time). It’s why documentation has a higher lifetime value than blog posts.

## Why this is a complex scenario
Before we dive into iterative development, let me explain why this principle deserves a space in the Simplifying Complexity series. Isn’t iteration a principle behind _all_,  writing not just complex scenarios?

Sure, while iterative development is a good idea regardless of the complexity of the content, with complex content there’s a much greater need for iterations because you rarely hit the target on the first try. With complex scenarios, there are a variety of use cases and users that you’re negotiating as you write the content. What might be right for one type of user might not work for another.

Software itself can also be a moving target, with developers adding or modifying or removing features on a weekly basis. With the scenario I described earlier, at one point the product team decided to split the rollout into two phases, so half the documentation was literally postponed. What’s in, what’s out, and what’s coming and when is also sometimes unclear.

Also, as with almost all doc scenarios, the user is absent, and so the writer must constantly make guesses  (hopefully informed ones) about the user’s technical level, information needs, development environment, and business goals. I explored this in depth in [Principle 6: Reconstruct the absent user | Simplifying Complexity](https://idratherbewriting.com/simplifying-complexity/reconstructing-the-absent-user.html). Without the many user types present, whether your content connects with their needs is often questionable and only confirmed in hindsight.

Overall, technical documentation faces the same challenges as software development. It’s nearly impossible to predict whether your product will meet the user’s needs until you release it to the audience. Especially with highly complex products that involve a lot of different variables, conditions, environments, and business goals, iteration is essential to eventually getting it right.

In an extreme example, think of the Rubik’s Cube. In an ideal world, you should take the least number of turns required to solve it. But this is not how it’s solved. You can’t strategically plan all your moves in advance and then solve the Rubik’s Cube in under 20 seconds. To solve it, you usually make a lot of unnecessary spins and turns as you try to move closer to your goal. Think of writing documentation for complex software products somewhat like playing Rubik’s cube, only you have the benefit of feedback to guide each new strategy of twists and turns.

## Agile development is software development’s approach to handling complexity
As we investigate iterative development, it’s important to note that iterative development is a distinguishing element of agile software development, which evolved from waterfall methods to address the uncertainties and unknowns in a more strategic way.

Waterfall approached projects with a heavy amount of up-front planning and scoping of requirements, resources, and timelines. However, despite the careful planning and strategic analysis, waterfall projects were regularly over-budget and past-deadline. In fact, according to studies, McKinsey and Oxford University found that

> “large software projects on average run 66 percent over budget and 33 percent over schedule; as many as 17 percent of projects go so badly that they can threaten the very existence of the company.” ([Achieving success in large, complex software projects | McKinsey](https://www.mckinsey.com/business-functions/digital-mckinsey/our-insights/achieving-success-in-large-complex-software-projects). )  

Why did so many waterfall projects run over budget and past schedule? Is it because the project managers were poor estimators of the work involved? Is it because they under-bid costs in order to secure project funding? Not really. It’s because software development is a complex undertaking, and you can’t know all the details  from the start. It’s like planning your life for the next decade. You can’t know everything that’s going to happen ahead of time; sometimes you won’t know what you have to face until you get into the nitty gritty details of something and see out what challenges, incompatibilities, and other complexities surface.

Software development’s big revolution away from waterfall to agile involved shortening the development cycle and incorporating regular  product reviews. You code for a couple of weeks and then release something that you can show to customers or stakeholders. You gather their feedback to make sure you’re on track. With each iteration, you might find yourself abandoning ideas or redoing features with another approach — essentially iterating on the same efforts until you get it right. If you find that you’re going in the wrong direction, well then you’ve “failed fast” and can course correct early on.

In contrast, if you isolate yourself in development tasks for 2 years before touching base with customers to see if you’re on track, you’ll likely find that you veered off course long ago.  Spence and Bitner explain that agile software development follows more of a scientific hypothesis model, where theories are frequently tested to see if they’re correct. They write,

> In a sense, many things on a software development project are theories, or more accurately, assertions that need to be evaluated. The plan itself is composed of many assertions about how long things will take to accomplish. Even the requirements are assertions about the characteristics of a suitable solution. Just because some stakeholders or subject matter experts say a requirement is valid does not mean that they are correct. We need to evaluate even the requirements to determine whether they define the right solution to the problem at hand. ([What is iterative development? — Part 1: The developer perspective](https://www.ibm.com/developerworks/rational/library/mar05/bittner/index.html))  

To apply this same principle to documentation, consider that documentation is a plan — a theory you construct about how users will potentially be able to achieve their goals. But you don’t know if your theory is correct. You need to release the theory into the wild and observe the results: did the theory hold true? did the theory have shortcomings? Then based on the feedback, you can iterate on your theory to bring it closer to the reality.

UX design follows a similar iterative process as software development. Jakob Nielsen explains,

> It has long been recognized … that user interfaces should be designed iteratively in almost all cases because it is virtually impossible to design a user interface that has no usability problems from the start.  ([Iterative Design of User Interfaces](https://www.nngroup.com/articles/iterative-design/))  

If product teams could accurately describe all requirements from the start, what need would there be for usability testing at all? With product requirements and prototypes defined up front, the success of the project would rest in executing the requirements. But that’s not how it works because both software development and UX design is a complex endeavor. You make an attempt based on your best effort, you get some feedback from users, and then you iterate on a new version that hopefully gets you closer to what users want and need.

Iterative development is a cornerstone in agile processes. In fact, the _Scrum Guide_ describes scrum (a method for agile) as a “framework for developing, delivering, and sustaining _complex_ products” (my emphasis). In other words, agile is a response to the complexity of projects. If projects weren’t complex, the waterfall approach would have been fine. As such, if agile is an approach for building complex software products, shouldn’t it also be the approach for building complex software documentation?

Much has been written about how documentation can align with the development cycles and pace of agile software development. Most commonly, the advice for creating delivery docs that customers will read is to [document late](http://agilemodeling.com/essays/documentLate.htm) to avoid “treading heavy.” In other words, if the project is in constant flux, don’t waste a lot of bandwidth and cycles updating your documentation. Wait until the dust settles a bit, and then create your customer documentation.

While this approach is sound for working with agile projects, it misses the whole point of the agile development philosophy in documentation’s own development process. It assumes that writing is a one-and-done effort. “Document late” is the same practice that students adopt in college writing courses: wait until the last weekend before a deadline, and then write your essay. Wait until just before your customer release, and then write your docs.

In this view, writing is a simple effort that you can hit on your first try. You’re just describing what engineers have built, right? As such, it should be straightforward and direct. The uncertainty and ambiguity of the project were already handled by the many iterations that the product team previously went through in creating the product features, right? Except that for some reason, documentation always seems to suck. I wonder why that is ….

I’m not advocating that writers try to write documentation with each sprint, keeping pace with the constant changes and flux of a product under development. I also recommend starting documentation late in the project as well. But where iterative development with the software product ends, iterative development with the documentation should be begin. Documentation itself should undergo the same iterations and cycles of review, similar to the software development process. At this point documentation should be seen as its own project and life cycle, independent of the software project itself.

In _Agile Modeling_, Scott Ambler and Associates explain:

> Ideally you should create documentation throughout the entire software development lifecycle (SDLC) when it makes the most sense, albeit that's usually towards the end of the lifecycle. When you do write documentation, you should take an evolutionary (iterative and incremental) approach to its development so that you gain feedback as to its actual value. In other words, write a little bit, show it to someone, get feedback, act on that feedback, and then iterate. The best documents are written iterative, not all at once. An iterative approach enables you to home in on what the audience for your documentation actually needs.  ([Core Practices for Agile/Lean Documentation](http://www.agilemodeling.com/essays/agileDocumentationBestPractices.htm))  

Ambler agrees with the agile approach to writing documentation. He leans toward writing late, but that late timeline doesn’t mean a one-and-done effort. Instead, just as with agile software development, with agile doc development you shorten your publishing cycle and intersperse it with constant feedback to increment with each iteration.

## Ways to iterate on docs
In iterative design, it’s important to note that with each iteration, you should be incrementing your design to bring it closer to what users need. Iteration alone doesn’t necessarily imply progress. You’ve got to base the improvements off of some feedback that will move you forward.

How do you get this feedback? You can start by using yourself as a user. Go through the steps or other material yourself, making sure you’ve accurately described everything. A lot of times, tech writers whiz through a process too quickly and often miss steps or other areas.

In [Reciprocal knowledge networks and the iFixit Technical Writing Project — Conversation with Guiseppe Getto](https://idratherbewriting.com/2018/07/25/how-the-network-shapes-knowledge-conversation-with-guiseppe-getto/), Getto explains that he has students participate in iFixit projects (smartphone repair) as a way to better understand the documentation process. One student, reflecting on what he learned, noted, “you really have to check and recheck and recheck your information to be a technical writer.” Another student said, “Each time our group was hoping to be finished with our guides, there was another area to improve, correct, or modify.”

By triple-checking the information yourself (and of course walking through the steps yourself) you can ensure some level of completeness. But the larger reason Getto immerses students in iFixit project isn’t to convey a sense of meticulousness within the writer’s own work. It’s to put students “in scenarios that mimic real-world technical communication situations as closely as possible.” In the real world, projects aren’t finished when you turn them in. By participating in iFixit, students learn that documentation needs to continually evolve based on feedback from the wiki moderators, from users interacting with the instructions, from other writers, from product updates, and more. Documentation is one node in an interconnected network of other nodes that are constantly in flux. As these other elements change, the documentation needs to also change.

Getto calls this idea “networked rhetoric,” which refers to the shaping influences of the network on the content. Even non-human actors (the tools used to author and publish, for example, or the tools used for repair, such a a spudger) influence the documentation.

As we look to gather feedback, we should look at the network that the documentation rests in, and see how each actor in this network might influence the documentation. Some actors in the network involve the product team, the stakeholders, the target users, the device_software product, the authoring_publishing system, the support team, field engineers, other documentation in the same developer portal, and more.

I won’t go into detail about the myriad ways you can collect feedback. Here are a few ideas:

* Review the content with the product team prior to release
* Conduct informal usability tests of the content with engineers outside the product team
* Monitor support cases related to your product
* Ask field engineers working with the product for feedback
* Monitor the web for industry changes related to the product
* Other documentation (from other products) that impacts this documentation





Getto is fascinated by the reciprocal influences of the network and the “ In Networked Rhetoric: iFixit and the Social Impact of Knowledge Work, Getto explains how the network (every aspect of it, both human and non-human) shapes and influences the documentation.






how many times have you gone through the instructions yourself? you can probably get most of the way through yourself.

 how can you capture the feedback every time someone goes through something?

— feedback mechanisms on docs
— comment forms on content. forms below posts works quite well. people worry too much about abuse of this feature.
— watch users go through topics
— integrate your content into a network that will incorporate feedback loops. Gusieppe article

One of the students wrote, reflecting on what he learned from the project, “you really have to check and recheck and recheck your information to be a technical writer.”Another student said, “Each time our group was hoping to be finished with our guides, there was another area to improve, correct, or modify.” It seems that while you were more interested in the reciprocal influences within the network that contribute to the creation of knowledge, your student’s takeaway here is mostly that he needed to triple-check his work.

Typically, even as technical communication professionals, there’s a certain writing process we teach. It goes something like: stage 1) research the writing situation, stage 2) draft a document, stage 3) peer review, stage 4) revise. And there’s nothing wrong with this writing process. It roughly resembles what all technical communicators do, to some extent. Its economical in that it fits within a learning module within an academic classroom.

But the issue is that when you’re writing in an actual industry context, the devil’s in the details. From my research, and also my work as a consultant, I know that some of those writing processes take months or even years and involve a small army of people. The docs are vetted by tons of SMEs and every time they get vetted there needs to be another peer review process, another revision, etc. until finally the document meets quality standards (or it’s just due to the client, whichever comes first).



## The curve of useful feedback
— log trajectory
— must also factor in ROT. not a static environment. devs constantly change things.
**“The first few iterations can probably be expected to result in major gains in usability as the true "usability catastrophes" are found and fixed. Later iterations have progressively smaller potential for improvements as the major usability problems are eliminated, and the design may eventually become so polished that very little potential for further improvement would remain.”https://www.nngroup.com/articles/iterative-design/**


## Iteration versus incrementation
— how to capture feedback with each page view
— feedback form. when i add to docs, very little feedback comes in

**3. is there a possibility that you’ve iterated too many times on something so that you can no longer see it and it loses its original coherence/?**

**Sadly, development can be iterative without being incremental. For example, the activities can be applied over and over again in an iterative fashion without growing the understanding of the problem or the extent of the solution, in effect leaving the project where it was before the iteration started.” https://www.ibm.com/developerworks/rational/library/mar05/bittner/index.html**

## Infinite iterations and project/budget realities
— the longer you work at a company, the more you get pulled in different ways y projects.
— no one plans for long-term maintenance

## Blogs can be an iterative way to write books
— outside of tech comm concerns, but when writing a massive project, probably best to do it incrementally.
— this is genius of the web. bit by bit
— this is also why i dislike PDFs. too static.
— wikis as example of iterative content

**Perhaps the best example of iterative design on the web is the use of Wikis. Wikipedia, for example, contains user generated content. Anyone is free to come along and improve on that content at any time. It’s easy for a reviewer (or editor) to visit that improvement and make a decision as to whether the change is an improvement or whether it takes something away instead. Over time, the theory is that Wikipedia’s content should evolve to make it the most valuable encyclopedia online.**

**It’s worth noting that this approach to iteration in design is a challenging one. With a huge community to draw on, one person’s “improvement” may well be another’s “detriment”. When using an iterative approach in your own design process, it’s likely that you will have more control over the decision making process than Wikipedia does. https://www.interaction-design.org/literature/article/design-iteration-brings-powerful-results-so-do-it-again-designer**



——
References

Sriram Chandrasekaran, Sauri Gudlavalleti, and Sanjay Kaniyar. [Achieving success in large, complex software projects]([Achieving success in large, complex software projects | McKinsey](https://www.mckinsey.com/business-functions/digital-mckinsey/our-insights/achieving-success-in-large-complex-software-projects). July 2014.

Ian Spence and Kurt Bittner. ([What is iterative development? — Part 1: The developer perspective](https://www.ibm.com/developerworks/rational/library/mar05/bittner/index.html)) IBM Developer Works. March 15, 2005

The Scrum Guide. Nov 2017. [Scrum Guide | Scrum Guides](https://www.scrumguides.org/scrum-guide.html)

[Document Late: An Agile Core Practice]([Document Late: An Agile Core Practice](http://agilemodeling.com/essays/documentLate.htm). Agile Modeling. 2004-2018.

Nielsen, Jakob. [Iterative Design of User Interfaces](https://www.nngroup.com/articles/iterative-design/). Nielsen Norman Group. Nov 1, 1993.

Scott Ambler & Associates. _Agile Modeling._ [Core Practices for Agile/Lean Documentation](http://www.agilemodeling.com/essays/agileDocumentationBestPractices.htm))

Johnson, Tom.  [Reciprocal knowledge networks and the iFixit Technical Writing Project — Conversation with Guiseppe Getto](https://idratherbewriting.com/2018/07/25/how-the-network-shapes-knowledge-conversation-with-guiseppe-getto/). Jul 25, 2018.  idratherbewriting.com.

Getto, Guiseppe. [Networked Rhetoric: iFixit and the Social Impact of Knowledge Work - TechComm](https://www.stc.org/techcomm/2014/09/11/networked-rhetoric-ifixit-and-the-social-impact-of-knowledge-work/), Technical Communication Journal. 61.3, AUGUST 2014

——


———
layer one: the foundation of ideas

note in your book that you want to focus on some topics that aren’t immediately obvious. one of these is iterations. **every time someone uses a topic, we should gather feedback about this topic. this feedback can then be used to improve the content.**

**why is this in the simplifying complexity series?**

look at the networked rhetoric article. every time you get feedback, it improves something.

**we greatly underestimate the amount of care it takes to get information right. that quote from the student who says he was shocked by how many times he had to edit a procedure to get it right.**

1. why do you think iterations are so important?
**2. how can you capture the feedback every time someone goes through something?**
**3. is there a possibility that you’ve iterated too many times on something so that you can no longer see it and it loses its original coherence/?**
4. is history or a tradition that has evolved over hundreds of years more advanced than places that are  more new?
**5. what are some examples of iterative systems? what is something that gets better the more it gets used**
6. what is the agile concept of user testing?
7. why don’t docs do user testing?
8. does hegel’s ideas about thesis antithesis synthesis come into play here? is there a dialectic that is going on that is driving forward a progress in a topic? like the users are the dialectic?
9. what are some sample processes that involve a lot of iteration? [Ideate, Combine and Iterate: The Ultimate Process to Create a Better User Interface | Adobe Blog](https://theblog.adobe.com/ideate-combine-and-iterate-the-ultimate-process-to-create-a-better-user-interface/)
10. can you apply iterative design to this problem? [Iterative design - Wikipedia](https://en.wikipedia.org/wiki/Iterative_design)
The typical steps of iterative design in user interfaces are as follows:

Complete an initial interface design
Present the design to several test users
Note any problems had by the test user
Refine interface to account for/fix the problems
Repeat steps 2-4 until user interface problems are resolved

why don’t we expose docs to several test users?

docs aren’t tested. why not? this is a huge flaw in things.

Iterative design is a way of confronting the reality of unpredictable user needs and behaviors that can lead to sweeping and fundamental changes in a design. User testing will often show that even carefully evaluated ideas will be inadequate when confronted with a user test. Thus, it is important that the flexibility of the iterative design’s implementation approach extends as far into the system as possible.” [Iterative design - Wikipedia](https://en.wikipedia.org/wiki/Iterative_design)

the AVL docs are a great example of this.

titles: “information design for complex information”
for your activities, have the user focus on their own docs. they should answer a series of questions about their docs and then apply these principles where appropriate.


**It has long been recognized [Refs. 1,2,3,4] that user interfaces should be designed iteratively in almost all cases because it is virtually impossible to design a user interface that has no usability problems from the start. https://www.nngroup.com/articles/iterative-design/**


**“The first few iterations can probably be expected to result in major gains in usability as the true "usability catastrophes" are found and fixed. Later iterations have progressively smaller potential for improvements as the major usability problems are eliminated, and the design may eventually become so polished that very little potential for further improvement would remain.”https://www.nngroup.com/articles/iterative-design/**

**i think the very fact that something is complex means that you will not likely capture or encompass it all on the first try.**

11. are you really exploring information design?
12. why can’t all the same ux principles also apply to documentation systems? seems like so much is the same
13. what if you could more expertly test your own instructions? test on pc versus mac? permissions? browsers?
14. what if you could identify all your own assumptions present during testing?
15. could you construct a rating system from these criteria?
Easy to learn: The user can quickly go from not knowing the system to getting some work done with it.
Efficient to use: Once the user has learned the system, a high level of productivity is possible.
Easy to remember: The infrequent user is able to return to using the system after some period of not having used it, without having to learn everything all over.
Few errors: Users do not make many errors during the use of the system, or if they do make errors they can easily recover from them. Also, no catastrophic errors should occur.
Pleasant to use: Users are subjectively satisfied by using the system; they like it.



Time on Task
Subjective Satisfaction
Errors Made per User
Help Requests per User

16. isn’t agile the ultimate example of iterative design? you’re checkin witht users every 2 weeks to see if what your building aligns with what they want.

 From all the lessons learned in software engineering, two are picked here to serve as motivations for the design of development processes: First, making plans for all eventualities, and providing a conceptually clean solution was a frequent reason for software failure as unnecessary complexity was introduced. Gabriel (1991) described the successful strategy of UNIX and C as ‘‘worse-is-better’’—taking a more flexible approach proved often to be more successful than doing ‘‘the-right-thing’’. **Second, the experience of thousands of software projects tells that, for various reasons, a sizable part, if not a majority of the requirements arrive or change after development has begun (comp. e.g. Jones, 1995).**
**tom note: the most pivotal change in software development is with iterative design.**

**The resulting form of development are iterative approaches that do not try to sequentially follow process phases but instead interleave different activities and enable the development team to slowly grow the software from a functional and manageable core, integrating customer and client feedback (Floyd, 1987)**. As the need for interaction with stakeholders and iterative design surfaced, design activities were attributed to the developer’s role and replaced the rigor of engineering to some degree; software construction was understood as a creative activity. minimalism book

17. in your agile projects, why isn’t the user consulted more regularly?
18. doesn’t forum threads and support provide this iterative testing?
19. what about the movies like moments where the same scene is played a dozen times from diff people’s views? apply to iteration?
20. do we repeat the same mistakes over and over? like we cannot learn from the past? is there a sense that every day iterates on the mistakes of the previous day?
what is a complex prob vs a wicked prob?



i think we should leverage the Qualtrics tracking thing a lot more intensively, focused very specifically on each page in the docs. a custom survey about the content. this is how you can capture the iterative design.

**some of the products are so complex, it’s really unlikely that you’ll get; them 100% right the first time. through the iterative development, you have to use the feedback you get to make it better and better. every time someone reads and uses the doc, you should be able to capture that feedback in order to iterate on the document. the more people who use it, the stronger it can become. but you need a more immediate mechanism to capture feedback about this. i think the embedded and customized surveys are exactly what you need. but can you really manage this on a page by page level?**

**i think the whole premise of agile development is that you can’t know the end nor plan for it b/c the projects are so massive, so you have to just start working little by little through this. you do iterative development and then pop your head up to see if you’re on the right track. that is how software development has shifted, so why don’t we do the same with docs as well?**

**the agile approach is a response to projects constantly being over budget and slipping their dates. they basically don’t factor in all the complexity because it is nearly impossible to adequately anticipate all the complexity ahead of time.**

is this the docops strategy?

**“In a sense, many things on a software development project are theories, or more accurately, assertions that need to be evaluated.** The plan itself is composed of many assertions about how long things will take to accomplish. Even the requirements are assertions about the characteristics of a suitable solution. Just because some stakeholders or subject matter experts say a requirement is valid does not mean that they are correct. We need to evaluate even the requirements to determine whether they define the right solution to the problem at hand. This leads us to adopt a style of software development where the assertions inherent in the plan are repeatedly challenged and evaluated by the design and development of demonstrable versions of the system, each of which is objectively shown to reduce the project risk and build upon the other to form the finished solution.” https://www.ibm.com/developerworks/rational/library/mar05/bittner/index.html



**Sadly, development can be iterative without being incremental. For example, the activities can be applied over and over again in an iterative fashion without growing the understanding of the problem or the extent of the solution, in effect leaving the project where it was before the iteration started.” https://www.ibm.com/developerworks/rational/library/mar05/bittner/index.html**


———
maybe you could work on a paper that argues for more tech writers based on the VSK. tech writers provide a first layer of testing and feedback. with VSK, they went straight to the devs. they burned their trust and confidence due to the poor docs and process. talk about the need for self-serve models in order to scale. but emphasize that resources are not being allocated to enable this scalability. and as a result, we just keep spinning our wheels. talk about how the lean-in model fails.

“To many developers, iterative and incremental development is the progression through an almost infinite series of iterations, each of which causes the system to grow larger and larger until the customers are happy with it or decide to stop investing in its further development. From this perspective, as long as work is getting done and changes are being made, the project is making progress.”https://www.ibm.com/developerworks/rational/library/mar05/bittner/index.html how well does this describe docs?

thought: each week, look at the SAs list of issues and DART’s support tickets and analyze whether docs could have helped in that case.

**the need for iterative development is why i dislike PDF so much. PDF is the antithesis of iterative development, as it captures a static point in time and doesn’t include the possibility for constant development and updates.**

“Planning and estimating is basically a mechanism for first determining that the project is worth doing and later as an approach for keeping the project on track. Few of us would hire someone to repair their home without knowing how much it will cost and how long it will take at least with some degree of certainty. Software development projects are no different: the people funding the project need to know how much it will cost and when it will be done.” https://www.ibm.com/developerworks/rational/library/mar05/bittner/index.html


**What Is the Underlying Complexity in a Project?**
**In general, 'complexity' implies intricacy due to the availability of multiple divergent options, leading to a multidimensional scenario. However, business complexity inherently arises because of uncertain conditions, varied methods and technological advancements. Project level complexity has two dimensions: (1) project complexity and (2) requirements complexity. https://www.projectsmart.co.uk/can-agile-reduce-complexity.php**

you should fill out a form based on expectations for documentation. this form should ask users to consider these principles of complexity in order for content to thrive in the ecosystem. you don’t always have to enforce this yourself. instead, you should use this as a way to bring documentation up to the next quality level.

Principle 1: Let users switch between macro and micro views
Principle 2: Make information discoverable through metadata
Principle 3: Ensure information harmony in the larger landscape
Principle 4: Reduce and distill information to its essence
Principle 5: Conform to the patterns and expectations of the genre
Principle 6: Reconstruct the absent user ????
Principle 7: Reduce the complexity of technical language
Principle 8: Align the product story with the user story
Principle 9: Examples (Coming soon...)
Principle 10: Iterate and increment successively with each use
Principle 11: Demonstrate with visuals

title here: Iterate and increment successively with each use


**The Scrum Guide claims, Scrum is a framework for developing and sustaining complex products. https://www.projectsmart.co.uk/can-agile-reduce-complexity.php**

A joint study by McKinsey and Oxford Uni­versity found that large software projects on average run 66 percent over budget and 33 percent over schedule; as many as 17 percent of projects go so badly that they can threaten the very existence of the company. https://www.mckinsey.com/business-functions/digital-mckinsey/our-insights/achieving-success-in-large-complex-software-projects

**in what ways are software projects different from the iterative development of docs?**
how could you allow people to comment inline in the very line they’re reading to provide feedback about that particular component?

is this going to be a practical tip here? what are the takeaways?

how do you get over the idea that doc is done when in reality you can’t spend forever working on it?

**“Agile methodologies are targeted toward such kinds of problems that involve change and uncertainty, and are adaptive rather than predictive. “https://pdfs.semanticscholar.org/a0d7/2500614af085cbe2bf5f19b7f0538ecccf16.pdf**

**me: what if the product is iterating, and you’re constantly adjusting the doc for this product that keeps iterating? this is going to burn a lot of cycles. this is a really interesting article: http://agilemodeling.com/essays/documentContinuously.htm**

To remain efficient as possible you should consider writing the deliverable documentation for iteration N during iteration N+1. With medium length iterations (two to four weeks) you will need to experiment to identify which approach works better for you.http://agilemodeling.com/essays/documentContinuously.htm

**“Document Late” practice —> http://agilemodeling.com/essays/documentLate.htm check this out.**

By writing deliverable documentation continuously throughout the project, you address the following risks:
**why doesn’t doc follow the same process as software design in the iterative development?**
Delivery risk. By writing the documentation in sync with the rest of the solution, you know you have sufficient documentation to support what you've built to date. The implication is that your solution will in fact be potentially shippable at the end of each iteration.
Accuracy risk. Because the feedback cycle between doing the work and documenting what you did is short it is much more likely that you will remember the critical details which need to be captured.
However, there are three risks which are potentially increased by this practice:

Financial risk. Because the requirements are likely to evolve throughout the project, you will need to update the deliverable documentation to reflect those changes. You are in effect "travelling heavy" from an agile point of view by documenting continuously.
Schedule risk. It takes time and effort to write and maintain this documentation, and any rework of the documentation resulting from evolving requirements in effect impacts your schedule due to the required rework.
Accuracy risk. Sadly, it's easier to write about documenting continuously than it is to do it. It's common that agile teams will put off writing documentation until they have time to do so, in effect moving towards the document late practice instead of this one.http://agilemodeling.com/essays/documentContinuously.htm


By waiting to document information once it has stabilized you reduce both the cost and the risk associated with documentation. Cost is reduced because you won't waste time documenting information that changes, which in turn motivates you to update the documentation. Risk is reduced because there is significantly less chance that your existing documentation will be out of date. If you write documentation containing information which has not yet stabilized then you are at risk of having to rework the documentation once the information has changed. In other words, you do not want to invest much time documenting speculative ideas such as the requirements or design early in a project. Instead, wait until later in the lifecycle when the information has stabilized and when you know what information is actually useful to you. The implication is that your documentation effort may be a few iterations behind your software development effort.

An extreme version of this practice is to wait until you are finished and then write the documentation, the primary advantage being that you are writing about a known and stable thing (the release of the software that you just built). There are clearly several disadvantages to this approach:

You have likely forgotten some of the reasons behind the decisions that you made, clearly a problem if this is important to you.
You may not have the right people anymore to write the documentation because they've moved on to other projects.
You may not have funding to do the work.
The will to write the documentation may no longer exist.
http://www.agilemodeling.com/essays/agileDocumentationBestPractices.htm


this topic explains how doc fits into agile: http://www.agilemodeling.com/essays/agileDocumentationBestPractices.htm


4.1 Iterate, Iterate, Iterate
**Ideally you should create documentation throughout the entire software development lifecycle (SDLC) when it makes the most sense, albeit that's usually towards the end of the lifecycle. When you do write documentation, you should take an evolutionary (iterative and incremental) approach to its development so that you gain feedback as to its actual value. In other words, write a little bit, show it to someone, get feedback, act on that feedback, and then iterate. The best documents are written iterative, not all at once. An iterative approach enables you to home in on what the audience for your documentation actually needs. http://www.agilemodeling.com/essays/agileDocumentationBestPractices.htm**

Documentation is as much a part of the system as the source code. In addition to working software, you'll also likely need to minimally deliver user manuals, support documentation, operations documentation, and system overview documentation.http://www.agilemodeling.com/essays/agileDocumentationBestPractices.htm consider putting this as a quote in your email signature.


Why? It’s because it is almost always cheaper and easier to create a prototype to test than it is to develop a system or product and then amend that based on user feedback. There are a huge number of tools on the market that allow you to create interactive prototypes for web and software applications and most of these are low cost to adopt.https://www.interaction-design.org/literature/article/design-iteration-brings-powerful-results-so-do-it-again-designer

**when should you start iterating? iterate earlier on the doc process. first the product team, then field engineers, then the partners of field engineers, etc.**

Examples of Iterative Design
**Perhaps the best example of iterative design on the web is the use of Wikis. Wikipedia, for example, contains user generated content. Anyone is free to come along and improve on that content at any time. It’s easy for a reviewer (or editor) to visit that improvement and make a decision as to whether the change is an improvement or whether it takes something away instead. Over time, the theory is that Wikipedia’s content should evolve to make it the most valuable encyclopedia online.**

**It’s worth noting that this approach to iteration in design is a challenging one. With a huge community to draw on, one person’s “improvement” may well be another’s “detriment”. When using an iterative approach in your own design process, it’s likely that you will have more control over the decision making process than Wikipedia does. https://www.interaction-design.org/literature/article/design-iteration-brings-powerful-results-so-do-it-again-designer**

Iteration is by nature not innovative; rather, it is aimed at incremental improvement. https://medium.com/the-design-innovator/iteration-is-not-design-668695445f76

The use of iteration and user feedback is especially good at identifying usability problems. Jakob Nielsen wrote a classic article on this subject. But the kind of feedback obtained in this kind of iteration cycle mainly helps to discover problems with a current design. It does not tell you how to solve those problems. Users are very good at letting you know by their actual behavior if they do not know how to use a feature of your product. But they are notoriously bad at being able to tell you how to fix your product. That is why some good folks spend their careers learning interaction design in depth and becoming experts at solving usability problems and creating products that feel simple and intuitive.https://medium.com/the-design-innovator/iteration-is-not-design-668695445f76

**one problem is that with each iteration, you might get some feedback that prompts you to add some note, and soon your document loses its coherence and unity and flow. it becomes piecemeal.**

1. Fail often and fail fast: It’s kind of liberating. You actually have permission to mess up. In fact, it’s encouraged. The thought behind this is to not spend too much time developing things before getting it out to be tested. Get concepts (as rough as they may seem) into the hands of the user. Their course correction or validation is invaluable.https://www.bdcnetwork.com/blog/4-keys-mastering-design-thinking-and-iteration-process
