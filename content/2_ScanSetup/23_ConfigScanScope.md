---
title: "Creating a Scan Scope" #
chapter: true
weight: 3 # MODIFY THIS VALUE TO REFLECT THE ORDERING OF THE MODULES
---

# Creating a Scan Scope
**CloudSphere CAM discovers devices that exist in your IT universe by executing Scan Jobs. The Scan jobs scan endpoints within a specified network boundary (Subnets, IP Ranges, IPs), which is defined using Scan Scope(s).**

*When configuring a Scan Job we first need to identify and define Scan Scope(s), and eventually add them to the job.*

*A Scan Scope provides a list of target IP addresses or hostnames that we want to be scanned while we execute a Scan Job. It also contains information about the Scope Type (target environment - Private Network, Amazon EC2, Azure, Google Cloud Platform).*

*This is automatic in the case of a Cloud deployment, but on-premise deployment scopes can be defined using the following:*
1. *List  - specified as a list of IP addresses or hostnames*
2. *IP Range - specified by a start and end IP address*
3. *IP Subnet - specified by a network address and subnet mask*


### Create a new Scan Scope

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
