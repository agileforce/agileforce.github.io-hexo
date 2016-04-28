title: london's calling you, salesforce - Lightning to the nation
date: 2016-02-05 11:35:33
categories: events
tags:
---

{% img img-topic /images/londons-calling-banner.png %}

Continuing my [London's Calling](http://www.londonscalling.net) live blogging we move onto the Salesforce Lightning talks.  Lightning is a new extension to the Salesforce platform, allowing you to build apps with a modern user experience

* Part 1: Getting Agile with Testing code in Salesforce
* Part 2: A career of fun & discovery

<!-- more -->


# Lightning Apps & Events 

{% img img-topic /images/salesforce-lightning-app-builder-devices.png %}

Lightning is the new way to build Salesforce apps on the platform, giving a modern user experience. Barry Hughes did an excellent job of showing how he took an existing Visualforce & Angular.js single page app and recreated it using Lightning, the Lightning Design System and [Salesforce Labs SLDSX sample components](). 

Taking an existing Visualforce single page app, Barry walked us step by step in rebuilding that app using Lightning, showing how to 

Q from the audience - which would you build tomorrow, Lightning or Visualforce/Lightning?
- spa's
lightning events are much more flexible than Angular.js routing

...

* [Lightning Single Page App (SPA) from a Visualforce SPA: Project Timesheets Re-visited](http://www.londonscalling.net/sessions/creating-a-lightning-spa-from-a-visualforce-spa-project-timesheets-re-visited/) by [Barry Hughes] in **Alt room**


No routing mechanism in Lightning
No examples to find
How do I handle CRUD operations without introducing memory leaks
SLDsX - gives a range of components that provide a tabbing navigation 
Apex is a conduit to accessing the salesforce data, Lighting apps themselves should not access the records directly.


Lightning apps save data by calling Apex

This spa component can now be used by dragging onto the design of an app using Lightning App builder

conclusions (photo)

Lighting is still evolving

unit testing is not covered yet, this is something that many are looking to learn from Keir Bowdens talk later today

No way to test a lightning event at present, so we still need to learn how to test these interactions

devinthecloud.worldpress.com 

## Lightning Style - design system

{% img img-topic /images/salesforce-lightning-experience-multi-device.png %}

Fabien showed how we can all use the beautiful and delightful Salesforce Lightning Experience design in our own apps...

----Rewrite
Salesforce recently unveiled Lightning Experience, the next step of it’s evolution. This includes a whole new and beautiful UI, but with this comes a new question: How can we create applications that match this new look & feel? Come see how to use Lightning Design System inside your application, no matter what technology you’re using: VisualForce, Lightning Component or even outside of Salesforce!
----Rewrite

* [Style your application with Lightning Experience Look & Feel using Salesforce Lightning Design System (SLDS)] by [Fabien Taillon - @], organiser of the Paris Salesforce community

# Lightning Power - Components

{% img img-topic /images/trailhead_module_lightning_components.png %}

The power that allows you to build Lightning Apps so fast are the Lightning components.

----Rewrite
Maybe you’ve done the Lightning Component Trailheads or perhaps you’ve read the developer guide? If so you’ve probably started to scratch the surface of various advanced programming concepts such as component facets, passing functions as parameters or dynamic creation of components or event handlers? Or maybe this is the first you’ve heard and you’re curious to see what’s possible? Either way, if you’d like to know more this session is for you!

Over the course of 30 minutes I’ll walk you through these concepts and by example show you how and more importantly why you want to use them to build awesome Lightning components.
----Rewrite


* [Advanced programming with Lightning Components](http://www.londonscalling.net/sessions/advanced-programming-with-lightning-components/) by [Thomas Waud]() - **2.45pm in Cmd room**



# Careers for all

Its never been a better time to have Salesforce skills, there are so many opportunities out there.

It takes all sorts of people and talents to make the Salesforce community a success.

There are big opportunities for exciting careers, but the array of choice can make navigating “what next” a bit bewildering. If you’re at a decision point in your career, or just looking for inspiration on new avenues, join our interactive panel and talk to folks who have all navigated different routes through the Salesforce world, have views on job market trends and share thoughts on any questions you have on your career and skills.

* [Salesforce’s calling – where can your Salesforce career take you?](http://www.londonscalling.net/sessions/salesforces-calling-where-can-your-salesforce-career-take-you/) by [Mary Youngs](https://twitter.com/maryyoungs) in Ctrl room 


Panel:
- Alex Wallwork - admin, consultant
- Mary Youngs
- Luke Emberton - Cloudsherpas CTA, Director of Technology
- Anup Jadhav - Startups, MVP
- Rich Law, Cloud Sherpas, Charity & 3rd Sector, consultant


# Trailhead: the path to enlightenment

[Pauline Dufour](https://twitter.com/Paulinedfr) and I were showing Trailhead to those unfortunate few who had not yet had the chance to join in the fun.

![Trailhead in action](/images/salesforce-trailhead-animated.gif)

> Talk a journey through Trailhead and start earning your badges (or earn even more if you have started already).  Sign up (or sign in) today at [developer.salesforce.com](https://developers.salesforce.com/trailhead) 


## Demo Jam

Just before lunch everyone gathered to watch some amazing demo's of the Salesforce platform.

...


# Talks I wanted to see

There were so many great talks, I couldnt get to see all I wanted.  Luckily, the venue we are in, SkillsMatter, recorded all the talks and they will be available soon.

So here are some of the talks I hope to catch up on in the next few weeks

Carolina ...

* [Building a web application with Google Places API & Lightning Connect](http://www.londonscalling.net/sessions/building-a-web-application-with-google-places-api-lightning-connect/) by []() - how to take advantage of an external data provider such as Google Places for building an application in Salesforce, for example showing nearby locations from Google Places API in real time & recommend other locations based on your relationship with other users

* [How To Code Logic Your Admin Will Love And Use](http://www.londonscalling.net/sessions/how-to-code-logic-your-admin-will-love-and-use/) by [Roy Gilard], leader of the Tel Aviv Salesforce community.

* [Asynchronous processing for fun and profit](http://www.londonscalling.net/sessions/asynchronous-processing-for-fun-and-profit/) by [Matt Bingham - ] - a crash course on all the different flavours of deferred & bulk processing in Apex. Learn to spot antipatterns and common async use cases, while keeping things predictable, testable and developer friendly.

* [Using Cognitive Computing in Salesforce.com to drive more valuable outcomes](http://www.londonscalling.net/sessions/using-cognitive-computing-in-salesforce-com-to-drive-more-valuable-outcomes/) - using the power of [IBM Watson](http://www.ibm.com/smarterplanet/us/en/ibmwatson/) to analyse a range of personality attributes to help discover insights about our customers from within Salesforce.

* [5 Things I Love About the Salesforce Marketing Cloud](http://www.londonscalling.net/sessions/top-5-things-i-love-about-the-salesforce-marketing-cloud/) - by Reid Carlberg who is a pleasure to listen to regardless of the topic.


There are so many more I havent mentioned, I'll watch them too when I get chance.

# Summary

London's Calling has been an amazing community driven event and I give my thanks to the organisers who spend months in the planning of this event.  Also thanks to the sponsors that helped make this possible and of course all the amazing people who spoke or attended the event.

Thank you all.
[https://twitter.com/jr0cket](John Stevenson - @jr0cket)

> London calling, yes, I was there, too.
> An' you know what they said? Well, some of it was true! 
> London calling at the top of the dial
> After all this, won't you give me a smile?
> London calling
>
> I never felt so much alike [fading] alike alike alike
>
> Copywright: The Clash, 1979


![Trailhead - Battlestations](/images/salesforce-trailhead-battlestation-banner.png)
