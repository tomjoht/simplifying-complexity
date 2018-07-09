---
title: Reducing the complexity of technical language
permalink: reducing-the-complexity-of-technical-language.html
---

{: .principle}
Highly technical material often becomes incomprehensible due to the unfamiliar terminology that's simply part of the technical domain. Readers who don't already speak the technical language in fluent ways will struggle to make sense of the material. To make these highly technical texts more accessible to users of all levels, you can create glossaries, embed definitions in tooltips, provide links for background knowledge, and more. As you define your terms, it's helpful to read beyond your company's content and check out how the same terms are used in your competitor's documentation and industry articles. The focus on precision with terminology helps keep you aware of usage discrepancies in your docs.

## Unfamiliar terms &mdash; one reason for incomprehensibility

One reason technical documentation is so difficult to follow is because of the unfamiliar terms and jargon in the content. A while ago I was evaluating whether to use Acrolinx, a language linter for tech docs, and I learned that the bulk of configuration for Acrolinx is in building out your own custom dictionary. Apparently, identifying your custom terms and incorporating them into Acrolinx's checking logic can take a number of weeks or months. The custom terms can account for around half of the terms in your dictionary.

Unlike most other professional writing disciplines, tech docs are notorious for the amount of specialized terms in their content. Not only do we have unique terms related to our products, industry jargon and company-specific terms make their way into docs, driving up their complexity.

API evangelist Kim Lane recently noted his frustration with an API's language when he encountered an undefined acronym &mdash; "DEG". Lane explains,

> I came across a set of API resources for managing a DEG the other day. You could add, updated, delete and get DEGs. You can also pull analytics, history, and other elements of a DEG. I spent about 10-15 minutes looking around their developer portal, documentation, and even Googling, but never could figure out what a DEG was. Nowhere in their documentation did they ever tell consumers what a DEG was, you just had to be in the know I guess. The API designer (if that occurred) and developer had never stopped to consider that maybe someone would stumble across their very public API and not know what a DEG was. ([Using Plain Language In Your API Paths](https://apievangelist.com/2018/07/09/use-plain-language-in-api-paths/))

In this case, DEG must have been an acronym specific to the developer's API. In these cases, there's really no excuse for not defining your own pet acronyms and unique vocabulary. You can't simply make up an acronym and not define it for users (without frustrating them).

But many times, acronyms and unfamiliar terms are part of a specialized domain. As a technical writer, using the correct terms for your knowledge domain and your product is necessary, and those terms are often appropriate for that particular knowledge domain.

To simplify the language, you can't just omit the necessary terminology for the domain or substitute in more friendly names. You have to teach the user the right language so they can participate in the conversation.

One commonsense approach for teaching users how to speak this language involves defining unfamiliar words for the user. You can define unfamiliar words in at least three ways: (1) include a glossary, (2) include inline tooltips with definitions, and (3) include "Background Knowledge" sections to help new users ramp up on the knowledge domain.

Since technical writers tend to be language connoisseurs, priding themselves on the ability to squeeze clarity out of engineering babble, focusing on language as a means of helping users understand content constitutes a major advantage tech writers can leverage to simplify complexity.

## Previous writing about glossaries

Entire books have been written on plain language principles and writing for clarity. For example, the principles of plain language are explained well in the [Federal Plain Language Guidelines](https://www.plainlanguage.gov/guidelines/). Ginny Redish's [Letting Go of the Words](http://idratherbewriting.com/2011/04/08/book-review-letting-go-of-the-words-by-ginny-redish/) also provides excellent guidance for clear language.

In ["Defining Glossaries"](http://www.ingentaconnect.com/search/article?option1=tka&value1=defining+glossaries&pageSize=10&index=1), Michelle Tackebary describes the history of glossaries and approaches for defining terms, such as distinguishing between *contextual definitions* and *stipulative* definitions. Tackebary provides a history and set of best practices rather than a methodological study.

In ["The ABCs of Writing a Technical Glossary"](http://www.ingentaconnect.com/contentone/stc/tc/1998/00000045/00000001/art00003), Evie Gray and her co-authors outline a number of principles and best practices for creating glossaries. For example, they cover commonsense principles such as to avoid defining terms with the term you're defining, but they also expand on the right tense, format, and scope to be used in glossaries.

Style guides also provide some guidance on glossaries. The [Apple Style Guide](http://cdn2.hubspot.net/hubfs/1772454/Blog_Images/01.26.16.Apple_Style_Guide.pdf) contains a useful section on "How to write a glossary." And [Read Me First!](https://www.safaribooksonline.com/library/view/read-me-first/0131428993/ch13.html) also has a "Glossary Guidelines" section. These style guides contain practical (though brief) advice on creating a glossary and tend to focus on consistent styles within definitions, cross references, and other aspects.

To limit the discussion to a reasonable scope, I'm focusing here on the terminology aspect of language, specifically how to handle the proliferation of specialized terms in glossaries. In complex technical material, the complexity is often due to the new language that users must operate within to understand the meaning. These scenarios are most common with developer documentation but would also include science or medical texts as well.

## Identifying unfamiliar terms for the audience

To ground the discussion in a concrete way, let's start with a passage to dissect. The following paragraph is from  tech docs I work on:

> This Fire TV Catalog plugin is based on Apache Cordova. [Apache Cordova](https://cordova.apache.org/) provides a wrapper that allows you to include native Android functionality in HTML5 web apps. Using Cordova, you can create an APK file for your web app.

Some terms that might be unfamiliar to users include the following:

* Fire TV Catalog
* Apache Cordova
* wrapper
* native Android
* HTML5 web app
* APK

In just two sentences, there are half a dozen specialized terms. Is it any wonder why tech docs can be so dense and inaccessible? How can we simplify the content so that users can understand what we're saying?

First, we have to identify terms that might be unfamiliar. A term on its own isn't familiar or unfamiliar &mdash; it can only be familiar/unfamiliar in the context of an audience. So the question is, *for our intended audience*, which terms will be unfamiliar?

Except for the first term ("Fire TV Catalog"), all the other terms are fairly standard terms in this knowledge domain (web app development). If you develop web apps, you should pretty much know what these terms mean. Otherwise, you have some initial learning to do, and you probably wouldn't even be reading this documentation.

For example, if you don't know what an APK is as it relates to app development, or what native apps or web apps are, then we need to roll back the tutorial here and start with more foundational concepts.

As a tech writer, how do you recognize which terms will be familiar with your audience? Without more understanding of your audience, identifying familiar versus unfamiliar terms is nearly impossible. (This is why my previous topic focused on the importance of [reconstructing the absent reader](reconstructing-the-absent-user.html).) In this example, the audience is a developer creating a web app, so the audience *should* be familiar with standard terms and concepts in the web app development space.

But how do you, as a technical writer who is presumably *not a web app developer*, know which terms are standard industry terms for web app developers? This is one of the main challenges in developer documentation. Basically, there's no shortcut here &mdash; as a tech writer, you have to ramp up on the knowledge domains you're writing in (at least a bit, even if the ramp up just involves a cursory read-through of material). Otherwise, you won't be able to distinguish between industry-standard terms and company-specific terms.

When you do ramp up on the knowledge domain, you'll start to recognize which terms are familiar and which might be new. It's not necessary to define familiar terms for your audience, because presumably this would just be extra noise, adding more information than the audience needs.

However, suppose your audience doesn't involve seasoned developers all familiar and conversant with these terms. More realistically, your audience's knowledge likely falls along a spectrum, with some newbie web app developers struggling to understand the space, and some seasoned web app developers not needing much help at all (guess which audience is more apt to be reading the documentation).

In this scenario, where the audience has a range of technical abilities, many industry-standard terms will be unfamiliar to some of the audience. Should you, as a technical writer, define them for the less experienced users? Or is the burden on the user to ramp up on the industry before reading your docs?

## "Background Knowledge" sections help new users ramp up

Here's one approach to helping new users ramp up on the knowledge domain. Rather than trying to educate newbie developers on the knowledge domains &mdash; a task usually beyond the bandwidth or expectations of any technical writer &mdash; you can provide a list of links the user can read to ramp up their knowledge. I call this section "Background Knowledge."

For example, in a topic I was writing about [device filtering and compatibility](https://developer.amazon.com/docs/app-submission/device-filtering-and-compatibility.html#background-knowledge), I included a section called "Background Knowledge." In that section, I provided a number of links to foundational material that would ramp users up to the right level.

{% include course_image.html size="large" filename="background-knowledge-terms" ext_print="png" ext_web="png" alt="Helping users ramp up on background knowledge" caption="Helping users ramp up on background knowledge" %}

Users who already understand these foundational concepts and industry-standard terms can skip the background knowledge sections, but users who would otherwise be confused would have a lifeline to follow to stay afloat. Remember that your audience doesn't consist of one user profile. You might have new web developers, seasoned web developers, QA engineers, novices embarking on their first web app project, and more.

In this particular documentation scenario, Amazon Appstore's documentation relies heavily on the Android documentation, since Amazon's operating system is a fork of Android, and we try to maintain as much parity with Android as possible. It would be foolish to try to repeat and maintain so much of the foundational concepts from Android in Amazon's documentation, but at the same time, it's not wise to assume that Android developers are 100% familiar with all Android coding practices. This "Background Knowledge" section is a convenient way to bridge potential gaps in knowledge without duplicating information.

In this "Background Knowledge" section, I also add some important terms to know. Many of these terms are industry-standard terms, but some aren't. For example, "app" and "APK" mean different things, especially within the Amazon Appstore ecosystem. Further, other app stores have differing terms for apps, such as "channel," which Amazon doesn't use in the same way ("Amazon Channels" provides premium cable networks like HBO and ShowTime). Listing out important terms here that the user would need to understand the discussion helps users learn the needed language to follow the concepts to come.

The embedded terms I include in "Background Knowledge" are a subset of the total terms in the glossary. The full glossary might contain hundreds of terms important to know across the entire doc set, but for this specific topic, the terms provided are the important and relevant ones to know for the topic at hand.

Providing these mini-dictionaries at the start of a topic makes readers more apt to actually read the glossary definitions, since glancing at 10 definitions is more feasible than reading through hundreds of definitions, many of which would be irrelevant to the reader's current purpose.

Also note that I've added the terms near the beginning of the topic rather than at the end. Engineers (and philosophers and other disciplines) tend to define terms up front that they're using in arguments and other logic to follow. It makes logical sense to arrange glossary terms like this, but we might be hesitant to do so if listing the glossary terms creates a long list that pushes the more important content down. My compromise is to stuff the glossary terms inside an expandable button.

## Does your documentation use industry standard terms correctly?

Earlier I noted that in order to distinguish between familiar and unfamiliar terms, you have to understand the knowledge domain you're writing in. This is much easier to say than do. Technical writers often cover a wide range of technologies, and developer landscape runs deep and complex. As a result, technical writers often have a superficial understanding of the knowledge domain, barely able to recognize the right lingo (for example, a tech writer might know that JavaScript uses the term "function" while Java uses the term "class"). So beyond recognition of the right terms for the industry, the next question is whether your documentation uses industry-standard terms *correctly*.

So far I've assumed that *Apache Cordova*, *wrapper*, *native Android*, *HTML5 web app*, and *APK* are industry standard terms. But remember that I'm not a web app developer, so my knowledge of web app development is only cursory. The terms look right, but are they? Are they the same terms my competitors are using in their documentation? Are they the same terms used in blog articles, posts on Stack Overflow, and elsewhere? If not, users will likely be confused.

For example, look at the term "HTML5 web app." Is this term correctly aligned with the industry standard term for web apps?  Does "HTML5 need to precede "web app"? Should it be written "web app" or "webapp" (one word) or "web application"? Does the "HTML5" adjective distinguish web apps from WebViews embedded in a native Android app? What do you call Android apps with embedded WebViews?

Here is where it helps to read the competitor's documentation to get a sense of how the industry as a whole uses these terms. In this example, I searched for "web app" on [developer.android.com](https://developer.android.com) and located their topic on [Web-Based Content](https://developer.android.com/guide/webapps/). Their usage of "web-based content" (rather than web app) refers to an embedded WebView within an Android application, which makes sense given that the site is about the Android framework (and not web app frameworks, which are based on HTML5, CSS, and JavaScript rather than Java-based Android). A WebView is kind of like a mini-web browser that you embed within a page &mdash; it shows content from an external website within a specific area of your page.

Looking at the [docs for Google Play Console](https://support.google.com/googleplay/android-developer/search?q=web+app) didn't lead to many hits, because Google Play is an Android shop that only accepts Android APKs. In fact, results from Google Play Console include hits from Android as well. In the combined results, there is a topic called [Best Practices for Web Apps](https://developer.android.com/guide/webapps/best-practices) and another called [Building Web Apps in WebView](https://developer.android.com/guide/webapps/webview), but the usage and context varies significantly from Amazon. Google says,

> If you want to deliver a web application (or just a web page) as a part of a client application, you can do it using `WebView`.

Thus, with Google, you might have a web page or web application that runs on a mobile browser, and you want to bring that web page or web application into your Android APK. You can do so through a `WebView`. But with Amazon, you can upload a zip file containing your mobile web application (all the HTML, CSS, and JS files) directly into the Appstore, without packaging it into an APK through a wrapper like Cordova. (Amazon ends up just wrapping the uploaded web application into an APK on the backend during the submission process.)

By reading through the competitor's documentation, I've expanded my understanding of these terms and can see where users might experience confusion. In a future edit to my docs, I might decide to explain more of what Amazon means by web apps, how the treatment differs from Google Play, and how you can upload web apps without resorting to a `WebView` in an APK file.

There are quite a few terms to get right here besides *web application* &mdash; highly related terms include *hybrid application*, *native application*, *progressive application*, *mobile applications*, and more.

See how reading the competitor's documentation can help illuminate potential issues with terminology that I assumed were industry standard but turned out to be more nuanced and complex than originally thought? It might require some general reading on a topic (as well as consultation with engineers) before you can feel confident that you're using the right industry terms and lingo, but it's necessary.

As another example around reading the competitor's documentation, I recently undertook the task of submitting an app into Roku from beginning to end just to get a better sense of the whole Roku user journey. Right from the start, I learned that Roku calls their apps *channels* instead of *apps*. And for the app I was building with Direct Publisher, their documentation didn't refer to it as a native app or web app at all. It was just a way to build a channel by using a feed.

When you read the competitor's documentation, not only do you get a broader sense of the industry terminology, you also increase your awareness of the user's full context. Especially if users might use multiple products across the technology ecosystem, understanding the terms and other workflows in competitor products can inform your own documentation in helpful ways. You can align with the same terms, note where processes or features differ, and more.

For example, Roku has a specific JSON or MRSS feed structure that users have to conform to in order for their feeds to validate. In exploring the JSON structure, I realized that it wasn't entirely compatible with one of Amazon's frameworks, so I submitted a ticket for engineers to make an enhancement.

Granted, this kind of knowledge gathering takes time, and we might object that we barely have enough time to edit the content we have, much less undertake reading how similar terms are used across the competitor's documentation and industry at large. But this reading is precisely where terminology gets interesting. If we only look at our own company's use of terms, the definitions of the terms might seem clear and straightforward. But we run the risk of operating in a bubble, without awareness of the linguistic chaos and complexity going on outside. It blew my mind the first time I realized that Roku didn't call apps "apps" but rather channels.

As we learn about the ways different companies use the same terms, it creates more intrigue and appeal around language. There's more of a sense of something at stake for incorrect or naive term usage. Perhaps this sense of heightened stakes is enough to awaken our Stephen-Fry-like language expertise faculties and take more delight in making glossaries.

## When your company is using the wrong term...

If you find that your company is using the wrong term, you can work to change it. For example, at my work, in our app submission process, our UI used the term *binary* when referring to *APK.* I'm not sure when or where *binary* was introduced, but this term caught on and permeated project descriptions, support, and solution architect discussions.

As I was reading through the competitor's documentation (Android/Google Play) to see how they used the term "binary," I found that they didn't use the term at all. Google consistently referred to the app files as an "APK." This brought more clarity to several Amazon support tickets where users were asking what "binary" files where. I could immediately see why users (especially those who uploaded their apps into Google Play) would be confused as to why Amazon's submission interface asked them to upload their "binary."

As a result, I championed changing the term binary to APK. Changing this term was not an insignificant update, given that "binary" appeared on tabs, microcopy, error messages, and other parts of the UI, not to mention throughout the documentation, KB articles, and internal project roadmaps, and more. Most problematic, the term had saturated the language that most Amazon teams used to talk about the submissions process. Solutions architects, project managers, support, and other team members at Amazon all perfectly understand what "binary" meant and used it freely, even though most users didn't.

I'm happy to say that in this effort to change terms, I was eventually successful. We decided to replace the term "binary" with "APK."

Sometimes you can't change your product's language to align with industry-standard language. Years ago at another company, I lobbied unsuccessfully to change the term "Omnibus" in an application. It was the term that the project sponsor preferred despite hundreds of users not understanding the term.

For whatever reason, you might be stuck with either the wrong term or a non-intuitive term. In that case, you might include a parenthetical clarifier after the term when you use it. For example, before the switch from binary to APK, I frequently referred to "binaries" like this: "You can submit your binary (APK) file on the Binary Files (APK) tab."

This might seem like a passive aggressive way for technical writers to sneak in their dislike of certain terms, whispering a more familiar one with each usage. Even so, there aren't many alternatives here.

## Company-specific terms

Beyond industry-standard terms, which I've explored in depth already, what other terms might need attention? The terms unique to your company or product, of course!

Usually, any unfamiliar term that is specific to your company should appear in a glossary. Here's a great example from the [Lyft developer documentation](https://developer.lyft.com/docs/glossary). The terms they define are as follows: *Driver Rating*, *Lyft*, *Lyft Line*, *Lyft Lux*, *Lyft Lux SUV*, *Lyft Plus*, *Lyft Premier*, *Passenger Rating*, *Prime Time*, *Trust & Service* Fee. As these are all terms mostly specific to Lyft, it makes sense for them to appear in the glossary.

{: .tip}
To read more about the importance of glossaries in API documentation, check out the [Glossaries](/learnapidoc/docapis_glossary_section.html) topic in my [API documentation course](/learnapidoc/).

Returning to my initial passage for discussion ("This Fire TV Catalog plugin is based on Apache Cordova...."), *Fire TV Catalog* is a company-specific term. It should probably be linked to either the introductory topic about Fire TV Catalog or to a glossary definition about Fire TV Catalog. This term happens to be especially confusing, since catalog doesn't refer to the apps listed in Amazon's Appstore but rather to the apps whose media has been ingested into a master index of searchable media.

## Technical considerations for glossaries

<script>
$(function () {
  $('[data-toggle="popover"]').popover()
})
</script>

I've explored which terms to define, but there are other considerations with glossaries, including technical ones.  First, the glossary definition should be stored in a re-usable source so that the definition can be provided in different parts of your documentation.

For example, you'll probably want the definition to appear on a dedicated glossary page as well as embedded on the page, and maybe embedded in <a style="cursor: pointer !important; color: green; text-decoration: underline; text-decoration-style: double;" data-toggle="popover" title="tooltip" data-placement="top" data-html="true" data-content="A tooltip shows a definition or hint for some UI text or other element. Tooltips hide explanations from users who don't need them while providing a way for others to get more detail.">inline tooltips</a>. (By the way, [Jekyll](http://idratherbewriting.com/documentation-theme-jekyll/mydoc_adding_tooltips.html) is excellent at re-using definitions stored in YAML files.)

Further, you might have specialized glossaries for different products, with overlapping terms. For example, a glossary for *Alexa Skills Kit* and *Alexa Voice Service* and *Alexa Auto* (which are all different products with their own documentation) might all define the terms "near field" and "far field." These terms might also appear in the Fire TV glossary. By storing all glossary definitions in one file, and then referencing that definition where needed, you can reduce duplication.

(I won't go into technical details on how to do this, since glossaries can be implemented in a variety of ways. Certainly, if doc projects are walled off from each other, this re-use becomes difficult. But in general, you  don't want independent teams each creating their own glossaries with similar terms defined in contrasting ways.)

There are other considerations for glossaries as well. If you decide to have one mega glossary, what product sidebar should be shown for it? Is it better to have smaller, specialized glossaries that focus on the terminology for a specific product and shown in the context of that documentation, or to consolidate all glossary definitions across the site into one massive glossary?

There are pros and cons to each approach. With smaller, specialized glossaries, readers can get a sense of the 10-20 unique words they need to know. The glossary topic can also be included in the sidebar for that documentation's navigation. However, if you link one definition to another (e.g., "See also..."), you have to ensure that the links in each specialized glossary doesn't have missing references.

But with one mega glossary, it's easier to maintain, and you don't need to worry about links between definitions remaining valid. The mega glossary can be a one-stop shop for definitions across your site. Viewing the glossary probably removes users from the context of a particular documentation set, but perhaps by opening the mega glossary in a separate window, this change in context wouldn't matter.

## Glossaries make you aware of your terms

More than anything else, creating a glossary makes you aware of all unique terms you're using in your documentation. It also makes you more accountable to use them in a precise and accurate way. This kind of awakening and awareness about the language we're using in docs can go a long way towards simplifying complexity.

The next time you're working on docs, stop and take a look at your content. List out all the terms that are either jargon or which might be unfamiliar to users. It can be somewhat surprising at first. Collect these terms into a glossary for the user. It's that simple. More importantly, when we define these terms, and then realize that the definitions are much more fuzzy than we originally thought, it helps expose why our docs get to be so complex in the first place.

## References

["Defining Glossaries."](http://www.ingentaconnect.com/search/article?option1=tka&value1=defining+glossaries&pageSize=10&index=1) Michelle Kidd Tackebary. *Technical Communication*. Volume 52, Number 4, November 2005.

["The ABCs of Writing a Technical Glossary."](http://www.ingentaconnect.com/contentone/stc/tc/1998/00000045/00000001/art00003), by Evie Gray, William Ingram, and Dennis Bodson. *Technical Communication*.  First Quarter 1998,
