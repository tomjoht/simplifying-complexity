---
title: Context-sensitive help
permalink: context-sensitive-help.html
published: false
---

Context-sensitive help is help that treats context as a variable to determine the help information shown. Creating this type of help can be challenging due to the changing contexts, which can alter meaning or require adjustment in the content.

* TOC
{:toc}

## Introduction

Most of the documentation I create is for developers, so there usually isn't a user interface (UI) that I'm describing. However, I've been focusing more on documentation for an app submission console, which has a UI. Because users are unlikely to consult the documentation before jumping right in and submitting their app, we want to incorporate more help directly in the user interface. As such, I've wondered what the best approach is for creating and delivering context-sensitive help.

I tried to find more conceptual, strategic info on creating context-sensitive help. Academically, there hasn't been much research into this area (that I've found). One study looked at click rates on help links in a grammar application (see Heift). The main finding was users click the contextual links about 10% of the time, more commonly with difficult questions.

Other articles talk more from a practitioner's perspective. Paul Mueller's article on "Developing an Embedded Help Solution" explains the reasons and approaches they took to implement embedded help. The article even contains JavaScript code required to render the content on the page. Paul uses the term "embedded help" more than "context-sensitive help," but I like the latter term because it is richer in scope (a concept I'll explore later).

I suspect most academics feel context-sensitive help is merely a technical implementation of documentation in a more user-centered way, and hence not inviting of deeper exploration.

Most popular articles about context-sensitive help are mostly technical how-to's; any conceptual information covers generally obvious, common-sense points.

In this article, I'd like to peel back the topic of context-sensitive help and explore the topic a bit more. I'll propose both conceptual and technical strategies for implementing it as.

## Context-sensitive help varies based on context

We often use the term "context-sensitive help" without pausing to understand exactly what this means. Context-sensitive help provides information that varies based on a particular context. Think of the context as a variable. As the context varies, so does the help.

Typically, if a user clicks help from the context of Screen 1, certain information appears. But if a user clicks help from the context of Screen 2, other information appears. We use the context of a screen's location to identify what help should be surfaced. Context is a variable that influences the help's information shown to the user.

Given this definition, context-sensitive help doesn't need to be embedded in a user interface to be context-sensitive. It just needs to change the information shown based on the context. The following contexts can all vary the type of information surfaced:

* [User's location](#user_location)
* [Data the user has input](#user_input)
* [The user's browser properties](#user_browser)
* [The user's profile](#user_profile)
* [External factors](#external_factors)
* [Keywords supplied by the user](#user_keywords)

The following sections expand on each of these context variables.

### User's location {#user_location}

As explained earlier, the user's location in the system can information what topics are shown. This is the most common approach, since you can zero in on content or topics all related to that location. This approach fails, however, if the user is simply lost in a system and can't identify the right location. For example, if you're trying to find how to set-up second factor authentication on a system but can't locate the right menu/screen where you make this configuration, location-based context won't be helpful.

### Data the user has input {#user_input}

If the user enters incorrect data, context-sensitive help can appear as an error message window. Other warning or path-correction messages might be displayed based on information the user inputs &mdash; such as missing fields or incompatible selections.

This scenario highlights the most common trigger for help: errors. Usually, users don't need help when they aren't committing errors in the application. It's when they get an error message (especially a confusing one, or one that asks them to do something vague) that they turn to help.

### The user's browser properties {#user_browser}

Ad tech is all too familiar with determining context from the user's browser. A typical example is when you search for a particular product (e.g., camping gear) on one site, and then suddenly you see ads for camping gear on other sites you've never visited. The ad is displayed dynamically based on the context it receives from the user. Technology that identifies specific properties about your browser (the browser type, location, IP address, and other settings) contributes to a unique, PII-safe profile that is shared in advertising databases. This unique profile knows what pages you've visited and can serve up similar ads to this profile.

You don't need ad tech logic to inform the context for your help. You can infer properties from the user's browser about the locale, the browser type, the device type, and more. Common examples are showing Mac-specific information when detecting the user has a Mac browser, or defaulting to Japanese when detecting the user's language is Japanese.

### The user's profile {#user_profile}

Assuming the user has a profile and is logged in, this profile can provide context to inform the help. For example, if a user has API keys associated with their profile, you can populate code samples with the API keys. If you have various languages shown in the UI, the user's preferred language specified in their profile can set the preferred languages to be shown by default.

Sometimes this technique is known as "dynamic personalization." The context of the user's profile informs the content shown to the user.

### External factors {#external_factors}

There might be external factors that determine the context as well. For example, if a system is down in an area that affects a group of users, that external factor could trigger special information shown to that user group. Or if a user qualifies for something (based on their location, profile, user input, or some other context), the information shown to the user could also be customized. In all cases, some external context is adjusting the information shown to the user.

### Keywords supplied by the user {#user_keywords}

We can also determine the context from users directly &mdash; most commonly through keywords supplied by users themselves. Users tell a search box what they're interested in seeing, and the system uses these keywords to provide corresponding information.

Including search as a form of context-sensitive help is a bit of a stretch, because usually we expect the help to automatically detect the context without the user needing to specify it through keywords. But because AI techniques are trending, I'm including keyword-supplied contexts as yet another type of context that can inform/change/adjust help.

Most relevant today, chatbots might be leveraged in scenarios that fit into this definition. Users tell the chatbot what they want (speaking keywords, or they type them in UI chatbots, or they select tags), and the chatbot uses those keywords (along with natural language processing) to return the right information from potentially thousands of other topics in the system.

### Definition summary

When we say "context-sensitive help," it is broader than just tooltips in a user interface. It is a system that displays information based on a particular context &mdash; a context that can vary, and as it varies, so too does the information shown. In that sense, it is an information system that is smart. The implementations could provide simple location-based links to surface help related to that location, but it could also be a system that takes input from user data, from browser data, external factors, search keywords, or natural language and use that context to surface the right information the user needs.

I've never worked on a project where we incorporated more advanced contextual logic to inform the help. We mostly use manual links based on UI locations. However, at some point we could take the approach to another level if desired. Because larger systems make it more difficult for users to find the right information, we should always be thinking about context that we can gather to surface the right information that the user needs.

## Context determines meaning

Because context contributes to meaning, context-sensitive help presents unique challenges with documentation. Strip a word of its context and it loses some meaning. For example, take the word "strip" and remove its context. Its meaning suddenly becomes vague and multi-directional. The same principle applies at the sentence level: a standalone sentence is less clear without surrounding sentences, a paragraph is less clear without surrounding paragraphs and headings, a chapter is less clear without a table of contents and book title, etc. The less context, the less clear the meaning.

For fun, pick out any word from a sentence and stare at it alone, without any context, for about 2 minutes. Pretty soon the word will start to look foreign and strange.

Context-sensitive help not only removes the context of the other documentation, it often *adds* a new context to the documentation. And since context informs meaning, changing the context potentially changes the meaning.

For example, "Keep me notified of updates" changes meaning if displayed next to your phone number or next to your email address in a UI. If you write this phrase at the bottom of a letter to your uncle dying of cancer, it would mean something entirely different. It also depends on who says it. A parole officer? A doctor? A police officer on a stakeout with his or her partner, and so on. Context helps establish the meaning of our words.

## Risks of new contexts

Although context can change meaning, radical misinterpretations are less common with documentation. More common would be missing context from an orphaned antecedent. For example, suppose this sentence appears in the UI:

> As mentioned earlier, the preview refreshes only on app start.

What was mentioned earlier? Similar scenarios with missing antecedents are common with "this" or "it."

Despite the dangers of introducing a new context for your content, one benefit to context-sensitive help is that users usually have the user interface as the present context. That UI context can assist the help content with clearer meaning, especially because help content often describes UI components. Now help doesn't need to describe or show a screenshot of the UI component in the help. The needed context to make the meaning clear is *right there*. This is why screenshots are often purposely removed from context-sensitive help.

But for help that doesn't describe a specific component, context-sensitive help is at a disadvantage. For example, using context-sensitive help to describe a process spanning multiple screens and components might not be that useful. In those scenarios, standalone documentation is probably more advantageous, because you aren't trapped by a specific user interface context or location for the information.

## Single sourcing context-sensitive help and standalone documentation

Creating context-sensitive help introduces challenges with single sourcing. Presumably, you want to use the same content in both your docs and the context-sensitive help. Why define a field twice? Most of the information is similar, so with a bit of cleverness and conditionalizing, you should be able to make the same information work in multiple places. This is, after all, the goal of single sourcing. It prevents inconsistency, duplication of effort, saves time, and more. Right?

However, the varying context makes it more difficult to use the same content across contexts. What makes sense in the standalone documentation might not make sense in the context of the user interface. Even for the easiest of scenarios -- field definitions -- the same help content can't merely be used wholesale in both places. A line in the doc might start by describing the UI component, explain how to access it, show a screenshot of the component, and define each option the component contains.

Yet using the same documentation snippet within the UI's context-sensitive help would be unnecessary, since the user is already looking at the UI component and its options. All that's needed is a short description of each option. The descriptions can likely be made without naming the title of the option described, since a tooltip triggered from an icon next to the field would make a field title unnecessary.

If a component merits more description and commentary than is appropriate in the UI, the context-sensitive help snippet needs to link to the full details in the documentation. But you wouldn't want this same link for more information to appear in the standalone documentation, because the link would point to itself.

Can you see how single-sourcing content between contexts becomes challenging? You have to create content that has a consistent meaning in multiple contexts. You have to write sentences or phrases that could work equally well in both the UI and the documentation. As a result, you might have to granularize the information into small chunks and snippets. At that point, authoring also becomes more onerous because your content likely consists of individually stored references that are hard to read as a whole and potentially manage.

If you abandon the goals of single-sourcing the content, you face other challenges. Now you have two doc sets to update. If you make an update to the field definition in one place, you have to update it in another. Maintaining multiple sets of mostly the same information can be maddening and require a lot of effort just to keep the two data sets in sync. Usually the two drift apart.

{% comment %}

## Strategies

I've been talking at an abstract level for a while. Let's dive into some real strategies for approaching context-sensitive help....

### Provide a list of links

Location doesn't always provide the right context to perfectly determine the information the user needs. Remember situations where users are simply lost, or where the information they need is part of a larger task workflow involving multiple locations in the UI. As such, when a user clicks a help link on a page, provide a list of possible topics related to that location.

To do this, you might tag your help topics with keywords corresponding to UI screens. All topics related to Screen X might have Tag X. In your context-sensitive help, you can provide a list of related links built from these this tag.

### Identify what's not shown

Users are most likely to need help when they commit an error in the UI. If a user inputs the wrong information, what error messages or warnings appear? If those dialogs, insert information to help the user correct course and fix the issue.

It can be difficult to see the entire user interface when many error windows, modals, on-screen warnings, and other interactions are hidden until the user triggers that context. When technical writers are assigned to create context-sensitive help, they're usually given a designer's mock-ups that shows a static screen. You'll have to look for what's not shown by triggering as many possible error conditions as you can. You could ask the front-end developer what happens under various scenarios where you input invalid information or make other errors in the UI. Then you could ask to customize the text shown to the user, as well as include links for more detail.


- you may not know the right information. it's somewhat hubristic to think we know it, so why not show the user a list of links to various topics in the help instead?


but you have the benefit of the UI context.

now you must single source it, hard to do both.

Aty

{% endcomment %}


## References

"Developing an Embedded Help Solution"
Author(s): PAUL MUELLER
Source: Technical Communication, Vol. 50, No. 1 (FEBRUARY 2003), pp. 24-32
Published by: Society for Technical Communication
Stable URL: http://www.jstor.org/stable/43090529

"Clicking for Help"
Author(s): Trude Heift
Source: CALICO Journal, Vol. 30, Learner-Computer Interaction in Language Education: AFestschrift in Honor of Robert Fischer (2013), pp. 187-202
Published by: Equinox Publishing Ltd.
Stable URL: http://www.jstor.org/stable/calicojournal.30.187

{% comment %}

## basic idea
- fitt's law: law that says the more distance a help topic is to the user's point of need, the less likely he or she is to find it. this is something like pitt's law
- user-centered. fundamental paradigm difference in help. not, you come to us, but we come to you. human-centered design. bringing help within the context of where the user needs it. reducing the difficulty of finding it.
- based on idea that users don't like to leave their current task. you bring help to them. people don't like to "read documentation." help users stay within th e context of their current task. michael hughes
- in broader sense, it is much more efficient to deliver help to a user if you can determine the context that defines exactly the information they need, rather than forcing the user to sort through all the stuff to figure out what they need.
- in reality, our help should be more like this. it should be smarter, it should use context.
- work closely with UI designer and engineers rather than separate.

## is csh better?
- does csh or embedded help meet the goals of the user? maybe. it could be said that we do users a disservice by (a) not prompting them to foray into the help. one learns a great many things by interacting in a learning systemnm. we want to give users the full experience. and (b) by putting band-aids on the application UI, we enable poor design. might be better to force devs to fix the underlying issue.we're making it harder for them to make sense of the info b/c we're giving them the tree instead of the forest, showing them little definitions or tooltips here and there.
- might also be bad b/c we're giving users little tooltips and helps here and there but not guiding them along a more sequential journey.

## producing it is a different experience

## what have others written about csh?
- clicking for help
- paul mueller article
- pronovix article

## strategies with csh
- what are you not seeing in the UI? modals that appear, dialog boxes, alerts, error messages, and other signposting to users.
- need analytics on links clicked in order to see what the result is. this needs to be communicated to dev as well. funnel back this info into design team.
- identify errors and difficult aspects of UI for the help links. users more likely to click or need help in those areas. this is just common sense: where do you have questions or run into needs for more information in a UI? well, that's where the help should be provided. it's like the safeguard for usability.
- csh is more than just tooltips. also alerts, error messages, on-screen text, labels, in-line definitions. placeholder text in forms (hints)
- different levels of help -- page level, section level, field-level.
this could be a more direct way of zeroing in on the reasons why people log support cases. need to go about this more strategically. catalog the reasons why people log support cases, and then connect those cases to the UI where they have the jumping off points, and then put links there.
like on Review Status. if app fails, link to "reasons for app failure."
- the optimal time to position the help is when a user runs into an error. people click the help link only about 10% of the time. users find it more relevant to try the UI first and only consult help if they find that they did something wrong or if they truly need it. thus, the first step in construcitng csh is to identify where users might encounter errors. identify the error messages in the UI and position links there. "Clicking for Help" article. <img src="media/rasters/for example, when users upload an image, if they get an error that says the image exceeded the upload limit, that's where you should position the csh link.  this is why it's critical when creating csh to identify all the error messages and all the difficult parts of the UI first.

## challenges with csh
- problem: UI help is a microdetail of a specific feature, whereas doc is a larger, tutorial or sequential nature. flow is different.
- put help bubbles on all fields for consistency, or only on confusing ones?
- how much text should go into the UI
- length limits requires you to treat tooltips like tweets or poetry, compressing massive amounts of communication into little snippets. puts a lot of pressure to use most communication skills.
- how do you ensure content flow across mediums?
- if the tooltip should have a link for more information, this has to be handled. add moreinfo property in the yaml file and combine it in the json output that devs implement
- tooltips or embedded text in the UI? embedded text is more clickable and relevant but occupies more space.

## examples of csh
- is there an example of csh done really well? google? play console.
- look at at least 3

## how to create csh
- how to deliver the help. json file. manage independently from application.
- csh should be single sourced in both UI and docs. otherwise out of sync, manual duplication, errors, multiple effort.
- basic approach to UI doc where you have a lot of fields, list in table rather than in each step.
- tooltip length should be short - 1-3 sentences. can't scroll in a tooltip. principle of progressive disclosure. link for more info. however, poses difficulty b/c a link for more information shouldn't appear in doc pointing to same page.
- think about csh as your first level of help. answer most immediate questions.
- recommended structure in the json file: tab, term, def, moreinfo. don't use array b/c it's hard to incorporate into your system. woudl have to use looping logic.
- table of info is brief only. more info sections appear below the table.
- provide demo to engineers so they can implement the CSH. demo should provide some working tooltips but let front-end engineer decide how they incoporrate.
- tooltips should be short: typically no longer than a tweet. otherwise tooltips are problematic (text exceeds the frame, might require scrolling, etc.) use progressive disclosure. if user needs more info, provide learn more link.
- on tabs where users just have a bunch of fields to select, don't list out steps that basically say, 1. in the X field, type this. 2. in the Y field, type that. reason being, these steps are unnecessary. user knows he or she has to fill out all the fields, and sequence usually doesn't matter. the numbered list like this doesn't faciliate much scanning. user should be able to quickly find help where he or she needs it.
- give devs a map of how they should implement the tooltips
- field definition table defines all the fields on the tab. - if a field definition merits extended explanation, provide that in a section below the table.
- place where json is stored needs to be CORS enabled
- tooltips and field defs in help should single source the content. as such, tooltip content should be stored in a reusable snippet like format.
"More info" in the UI, "Learn more" to point to the doc.

--------


Questions

What question are you asking?
How did the question become relevant to you?
What have others written about this topic?
What is solution (n)? What's wrong with the solution (n)?
What's your proposed answer?

Central question: How should one go about creating context-sensitive help?



----------
cs2

- what is the definition of X? help that is organized by context within the user's environment. help in the context of the user. call it user-context help?
- what is X for? enables easier, quicker access to the help.
- what assumptions do you have about X? better, makes help more clickable.
- what is X's story? help neglected is suddenly become visible and useful b/c it's in the context of the user. but prob. overselling that.
- what does X assert? help is more used if in the user's context. what if it's used less? asserts that this is a more user-centered approach to doc, and this move is good. we want to do things that make things more user-centered. does merely positioning and organizing the content in the user's context and environment what makes it user-centered? centered content around user? could we still have content in CSH that is not user-friendly?
- how does X's assertions contradict themselves? makes it easier for users, but then they don't foray into help, don't get lost. they try to navigate the app using little fragments of info. there might be benefit to immersing a user in the big help. like having groceries delivered versus going out to get them yourself. like bringing the library to the user, but only small snippets. isn't there benefit to having the user go to the library? in a way, we are shortchanging the user on the information delivered. we think we're helping the user, but now we're making it harder for them to make sense of the info b/c we're giving them the tree instead of the forest, showing them little definitions or tooltips here and there. more useful would be for user to immerse themselves in more context and tutorials.
- how does X become dangerous? too much info makes the UI complex, burdensome.
- what are some good and bad examples of X? google play console.
- how do you know whether X is good? whether it reduces support in ways that regular doc does not.
- what principles are assocated with X? progressive disclosure, immersion.
---------
cs3
- what is the ultimate question we arrive at if we trace up questions higher and higher with purpose?

---
more thoughts:

- what you say changes its meaning if the context changes. example: some photos side by side in newspapers have disastrous consequence3s.

Ideally, I would have thought more would be written on the topic, though perhaps I've zeroed in on too specific of a topic?

Online there isn't much either:

https://pronovix.com/blog/overview-context-sensitive-and-embedded-help-formats
https://cherryleaf.teachable.com/p/writing-and-desiging-embedded-help
https://www.linkedin.com/pulse/what-context-sensitive-help-steven-greffenius/
https://help.wixanswers.com/en/article/creating-context-sensitive-help
http://www.doccontents.com/fr/2016/05/31/what-is-contextual-information-for-modern-software/
https://docs.servicenow.com/bundle/jakarta-servicenow-platform/page/administer/navigation-and-ui/concept/c_ContextSensitiveHelp.html

articles on context:
https://www.garyvaynerchuk.com/content-is-king-but-context-is-god/
https://moz.com/blog/context-is-king
















considerations:

- tooltips need to work in the UI and in the docs. links to more info have to make sense.
- minimize number of URL changes, since we have some UI links already pointing to sites.
- Go through an identify all the existing tooltip links. Make sure they still point to valid pages or are redirected:

https://developer.amazon.com/public/solutions/platforms/webapps/docs/appurl.html



- glossary tooltips are like context-sensitive help within the docs themselves. that's why they follow a similar model.


thought: could you do more cs within the content you're currently working on in your job?

csh is more than just tooltips. also alerts, error messages, on-screen text, labels, in-line definitions. placeholder text in forms (hints)

csh follows the principle of progressive disclosure. you graduate levels of information. thus you have to structure and layer your information this way.

https://w.amazon.com/index.php/AWS/Teams/Design/UXDesign/AWS_HIG_Development/AWS_User_Assistance_Ecosystem#Writing_guidelines_for_help_panel_content_.28DRAFT.29

https://alpha-docs-aws.amazon.com/awsstyleguide/latest/styleguide/consoles-and-ui.html

piggyback on this larger principle of progressive disclosure as the link into more philosophical contexts.

https://w.amazon.com/index.php/AWS/Teams/Design/UXDesign/AWS_HIG_Development/Help_Panel

based on idea that users don't like to leave their current task. you bring help to them.

includes error messages, alerts, and other text.

information must flow seamlessly from one to another. the tooltip flows into more help. content flow.

identify pain points in the app and apply CSH as a kind of oitment or aid to reduce the pain.

forces you to interact with front-end devs.

in your demo, do you have a page-level help button as well as tooltips?

what terms are new, vocab that specific to the context?

mapping the applicatoin so you know where all your help appears. do you create a sample app?

is there a procedure for doing csh?
- identify the pain points
- tooltips?
- provide the blueprints for the front-end devs?

how much info should you bring into the UI? why not bring it in via a modal?

content is not sequential, not a tutorial. it is accessed during a specific point in the UI at any time.

"More info" in the UI, "Learn more" to point to the doc.

does this feed into user-centered design? you are designing help around the user, not requiring the user to come to the help.

best way to incorporate csh
cs1
- is progressive disclosure the principle to follow? surely.
- what does pd even mean?  information in layers.
- examples of pd in regular life? chapter summary followed by full details. beginning math and then algebra and then calc.
- how do you ensure content flow across mediums?
- how would you need to change the way you write? come to the user. figure out how to connect it to the rest of the content.
- how much can you extract from the docs and bring into help? i like the 3 tier model.
- is there a conflict between csh and doc content b/c csh is not a tutorial or sequence, and doc contnet might be understood within a larger context or sequence/tutorial? what if the doc content references other parts of the page or refers to other parts of the page? yes. this might make it really hard to single source.
- is there an example of csh done really well? google? play console.
- deciding whether to write content directly in the UI or to put it into a collapsable section or tooltip? how to decide? prob. a bit of both.
- what exactly is th emodel of pd? do you just unravel more and more details, more complexity? do you write in an inverse triangle? the inverse triangle.
- how does PD interact with jargon? can you somehow ramp people up so they aren't thrown headlong into something complex? qusi similar.

--> - is there a conflict between csh and doc content b/c csh is not a tutorial or sequence, and doc contnet might be understood within a larger context or sequence/tutorial? what if the doc content references other parts of the page or refers to other parts of the page? yes. this might make it really hard to single source.

next level: help that appears based what you're doing in the app. logic that looks to see what is o=incomplete or what is incorrectly coded.

screen overlays and walkthroughs are also really common

another level is to change the text tat appears in the interface like the button names and tab names and such so that they're clear from the getgo

implement a related topics feature?

what if a modal appears and launches a wizard? a chatbot? what would you like hepl with here? which field? question?

links within tooltips. where do they go?

identify prob areas and other areas in app and put links there

how do you track the number of times that someone clicks a link in your application? this is essential. need to have some query strings in the tooltips.

this could be a more direct way of zeroing in on the reasons why people log support cases. need to go about this more strategically. catalog the reasons why people log support cases, and then connect those cases to the UI where they have the jumping off points, and then put links there.

like on Review Status. if app fails, link to "reasons for app failure."

use metrics on clicks in csh to identufy prob areas in ui to improve.

identify prob areas and other areas in app and put links there

how do you track the number of times that someone clicks a link in your application? this is essential. need to have some query strings in the tooltips.

this could be a more direct way of zeroing in on the reasons why people log support cases. need to go about this more strategically. catalog the reasons why people log support cases, and then connect those cases to the UI where they have the jumping off points, and then put links there.

like on Review Status. if app fails, link to "reasons for app failure."

the optimal time to position the help is when a user runs into an error. people click the help link only about 10% of the time. users find it more relevant to try the UI first and only consult help if they find that they did something wrong or if they truly need it. thus, the first step in construcitng csh is to identify where users might encounter errors. identify the error messages in the UI and position links there. "Clicking for Help" article. <img src="media/rasters/

for example, when users upload an image, if they get an error that says the image exceeded the upload limit, that's where you should position the csh link.  this is why it's critical when creating csh to identify all the error messages and all the difficult parts of the UI first.

{% endcomment %}
