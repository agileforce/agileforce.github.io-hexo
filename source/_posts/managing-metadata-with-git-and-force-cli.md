title: Managing Metadata with Git and Force CLI
date: 2014-10-11 09:25:09
tags:
- force
- git
---

  In this article we will show you how to save the app you are building for the Salesforce Hackathon in Git using the Salesforce Force.com CLI.

> The Force.com CLI is a really powerful tool for interacting with your Salesforce Org.  You can create new custom object, run queries and in this case download all the Metadata or any part of the Metadata from your Org.

<!-- more -->

## Clone the BeMyApp repository

You should have recieved a repository from BeMyApp, called something similar to `repository-123`.  Using a Git client such as Github for [Mac](https://mac.github.com)/[Windows](https://windows.github.com), [SourceTree](http://sourcetreeapp.com/) or [Git command line](http://git-scm.com).

The Git command line is:

    git clone https://github.com/bemyapp/repository-123.git


## Getting Saleforce Org Metadata using the Force.com CLI

First you need to create an unmanaged package in your Salesforce Org, containing all the artefacts you want to manage.  If you create an App in your Salesforce Org then simply add that.

{% img img /images/salesforce-gardening-packages-new.png %}

If you created an App in your Salesforce Org, then you can simply add that App and it will include all the relevant metadata.

{% img img /images/salesforce-gardening-package-add-app.png %}

> If you have created a Custom App and included tabs for you Custom Objects and Visuforce Pages and Canvas Pages to the Custom App the Force.com platform will automatically add any dependent resource such as Apex classes and Static Resources for you.


## Installing the Force.com CLI

Download the appropriate file for either [MacOSX](https://github.com/heroku/force/raw/master/binaries/darwin-386/force), [Windows](https://github.com/heroku/force/raw/master/binaries/windows-386/force.exe) or [Linux](https://github.com/heroku/force/raw/master/binaries/linux-386/force).

Save this file to a place on your operating sytem execution path (`$PATH`)

> On Mac & Linux you can move the `force` file in the directory `/usr/local/bin` using the command `sudo mv force /usr/local/bin`.


## Using the CLI to get an unmanaged package

You can use the force cli to download and unpack the package you created in your Salesforce Org into a folder called `metadata`.

```
force fetch package <packagename> --unpack
```

A browser window will open and you are prompted to enter your Salesforce Org username and password.  Then select `Allow` so the force cli tool can connect to your Salesforce Org and download your package.

> If you are using Chrome, you may experience a blank page after allowing access from Force CLI.  In the browser URL window, click the sheild icon on the right hand side and select "Run insecure script"

You should now have a directory called `metadata` in which is a sub-directory named after your package.  This sub-directory contains all the artifacts that you specified when you created your unmanaged package (custom objects, custom fields, page layouts, etc).


## Saving your changes to Github

Once the metadata is downloaded, your add and commit all the files to your local git repository as usual.

```
git add .
git commit -m "first git challenge"
```

Now you can share that commit with the repository given to you by BeMyApp using the command

```
git push origin master
```

Now get back to hacking your App.

Thank you
