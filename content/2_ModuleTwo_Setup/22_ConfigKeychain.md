---
title: "Configuring the Keychain" # MODIFY THIS TITLE
chapter: true
weight: 2 # MODIFY THIS VALUE TO REFLECT THE ORDERING OF THE MODULES
---

<!-- MORE SUBMODULES CAN BE ADDED TO DIVIDE UP THE SETUP INTO SMALLER SECTIONS -->
<!-- COPY AND PASTE THIS SUBMODULE FILE, RENAME, AND CHANGE THE CONTENTS AS NECESSARY -->


# Configuring the Keychain

<ul> In order to get accurate and detailed information about servers and services, the Application Discovery requires server Credentials to access information. Keychains are lists of Credentials. <ul/>

### Create a new Keychain 
First, we'll need to create a new Keychain.  Navigate to the Discovery menu on the (left nav bar) and select the sub-menu item title Keychains.  

Click the blue plus sign button in the upper right hand corner to start the Keychain creation process.

Select Cloud as the Keychain Location, name the Keychain and add a brief description.  

Note: Keychains and associated credentials can be stored on the cloud or locally on the appliance as needed.  Cloud Keychains are more easily modified and can be updated simply via the CloudSphere UI.  Locally stored credentials must be modified on the Virutal Appliance as needed.  

### Add Credentials

Click on your newly created Keychain and click the blue button titled Add Credential in the upper left corner of this screen.  

Review the access email for the credentials provided and enter each of the credentials individually to add them to your Keychain.

You will also have the option to test the credentials that you just entered, which is helpful to make sure there are sufficient privledges.

Once all of the credentials have been added to the Keychain, you have completed the configuration of your Keychain.  Well done!

{{% notice info %}}
<p style='text-align: left;'>
**REMOVE:** With the exception of _index.md, the module folders and filenames should be changed to better reflect their content, i.e. 1_Planning as the folder and 11_HowToBegin as the first submodule. Changing the "weight" value of the header is ultimately what reflects the order the modules are presented.
</p>
{{% /notice %}}

#### Creating a Scan Scope
Now that we have our Keychain configured, we can move on to creating the Scan Scope

