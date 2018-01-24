---
title: Guiding users through non-linear systems
permalink: guidance-through-non-linear-systems.html
published: false
---

In the previous tutorial, we looked at embedding maps to help guide users through larger processes. But all the maps I showed were linear maps. What about maps through non-linear, complex systems?

## Complex systems

A complex system isn't merely one that is technical or which contains many parts. It's a system that defies linear processes by including branching, conditions, feedback elements, many decision points, recursive processes, variables that affect the user's paths, and more.

In Content and Complexity, Michael Abers says that in complex systems,

> "Each new piece of data the user uncovers affects the path taken and the eventual outcome. ... it does not lend itself to being performed with a defined set of tasks nor can those tasks be performed in a fixed order. ... the step-by-step route to completing a task simply does not exist. ... instead of following a set path, the user continuously adjusts their mental path as new information presents itself. ... attempts to describe step-by-step actions break down b/c no single route to a solution exists."

In another article, Mirel gives a sample example of a sales analyst trying to decide how much to stock an item. The analyst might run various reports, weigh different factors against each other, analyze trends and other conditions to arrive at a conclusion. Each analytic activity can change the path the user takes. She says this constant feedback loop with each input aligns with research about how users approach complex tasks.

To illustrate, suppose you have back pain and are trying to find a solution for it. Your initial searches help refine your vocabulary and point you toward new directions and realizations. Each article you read can vary the next step you take. There isn't a linear process to follow to reach your goal. In these systems, presenting the user with a linear map that consists of definite tasks won't help much.

Albers suggests that for these scenarios, the information system needs to naturally adhere together around a specific context that the user presents. By decoupling the information into separate, semantically identified pieces, these pieces can be dynamically assembled to address the specific context the user presents. Again, this context constantly changes as the user makes his or her way through the system (with feedback changing the path, or other chosen variables influencing the results). The supporting information is one that constantly changes shape to match this fluctuating context.

Alberts says that a good way to understand this information model is with the analogy of scintering in ceramics. Scintering is the chemical process whereby individual components begin to naturally cohere into a connected structure.

[ youtube video ]

Albers says that XML gives promise as an approach to decoupling information and dynamically assembling it. (He wrote the article 15 years ago, so keep that context in mind.)

> "Only recently, with technologies such as XML and dynamic web page generation, has interaction design gained the underlying tools to actually support complex problem solving in the manner i call for here. With XML, the reports can be mrked-up and the various elements presented to the user grouped together in a manner which suports the information needs. Unfortunately, how to use those technologies to help us get from where we are to where we need to be has not been adequately addressed. [summary: he wants to generate information based on the user's context, dynamically pulling the information that the user needs in real-time to address that situation.]"

weinburger
doesn't work b/c google can't index decoupled bits of information. users find info via search. 


complex system that defies linearity. inputs revise the path. feedback loop causes you to change directions. "paths of action that are unpredictable paths that are never completely visible from any one vantage point, and nuance judgments and interpretations that involve multiple factors and that yeild many solutions, each with costs and benefits. (mirel, 1998)" ...

"Each new piece of data the user uncovers affects the path taken and the eventual outcome. The sales analysis qualifies as complex because it does not lend itself to being performed with a defined set of tasks nor can those tasks be performed in a fixed order."

"the step-by-step route to completing a task simply does not exist. ... instead of following a set path, the user continuously adjusts their mental path as new information presents itself."

" in a complex problem-solving environment, attempts to describe step-by-step actions break down b/c no single route to a solution exists."

understand entire customer journey.

"In complex problem solving, rather than simply completing a task, the user needs to be aware of the entire situational context in order to make good decisions... early analysis must uncover the user goals and information needs in order to allow the user to build the required picture of the entire sutiation."

"Only recently, with technologies such as XML and dynamic web page generation, has interaction design gained the underlying tools to actually support complex problem solving in the manner i call for here. With XML, the reports can be mrked-up and the various elements presented to the user grouped together in a manner which suports the information needs. Unfortunately, how to use those technologies to help us get from where we are to where we need to be has not been adequately addressed. [summary: he wants to generate information based on the user's context, dynamically pulling the information that the user needs in real-time to address that situation.]"

"all the information possibly relevant to support addressing the user's goals and information needs simply cannot be dumped onto the screen. nor can a hierarchy of links solve the design problem of effective information presentation."

"Instead of a linear step-by-step procedural process, providing informatino for complex problem solving could be better viewed as a process comparable to sintering ceramics....In complex prolbem solving, the individual pieces of data need to be compressed and manipulated to form a coherent picture of the real-world process they describe." https://www.youtube.com/watch?v=NzCeMxq0bPs
https://www.youtube.com/watch?v=48Is5ENhkGE

same ideas as david weinberger. you have little pieces of information. when a user enters a context, the relevant information can form around the user.

information should be dynamically brought together to a layer of presentation based on the user's need, not based on a fixed design.

"The information design must ensure that infomration salience is proporational to its importance. all data is not creted equal. Some data is more relevant to the situation than other data. The design must not allow easy to present bu tunimportant data to dominate."

"...the requirements analysis cannot focu on defining a single path; nor can it define exactly which information is desired. instead, the analysis must uncover potential information requirements and presentation methods."

"As people address a complex problem, a structure emerges which is based on the context, the interrelationships between important elements, and the user's schema. Highly effective support for complex problem solving thus must match the emergent structure, a structure that undergoes multiple shifts in its point of view as the problem solving progresses."

"Only recently, with technologies such as XML, has information design gained the underlying tools to actually support complex problem solving in a general manner. with these new technologies, we finally have the means to break up the old contextual elements, recombine them at will, and present information uniquely focused on a problem. However, although the need to support complex problem solving is undisputable, we lack a clear methodology to support capturing the information requirementes, reordering and dynamically constructing information to fit a situational context, and designing the iterface for such a system."
