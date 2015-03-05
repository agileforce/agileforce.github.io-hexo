title: Getting Started with Github for versioning Salesforce Metadata
date: 2014-10-10 19:42:57
tags:
- salesforce
- git
---

Using [Git](http://git-scm.com/), [Github](https://github.com) and the [Force.com CLI](https://developer.salesforce.com/page/Force.com_IDE) you can easily record all the changes you make to the behaviour of your Salesforce Org.  Having a history of all the changes can be invaluable, allowing an easy way to track down issues and document how your Org was developed.

> In this guide we will cover a very easy way to use Git and the essentials of the Force.com CLI.  You can of course download all your Salesforce Org Metadata with other tools such as [MavensMate](http://mavensmate.com/) and [Force.com IDE](https://developer.salesforce.com/page/Force.com_IDE).

<!-- more -->

<div align="center">
<iframe src="//www.slideshare.net/slideshow/embed_code/40125265" width="427" height="356" frameborder="0" marginwidth="0" marginheight="0" scrolling="no" style="border:1px solid #CCC; border-width:1px; max-width: 100%;" allowfullscreen> </iframe> 
<div style="margin-bottom:5px"> <strong> <a href="https://www.slideshare.net/JR0cket/dreamforce14-metadata-management-with-git-version-control" title="Dreamforce14 Metadata Management with Git Version Control" target="_blank">Dreamforce14 Metadata Management with Git Version Control</a> </strong> from <strong><a href="http://www.slideshare.net/JR0cket" target="_blank">John Stevenson</a></strong> </div></div>

## Getting Started with Github

[Github](https://github.com) is a cloud service for managing source code and configuration files.  You can use it manage all the changes you make to any text files in your project and easily share those changes with other developers.   Github also gives a visual way to compare changes between versions (a visual diff).

As all the Metadata in your Salesforce Org is essentially a collection of text filescontaining XML, then its easy to use Github to manage all your changes.  You can of course also manage all your Apex, Visualforce, JavaScript and HTML5 code too.

To get started:

1)  create a free account on [Github](https://github.com)
2)  install the Github desktop app ([MacOSX](https://mac.github.com/) or [Microsoft Windows](https://windows.github.com/))


## Create a Github Repository for your Salesforce Metadata

Once you have your Github account you can create a new repository.  A repository is a simple data store that will hold all the changes made in your project.

In this example I have created a Gardening app in my Salesforce developer org, so I will created a repository on Github called gardening-app

![](/images/s1-github-repository-new-gardening-app.png)


## Setting up the Github App

Run the Github desktop app installed earlier.  If this is the first time you have used the Github app, you will need to configure it with your Github login details:

![](/images/github-app-login.png)

Next you need to tell Github app your name and email address.  This is used to record who has created a change in your repository.  Its common practice to use the same name and email address you used when you created your Github account.

![](/images/github-app-config-identity.png)

Finally, the Github app will check your computer for existing Git repositories.  If you do not have any or do not wish to add any repositories on your computer at this time then just press **Done**.


## Using the Github App to download the Gardening App repository

So far, the Gardening App repository I created is only on Github.  Whilst you can add and edit files via the Github website, if you are working on more than one file at a time it is easier to copy the repository to your computer.

{% img img-topic /images/github-repository-clone-steps.png %}

The Github app makes copying a repository easy and uses the term Clone.

1) Click the Add button

2) Select Clone

3) Select the Gardening repository or type in the name of your repository if you have many repositories already on Github

4) Select the Clone button to copy all the files of the repository from Github to your computer.

You are then prompted as to where you want the files to be created.

In my project directory I have a directory called salesforce which I selected as the destination.  The repository from Github is then copied into a file called s1-gardening-app in the salesforce directory.

![](/images/github-app-repository-no-changes.png)

Any files you add or changes you make to existing files will be detected automatically by the Github app.  So its time to get the Metadata from your Salesforce Org

You are now ready to get the metadata from your Salesforce Org and version it with Git.  See the article on how to [manage metadata with Git and Force CLI](http://agileforce.co.uk/managing-metadata-with-git-and-force-cli) for details on how to do this.
