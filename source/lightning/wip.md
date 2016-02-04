## Presentation 

* Overview 
- what is lightning connect 
- what value does it bring 
- who uses it 

* How to use lightning connect 
- Configure an external data source 
- Configure one or more external objects 
- Use Salesforce as usual - desktop & mobile

# External Objects 
- what are they 
- are they just for Lightning connect ??
- what other uses do they have ?

# OData Providers
- simple protocol to build in your own languages 
- example apps & tools
- building your own app

# Heroku Connect 

# Partners 
- Jitterbit, et al.

http://www.jitterbit.com/blog/announcing-the-new-jitterbit-lightning-connector-for-salesforce/


# Lightning components 
- using with Lightning components

# Thank you & Resources 

https://developer.salesforce.com/lightning

Lightning connect product overview - https://www.youtube.com/watch?v=nSi_sD8Rqow

Slides
https://slideshare.net/jr0cket


Messages 
- unlock your back office data with Lightning connect - simple & effective way to use data from your entire company without expensive system integration projects

- make use of ever increasing public data (weather & traffic info for teams out on the road) and create innovative apps that helps everyone in the business be more effective and collaborate

Old-style batch integration is no match for the demands of our always-on digital world. Salesforce Lightning Connect goes native with real-time connection.

http://diginomica.com/2014/11/13/salesforce-adds-native-real-time-integration-lightning-connect/


It will allow you to store the data off platform but utilise a special kind of Custom Object to view it.


Track and represent data from sources outside Salesforce by creating external objects. Each external object maps to a table in a data source outside Salesforce, such as SharePoint®, and allows you to set up access to its data from search and custom tabs in Salesforce. Each external object relies on the connection details stored in an external data source definition.

Managing External Data Sources

Define external data sources to manage connections with data sources outside of Salesforce, such as SharePoint®. An external data source definition contains connection and authentication information to access external data. Once an external data source is set up, its visible content is mapped to external object definitions to enable searching for external data in Salesforce.

Data Integrations

Salesforce offers a rich library of programmatic and declarative integration tools to implement business logic spanning multiple application systems.

LIGHTNING CONNECT
Use data from any external data source in real time with any application you create on the Salesforce1 Platform. Instead of spending months integrating legacy systems, you can easily connect and access data in real time to incorporate that data into any application.

HEROKU CONNECT
Easily sync data between your Heroku customer apps and your Force.com employee apps. Loyalty apps, buying experience apps, marketing campaign apps, and Internet of Things apps are among the many use cases where Heroku Connect delivers the customer experience you want, with all of the data going back to your employee-facing applications.

https://developer.salesforce.com/blogs/developer-relations/2015/02/salesforce1-lightning-overview.html

http://trivia1.herokuapp.com/

https://chrome.google.com/webstore/detail/salesforce1-simulator/cknbjckicenodbiaejbmkjhldffonggp?hl=en-US

https://developer.salesforce.com/blogs/developer-relations/2015/02/access-salesforce-data-external-sources-lightning-connect.html

Build your own odata with node & mongo
http://appirio.com/category/tech-blog/2015/03/tutorial-powering-lightning-connect-with-mongodb/

http://www.odata.org/
http://www.odata.org/blog/salesforce-external-object-integration-using-lightning-connect-with-odata/

## Partner connectors
http://www.jitterbit.com/blog/announcing-the-new-jitterbit-lightning-connector-for-salesforce/

http://www.tquila.com/blog/2014/11/11/what-salesforce-lightning-connect-and-external-objects

http://tquila.com/blog/2015/02/20/data-warehousing-heroku-postgres-and-salesforce1-lightning-connect

http://creation.technology/salesforce-lightning-connect-odata/

http://cloudyworlds.blogspot.in/2015/01/lightning-connect-and-sql-integration.html


https://developer.salesforce.com/blogs/developer-relations/2015/03/external-objects-lightning-connect-poc-in-5-days.html
https://developer.salesforce.com/page/Building_a_Data_Integration_Proof_of_Concept_Using_Lightning_Components

https://developer.salesforce.com/blogs/developer-relations/2015/02/lightning-strikes-trailhead.html
http://peterknolle.com/process-automation-trailhead-review/

https://help.salesforce.com/HTViewHelpDoc?id=external_object_define.htm


#IoT
http://reidcarlberg.com/2015/03/05/access-iot-data-in-salesforce-with-heroku-connect-odata/

Heroku Connect
https://developer.salesforce.com/blogs/developer-relations/2015/02/simple-data-integration-heroku-connect.html

https://blog.heroku.com/archives/2014/11/13/heroku-external-objects

https://www.heroku.com/connect
https://devcenter.heroku.com/articles/herokuconnect
https://addons.heroku.com/herokuconnect

External Objects
https://www.youtube.com/watch?v=GGvCcuTbhZE


OData sources & partners
Obviously, not every data source supports OData natively. Which is why Salesforce is pushing on an ecosystem drive that brings partners like Informatica, Jitterbit, MuleSoft, Progress Software, SnapLogic and SoftwareAG into the jamboree. Those guys have built their businesses on helping customers move enterprise data around between systems and delivery models; with some friendly peer pressure from Salesforce, they now support OData and Lightning Connect.

IT organizations spend less time worrying about how to get all their data into Salesforce and more time just doing it. In turn, workers at those organizations will be able to do things like check inventory data from within the Salesforce1 mobile app for potentially the first time ever.  That's going to be the sales pitch for Salesforce as it continues to go after bigger companies.

Large enterprises are definitely the target demographic for Salesforce1 Lightning Connect: With subscriptions starting at $4,000  a month, depending on the number of data sources



## Lightning sample apps

https://developer.salesforce.com/blogs/developer-relations/2015/02/lightning-components-sample-app-belgian-beer.html


## Process builder
http://www.tquila.com/blog/2015/03/09/bulkify-lightning-process-builder





# Article: Salesforce adds native real-time integration with Lightning Connect

SUMMARY: Old-style batch integration is no match for the demands of our always-on digital world. Salesforce Lightning Connect goes native with real-time connection. 

Two electric cablesSalesforce.com has today officially released Salesforce1 Lightning Connect, which brings data in real time from back-office systems into applications built on the Salesforce1 Platform. The technology, which uses the OData open data access protocol, was demonstrated at last month’s Dreamforce conference, and has been in pilot for some time under its earlier name of External Data Objects.

Connect is designed to provide the real-time access to information that people increasingly expect in today’s digital world, but which has posed a huge challenge using traditional methods of integration between different applications and data stores. As Adrian Kunzle, product management lead for platform services told me in a pre-briefing:

    What we’re trying to do is lower the economic hurdle and make it easier to bring that data in that you wouldn’t otherwise do because it’s too expensive.

Typical use case

A typical use case demonstrated by Salesforce.com is to bring sales order data from a back-office system such as SAP into the Salesforce application where it can be viewed within the Salesforce account record for that customer.

Previously, this would typically have been achieved by exporting the data from the ERP system as an XML file and then processing it within the Salesforce environment. This involved a batch process to export the data and extra coding to complete the integration. It was long-winded, said Kunzle.

    [There was] a lot of drag associated with that. It didn’t neatly fit into everything that is the Salesforce platfrom. Now it all just fits into the mechanisms that are already there.

With Lightning Connect, the data is accessed directly from the source system without being copied across, but still appears to the Salesforce platform as a native custom object. This means the external data can be brought into existing desktop or mobile applications, added to custom apps using the Visualforce drag-and-drop development tool or Apex coding, or included in search results or API output.

While the current release is read-only, Kunzle told me future versions will include the ability to write to the external data store.

    What’s going GA now is read-only. In the next release we’ll be piloting write. You’ll be able to edit this object and any change you make to the data or the status will be remote posted back to [the source].

    That’s quite exciting for things like approvals because you’ll be able to change approval state on the Salesforce side.

Enterprises will want to consider carefully how they implement connections. There will normally be a single authentication for all connections to a source, although the ability to view specific accounts or data within Saleforce will still be governed by Salesforce’s own user access management controls.

Salesforce also today announced Heroku External Objects, which adds the same native real-time connectivity to its Heroku Connect technology.
‘Code-free’ integration

Although it shares the same ‘Lightning’ branding as the platform’s component development framework, Connect can be used independently. The most common use case is nevertheless likely to be a Salesforce administrator using the drag-and-drop Visualforce environment to add external data into an existing application. In its press release today, the company claims: “integration can now be completely code-free, allowing any user to quickly connect data with just a few clicks.”

Of course that will still require co-operation from colleagues in IT to make the source data available within the Salesforce environment. When they have done their part, the external data sources and any objects created will appear on a side menu in the Force.com environment.

Once users have connected to a data source, they can then ask the tool to automatically built a custom object based on the structure of the external source. Using a shared reference ID to match records they can then create a lookup within the Salesforce application, such as a list of sales orders in the Salesforce account view.

Salesforce says that its integration vendor partners, including Informatica, Jitterbit, MuleSoft, Progress Software, SnapLogic and SoftwareAG, have built an extensive library of OData compliant adaptors for Lightning Connect.

The new Lightning Connect functionality is enabled in Developer Edition but customers will have to pay extra to use it in production. Pricing starts at $4000 per month per data source.
My take

The ability to bring real-time data from a completely different system directly into another application in the way that Salesforce.com can demonstrate with Lightning Connect is quite a breakthrough. For a long time I’ve been saying we should stop using the term integration and start talking about connection instead. That’s because the concept of integration comes loaded down with a lot of assumptions that date from the client-server era, when joining separate applications or data sources together was something you did as a one-off project that you hoped you’d never have to revisit.

That won’t do in the digital era, when applications and data sources are constantly changing and adding new fields and features. A one-off integration will quickly become obsolete. Instead, you have to start thinking in terms of continuous connection that can tolerate changes in both the source data and the destination application. You have to deliver the data in real-time, too, because in a digital world, the data is constantly changing and yet people expect to get answers and make decisions on the spot. In such circumstances, the compromises and workarounds of old-school integration create more problems than they solve.

Lightning Connect takes a fresh approach, building on the OData protocol which uses the REST principles of data access that grew up with the Web. Bringing data in this way into Salesforce’s continuously upgradeable application development platform achieves the seemingly impossible goal of delivering change-tolerant connection to real-time data.

Of course it’s far from perfect for now. This first generation of the technology is read-only, and there’s more work to do before it can be extended to accept editing from within Salesforce. As I understand it, access to the data source is effectively single-user at present, and enterprises will have to manage that very carefully to ensure there are no adverse security implications.

Nevertheless, this is an important leap forward in capabilities. It’s so different from the long-established processes of exporting, scrubbing and then remarrying data that it will have some scratching their heads in dismay. In my view, it raises the bar in terms of what we should all expect going forward when we talk about connecting applications and data.

