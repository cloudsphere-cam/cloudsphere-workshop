---
title: "Services Explorer" # MODIFY THIS TITLE
chapter: true
weight: 2 # MODIFY THIS VALUE TO REFLECT THE ORDERING OF THE MODULES
---

# Using the Exporer UI to Examine Services

**Now that you understand how to use the Explorer UI, we'll look at some more in-depth exploration of Services**

### What is a service

Before we get in to reviewing services, we first want to define how CloudSphere views services as part of our platform.  

Services in our tool refers to a group of applications and their underlying infrastructure that collectively combine to provide a given service within a business.  Basic examples include a CRM, HR system, ELK stack or online shop.  Each of these services is comprised of a series of applications and the supporting infrastructure.  

When moving a business service to the cloud, it's imperative that you understand all facets of the service including the supporting applicaitons and infrastructure, but also the underlying communication and dependencies of that application.  It's very common for applications or services to run on shared resources, which could create business risk if not fully documented.  
   

###Services Explorer Home

Selecting the Services sub-menu in the left nav menu will bring you to the Services home view.  From here, you will find a detailed listing of each service identified as part of the scanning.

![Services Home](/images/serviceshome.PNG)

Each service will have a number of data points, both user generated and system assigned, for ease of review.  Users can assign custom tags to each service, as well as the details related review status, importance, label and more.  

To manually update the fields on a given service, double click the name of the service and navigate to the Overview tab at the top of the page.

![Services Overview](/images/servicesoverview.PNG)

Click the edit button and you'll be taken to a screen that allows you to edit details like the name and label.  There are also dropdowns for details such as importance, review and wave value.  While the system will assign a wave value, you do have the option to designate an alternative wave as appropriate.  

![Services Edit](/images/servicesedit.PNG)

Similar to the Explorer view of servers and applications, the services detail includes various details tabs including the metrics, resources, dependencies and communication.  

![Services Dependencies](/images/servicesdep.PNG)

Again, you can use the gear icon to show extended views in the communication and depencies tabs, to help uncover hidden relationships to minimize risk during a cloud migration. 

![Services Dependencies Extended](/images/servicesdepex.PNG)

Moving back to the main services page, we can see the start of our migration planning already coming together.  We are starting to see the various wave groupings associated with each service and can start develop our migration waves with minimal risk.  

![Services Home](/images/serviceshome.PNG)

Let's go ahead and pick a service to explore further and talk about how we'd start planning on moving that service.  There is a service called Data_Logistics_Platform that has a wave 1 value assigned to it and is flagged as approved.  

![Data Logistics](/images/datalogistics.PNG)

Double clicking on this service and navigating to the Dependencies tab shows us this service is comprised of two applications on a single virtual machine.  

![Data Logistics Dep](/images/datalogisticsdep.PNG)

Taking a look at another service, like our Elastic ELK Stack, shows an entirely different type of service.  This example highlights the combination of ElasticSearch, LogStash and Kibana that make up the ELK stack, as well as the five VMs supporting those applications. 

![ELK Stack](/images/elkstack.PNG)

Selecting the Extended View in the Dependencies tab uncovers a hidden connection to our demo service application, which would "break" if we attempted to move the ELK Stack alone.  

![ELK Stack Dep](/images/elkstackdep.PNG)

Similar levels of complexity are uncovered in the Extended View of the Communication tab as well.  This shows us that we need to approach this service with caution to minimize risk during a migration and is the primary reason this is designated as a Wave 3 service.  

![ELK Stack Comm](/images/elkstackcomm.PNG)

When prioritizing wave planning, starting with the more simple and isolated services is generally where most companies will start.  Simple lift and shift (also known as rehosting) or replatforming are generally easy wins that companies can use to start their cloud migration journey.  Once there is a certain level of comfortability with basic service migration, moving more complex services become easier over time.

![Services Home Sorted by Wave](/images/serviceshomesorted.PNG)


{{% notice info %}}
<p style='text-align: left;'>
**REMOVE:** With the exception of _index.md, the module folders and filenames should be changed to better reflect their content, i.e. 1_Planning as the folder and 11_HowToBegin as the first submodule. Changing the "weight" value of the header is ultimately what reflects the order the modules are presented.
</p>
{{% /notice %}}

#### Insight Consoles
Keep these examples in mind as we move to the next section, where we'll examine these services and more in the Insight Consoles

