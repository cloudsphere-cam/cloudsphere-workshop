---
title: "Using the Explorer UI" # MODIFY THIS TITLE
chapter: true
weight: 1 # MODIFY THIS VALUE TO REFLECT THE ORDERING OF THE MODULES
---

# Using the Explorer UI

**In this section, we'll take a look at the Explorer UI functionality and review sections including the IT Universe, Servers and Applications**

### Explorer UI

Upon logging in to the CloudSphere tenant using the credentials provided in your workshop welcome email, you will be taken to screen within the Explorer UI section called the IT Universe.

![IT Universe](/images/ituniverse.PNG)

The IT Universe provides a high level summary of the environment(s) that have been scanned by the platform.  You'll see logical groups across environment types, including Development, Testing, Staging and Production.  Within those groups, there will be additional detail related to the services, applications, containers and servers within each enviroment.

Clicking on any of the circular quandrants, takes you to a visualization of the individual services, with lines between services where there are communication or infrastructure dependencies.  

![Quadrant](/images/quadrant.PNG)

Clicking on any of the services will take you to a view that highlights the underlying infrastucture supporting that service.  Hovering over each of the blue dots will highlight the specific underlying applications.

![Quadrant Service](/images/quadrantsvc.PNG)


### Explorer Servers

If you select the sub-menu titled Server in the left navigational bar, you will be presented with a list of all servers that we captured as part of the scanning.  

![Server menu](/images/servermenu.PNG)

Pressing the plus sign to the right of the Servers sub-menu will provide you with an expanded list of addtional, logical sub-categories for ease of review.  

![Server plus](/images/serverplus.PNG)

You'll see grouping related to OS, environment type and status.  Choose a sub-category and see the specific list of servers associated with your selection.

From any of the list views, you can double click any of the rows to get extremely granular insight related to that server.  

![Server detail](/images/serverdetail.PNG)

From this detailed view, you can navigate across the various header tabs to get different insights related to the server you've selected.

The overview tab provides all of the high level details related to the server, inclyding IP, location, manufacturer, OS, specs and more.  

Navigating to the Dependencies tab will provide you with an interactive visualization of that server, including the applications it's running and any related services it is supporting.  

![Server dependencies](/images/serverdep.PNG)

Navigating to the Communication tab will provide you with a detailed communications map, which also highlights any other resources with shared communications. 

![Server communication](/images/servercomm.PNG)

Navigating to the Metrics tab will provided you with detailed charts related to telemetry data for the server you are reviewing.  These data points are also collected for the TCO and Right-sizing data that we'll see later in the Insights Consoles.

![Server metrics](/images/servermetrics.PNG)

There are even more tabs available, so feel free to explore all of the tabs to see the level of detail provided for each server in the environment.  

### Explorer Applications

Similar to the Servers view, there is an expanded view of all Applications scanned in the enviroment as well.

![Explorer Applications](/images/explorerapps.PNG)

Much like with the servers, you will see applications grouped as a whole, as well as logical sub-categories by toggling the plus sign to the right of the sub-menu. 

![Application Groups](/images/appgroups.PNG)

Furthermore, double-clicking any of the applications listed will take you to an expanded view with multiple view tabs, inlcuding the communication and dependency mapping.    

![Application detail](/images/appdetail.PNG)

You'll find an icon in the lower left of the screen that looks like a large gear next to two smaller ones.  If you click that icon and check the box labeled Extended View, you'll be able to see any additional applications tied to the underlying infrastructure, as well as possible hidden communication or dependencies assocaited with the application inspecting.


{{% notice info %}}
<p style='text-align: left;'>
**REMOVE:** With the exception of _index.md, the module folders and filenames should be changed to better reflect their content, i.e. 1_Planning as the folder and 11_HowToBegin as the first submodule. Changing the "weight" value of the header is ultimately what reflects the order the modules are presented.
</p>
{{% /notice %}}

#### Exploring Services
Now that your understand how to use the Explorer UI to review the IT Universe, Servers and Applications, we'll take an in-depth look at Services

