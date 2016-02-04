title:  External Objects 
---

# Overview 

External Objects provide an ability for the Salesforce Platform to reach out to an external system and use its data, without having to store that data in your Salesforce Org. 


## Use Cases 
How often have you wanted to view large volumes of data from external or on-premise systems within Salesforce? The solutions usually play out as follows…

Avoid having to store everything in Salesforce.  Moving everything to the cloud does require time and care not to include data that wont be directly valuable.

  By orchestrating search over a wide range of back office and external data sources, External objects allow you to treat the world as if it was just part of Salesforce.




## Article What is Salesforce Lightning Connect and External Objects?

Posted by Tquila on 11 November 2014

This post is Part 1 of a two part series on Lightning Connect and External Objects. This first post discusses the technology and the capabilities, the second will walk you through the steps to set up Lightning Connect in a Developer Edition Org.

External Objects were first described in the Winter ‘15 release notes. External Objects provide a native platform ability for Salesforce to reach out to an external system and pull in the data it requires to display in Salesforce. How often have you wanted to view large volumes of data from external or on-premise systems within Salesforce? The solutions usually play out as follows…




A large retail company looking to present their Customer Service Reps with the customers retail transactions from an on-premise Enterprise Resource Planning (ERP) system. How would we do this?

    Load the data into Salesforce: There are tens of millions of records so will need to manage the volumes and archiving to mitigate data storage, the data will essentially be duplicated for the purpose of presenting it to the user.

    Callout to a web service: Requires the external service to serve the data to Salesforce. Will need to define APIs and mechanism for presenting the data and custom UI for presenting this alongside the customer in Salesforce.

Both of these options are time consuming and involve a lot of effort and therefore cost. The truth is that unlocking data can be an expensive job.
Lightning Connect and External Objects

Lightning Connect is the new name for External Data Sources which was announced in the Winter '15 release notes just before Dreamforce. External Data Sources and External Objects are still the setup features used to manage Lightning Connect and Files Connect.  
Let's Dig into External Objects

External Objects allow for data to be exposed to Salesforce but not persisted on the platform. This is a nuanced distinction. In the old world, with our initial requirement we would weigh up the differences, we would discuss if the data would be valuable for driving workflow, or for reporting. If yes to one of these was a tick in the column for loading the data and persisting it in in Salesforce column, a no meant a vote for a web service to present the data will be just fine. With External Objects there is a new option. 

External Objects essentially provide a wrapper around the oData protocol which does initiate web service calls to retrieve the data as it’s presented on the screen or queried. This allows the data to be tightly integrated into the platform and used in standard layouts, and even SOQL, SOSL and APIs. Remember, this data is never stored in Salesforce but pulled in on demand through web services, this means you avoid the unnecessary (and expensive) limits and costs of data storage.

External Data Sources are mapped and synced to a new type of Custom Object in Salesforce called External Objects (suffixed __x). These are defined through setup declaratively. To use External Objects  your data needs to be exposed as an oData source. I am no expert on oData (yet) so you can read more about it here. Once exposed as an oData source you then configure your External Data Source. Salesforce and the oData protocol work their magic and define your External Object definitions for you including custom fields and data types (we will step through this process in the follow up post).

External Objects do not support workflow or reporting (reports not available at present but planned) but they are exposed to List Views, Related Lists, Global Search, even natively on Salesforce1 mobile. Also, I just found that mini page layouts work when you hover over recent items. What is even cooler is that the External Objects are natively exposed to SOQL, Apex and APIs. This means you can build custom charts, custom UIs or simply leverage standard tabs and page layouts. This is killer for unlocking your data. Expose via oData to Salesforce and it’s unlocked through not just the Salesforce platform but anything that can poke at the APIs too!

Indirect Lookups allow you to link a field on your External Object, e.g. CustomerID to an External ID field on your Standard or Custom Object. This is great, and simple to achieve. Once you have set-up your Indirect Lookup the External Object will be available as a related list on your page layouts and can be used for joining SOQL queries. This is such a great feature as your users won't have a clue that the data they are viewing is actually coming from somewhere else. This is explained in more details in the follow up post where we set up External Objects. 

Although External Objects are read-only (for now, oData does support full CRUD), Chatter is supported on External Objects however fields cannot be tracked and attachment are not allowed, even in the feed – you can try but you’ll get a funky error dialog.
Real life (limits and the decision to actually use it in the wild)

In real life you may not have an oData service lying around. If you have data buried in an ERP then you can have a partner product to translate the protocols for you. The only services I am aware of that natively support oData are SAP and Sharepoint (Files Connect).

At Dreamforce, Salesforce highlighted a number of integration partners supporting oData including Informatica Cloud, Jitterbit and Mule (to name a few). Each of these products have connectors for Salesforce and most of the data sources. These should be able to translate your non-oData data sources into the oData standard.

As this is real life we have to consider actual feature set and latency. I have not tried this real life scenario yet as I havnt got a large scale ERP system to hand, but I have tried with a publicly available oData source and it just worked, straight away. oData is a standard, Salesforce have implemented that standard, so it should just work. As for latency again real life will have to tell you this -  it depends on the originating data source, database performance (e.g. column indexing), the network, and firewalls etc. But in the tests I have done with a free publicly available data set you really couldn't tell it was being loaded separately from the rest of the data being displayed. Perhaps when testing extensively with SOQL and API you will see latency but that testing is for another day.

In real life we deal with limits on the platform. This was the #1 question from my colleagues – can this really be used without butting heads with limits. What’s great is that all of the limits are available online (links at end of post). 

The most notable technical limit is that an Org is limited to 10,000 OData queries per hour, with higher limits available to purchase. 

Salesforce queries the external data source via web service when:

    A user clicks an external object tab for a list view
    A user views a record detail page of a parent object that displays a related list of child external object records
    A user performs a global search in Salesforce or Salesforce1 mobile app
    An external object is queried via the APIs, Apex, SOQL, or SOSL

The flat cap of queries per hour rather than being mapped to the number of users within the org may make the feature difficult to implement in large Orgs as estimating the cost comes down to a measure of usage. I would assume the limit was set at a sensible benchmark where most customers will comfortably sit within. The decision to use flat limits is an odd one especially when the model for API rate limiting works well when it’s pegged to users in the Org. I would like to see this adopted as the model for other rate limits such as Streaming API and oData Queries.

An interesting feature is the option for ‘High Data Volume’. This essentially turns off one or two things to allow you to break through some of the limits. This means it is only necessary for specific scenarios. According to the documentation,  ‘High Data Volume’ bypasses most of the rate limits, but means the External Objects aren’t available in Salesforce1 and don’t support record feeds.

Lightning Connect Consideration and Limits - More information here 

External Data Limits - More information here
Conclusion

Lightning Connect can potentially solve some important use cases and further position Salesforce as the modern front end for your back office and legacy systems. The ability to interact with External Objects through SOQL, SOSL, Apex, and APIs is killer. This allows you to truly unlock data that you thought was siloed in your legacy systems. I am really looking forward to getting hold of this in the wild. I can already see a few great applications for Lightning Connect when reviewing some of the solutions in the Tquila pipeline. 

In the next post I will walk you through the steps for setting up Lightning Connect using a publicly available oData source.
