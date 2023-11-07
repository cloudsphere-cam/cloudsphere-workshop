---
title: "Insight Consoles" #
chapter: true
weight: 3 # MODIFY THIS VALUE TO REFLECT THE ORDERING OF THE MODULES
---

# Insight Consoles
**In addition to the Explorer UI, CloudSphere has an extensive collection of detailed dashboards and reports that provide valuable insight related to your scanned environment(s)**

### Insight Consoles Overview

Selecting the Insight Console option in the left nav menu will open a new browser tab.

![Console home](/images/consolehome.PNG)

To get started, let's first navigate to the Executive Summary console using the link in the top right of the screen.  

![Exec Summary home](/images/execsummaryhome.PNG)

This console contains a wealth of high level detail related to the environments scanned.  Geographic mapping, as well as summary detail on IT Elements, Application Types and Database vendors are all available in the top row at a glance.

The second row of data contains detail related to the services mapping in the environment, as well as the review status and more.  

![Exec Summary bottom](/images/execsummarybottom.PNG)

The third row of data related to the migration recommendations (6 R's) and wave planning details.  

This console is great for providing high level insights in to the migration process as your team is preparing for or executing a migration.  


### Insight Console

Let's go ahead and close this tab and go back to the Insight Console view.  This is a critical view for understanding the success and completeness of your scan jobs.  

![Console home](/images/consolehome.PNG)

If there is a need for remediation, such as credential issues, partially discovered servers or IPs that weren't in scope, we can identify and resolve as needed from this screen.  

In the Discovery Remediation summary, there are links to detailed views of each remediation need to make the resolutions easy to identify and take action against.  

In the Build Business Context section, you can see application level detail for what has been mapped versus what the system is suggesting or has found but not able to identify with confidence.  

In the Review and Enrich Services Data, this is where you can see a detailed view of the services identified and the associated statuses for the review, migration and other attributes. 

In the Explore Cyber Asset Inventory section, you can view detailed reports related to various IT Element inventories across various logical groups and categories.


### Migration Console

Let's move on from here to the Migration Console, by selecting the link at the top of the screen.  

![Migration Console home](/images/migconsolehome.PNG)

From this screen, you can see high level detail related to planning for a cloud migration, including links to an Economic Assessment Dashboard, as well as a Migration planning dashboard.

Below the row of charts, there is a detailed report at infrastructure and service level which can be exported as needed.  

Selecting the Migration Exclusion Dashboard will take you to a detailed report of any assets that have been excluded from the migration process.  This ensures that the migration planning dashboards include only the assets that are in scope for the migration and aren't cluttered with extraneous assets.

![Migration Exclusions](/images/migexclusions.PNG)

Selecting the Economic Assessment Dashboard will open a new tab with a wealth of financial data related to the cloud migration. This dashboard can help to understand the TCO and expected savings associated with the cloud migration.  The figures include "like for like" TCO estimates, as well as right-sized estimates, that represent what the reduced cost would be with appropriate resource sizing.  

There are also calculations related to the associated savings when opting for a 1 or 3 year reserved instance committment.  These costs can be toggled by AWS region by toggling the drop down on the left of this report.  

![Economic Assessment](/images/econassess.PNG)

Below the charts and cost estimates, there is a detailed report of the data dipicted above at a line item level as needed, such as the server recommendations

![Economic Assessment Detail](/images/econassessdetail.PNG)

Closing this tab and clicking on the Migration Planning Dashboard will open a new report with some of the data from the Executive Summmary, with some additions.

![Migration Planning](/images/migplan.PNG)

In the middle of the page, you can move between tabs including Service Details, Service Migration Process and PaaS Options.  

Each tab contains a unique data set related to the planning and execution of a migration.  


### Optimization Console



From the Discovery menu, navigate to the Scopes sub-menu

![Discovery Scopes](/images/discoveryscopes.PNG)

Click the blue plus sign in the upper right hand corner to start creating your new scope.

![Create Scope](/images/createscope.PNG)

Add a name and description to the Scope and select "Amazon EC2" as the Scope Type.

### Adding Targets to Scope

Click on your newly created scope to add the "Cloud Provider" subcription listed.  In the case of an on-premise deployment, we could instead add IPs, IP ranges, subnets, or hostnames to set the scan scope.  

![Add Scope](/images/addscope.PNG)

### Adding a Cloud Provider

This step has already been completed for you, but for future reference, a Cloud Provider account can be easily added to the CloudSphere platform.

In the Settings menu, there is a General sub-menu where you can add the Cloud Povider account.  

![Settings General](/images/settingsgeneral.PNG)

This account will require the standard AWS IAM ReadOnlyAccess permission level in order to access the environment.  

![Cloud Provider Settings](/images/cloudprovidersettings.PNG)

### Adding Exclusions

An exclusion is a scope (Target IPs) that you want to exclude or avoid scanning. By using this step, you can add a list of target IPs that you would like to avoid scanning. You can either choose an existing exclusion from the list which you have already created or create a new exclusion similar to creating a new scope. Exclusions are particularly useful when you are scanning a subnet of IPs, as one example.

We'll skip this step for today's exercise, so you have now completed the creation of a new Scan Scope, **nicely done!**


*Additional reference documentation related to scanning:*
*Scanning Best Practices: https://docs.cloudsphere.com/hc/en-us/articles/6259702566939-Scanning-Best-Practices*
*Identifying Network Segments for Discovery:https://docs.cloudsphere.com/hc/en-us/articles/5046106276635-Step-1-Identify-Network-Segments-for-Discovery* 


{{% notice info %}}
<p style='text-align: left;'>
**REMOVE:** With the exception of _index.md, the module folders and filenames should be changed to better reflect their content, i.e. 1_Planning as the folder and 11_HowToBegin as the first submodule. Changing the "weight" value of the header is ultimately what reflects the order the modules are presented.
</p>
{{% /notice %}}

#### Configuring the Scan Job
Now that we have a Scan Scope created, we can proceed with configuring the Scan Job
