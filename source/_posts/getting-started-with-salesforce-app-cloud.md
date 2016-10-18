title: getting started with salesforce app cloud
date: 2016-07-25 09:22:22
categories: app-cloud
tags:
- app-cloud
- beginners

---

{% img img-thumbnail /images/salesforce-app-cloud-logo.png %}

With Salesforce App Cloud you can rapidly create business apps with Force.com and deploy & scale bespoke apps using Heroku.  Salesforce App Cloud is a entirely hosted platform which offers free developer environments (no credit card required).

Lets take a high level view of the Salesforce App Cloud, specifically Force.com and Heroku.

<!-- more -->

{% img img-topic /images/forcedotcom-concept.png %}

# Force.com - apps & services for your business

[Force.com](https://developer.salesforce.com/platform/force.com) is for building apps that support the people in your organisation and as a single source of data for all your enterprise services.  Force.com also has reporting & analytics tools and API’s for visualising and interpreting data.

Force.com provides a central application server, abstracted database and enterprise services all available via a range of [open API’s](https://developer.salesforce.com/trailhead/api_basics/api_basics_overview).

Applications are created by modeling objects, defining business processes and configuring UI elements, all without having to write code.  Any additional custom business logic is written in Apex (a Java like language) and custom UI can be coded in HTML5 or Javascript frameworks, such as [Salesforce Lightning Components](https://developer.salesforce.com/trailhead/en/module/lex_dev_lc_basics).

# Heroku - scaling custom apps & services

![Heroku languages](/images/heroku-languages.png)

[Heroku](https://heroku.com) is like having your own personal DevOps team at your fingertips.  You can write custom applications in your favorite language, framework or architecture and let Heroku deploy and scale them for you easily.

Heroku also provides a range of on-demand Relational & NoSQL databases and 150+ other services to speed up the development process.  Create a Postgres, Redis, Mongodb or Kafka persistence service at the click of the button.

See how easy it is to deploy and scale your favorite language with the [Heroku Getting Started Guides](https://devcenter.heroku.com/start).

# Integrating your Apps with Salesforce via Force.com

Force.com has [a wide range of secure API’s](https://developer.salesforce.com/trailhead/api_basics/api_basics_overview) with which to integrate your own applications.  Any applications built on top of Force.com automatically become available via the Salesforce APIs.

Typically your own applications will use the [Salesforce SOAP API](https://developer.salesforce.com/trailhead/api_basics/api_basics_soap) or [REST API](https://developer.salesforce.com/trailhead/api_basics/api_basics_rest) for integration.  Other common API’s include the [Bulk API](https://developer.salesforce.com/trailhead/api_basics/api_basics_bulk) for loading large data sets and [Streaming API](https://developer.salesforce.com/trailhead/api_basics/api_basics_streaming) which lets you push a stream of notifications from Salesforce.  Salesforce also provides the [Force.com Web Services Connector](https://developer.salesforce.com/page/Introduction_to_the_Force.com_Web_Services_Connector), a high-performing Web services client stack implemented with a streaming parser that is the preferred tool for working with salesforce.com APIs.

To call your own API’s and services from Salesforce, we provide [Apex Integration Services](https://developer.salesforce.com/trailhead/module/apex_integration_services).

All the Salesforce API’s are available from any applications that are defined as Trusted in Salesforce and run over HTTPS, such as those deployed on [Heroku](https://heroku.com).  Those Heroku deployed apps also have the [Salesforce Connect service](https://developer.salesforce.com/trailhead/module/lightning_connect) available via (Heroku Postgres)[https://postgres.heroku.com] to automatically synchronise data between Salesforce and your custom applications.

# Trailhead - learning App Cloud

{% img img-topic /images/trailhead-banner.png %}

We created Trailhead to interactively help to build applications on the Salesforce App Cloud, asking questions and setting challenges so you can evaluate your skills along the way.  If you are just starting with Salesforce, try the [Developer Beginner trail](https://developer.salesforce.com/trailhead/trail/force_com_dev_beginner).

# Sign up Free Developer Environments

Force.com - sign up at https://developer.salesforce.com/trailhead for a Trailhead login to track your progress.  The same account also gives you a free Force.com developer environment with all the features of a production enviroment, only limited by number of accounts & rows of data.

Heroku - sign up at http://heroku.com and download the [Heroku CLI](https://toolbelt.heroku.com) tool and start deploying your apps, provisioning services and getting back to focusing on your app development.

In the next article in this series we will discuss Open Banking applications and services to help inspire your own ideas on how you could use the Salesforce App Cloud.  In the mean time, checkout [developer.salesforce.com](https://developer.salesforce.com) for more examples of building apps in the Cloud.

Thank you
John Stevenson
[@jr0cket](https://twitter.com/jr0cket)
