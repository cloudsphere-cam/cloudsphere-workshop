---
title: "Configuring the Keychain" 
chapter: true
weight: 2 
---


# Configuring the Keychain

**In order to get accurate and detailed information about servers and services, the Application Discovery requires server Credentials to access information. Keychains are lists of Credentials.**

### Create a new Keychain 
First, we'll need to create a new Keychain.  Navigate to the Discovery menu on the (left nav bar) and select the sub-menu item title Keychains.  

![Discovery Keychains](/images/discoverykeychains.PNG)

Click the blue plus sign button in the upper right hand corner to start the Keychain creation process.

![Create Keychain](/images/createkeychain.PNG)

Select Cloud as the Keychain Location, name the Keychain and add a brief description.  

Note: Keychains and associated credentials can be stored on the cloud or locally on the appliance as needed.  Cloud Keychains are more easily modified and can be updated simply via the CloudSphere UI.  Locally stored credentials must be modified on the Virutal Appliance as needed.  

### Add Credentials

Click on your newly created Keychain and click the blue button titled Add Credential in the upper left corner of this screen.  

![Add Credentials](/images/addcredentials.PNG)

Review the access email for the credentials provided and enter each of the credentials individually to add them to your Keychain.

![Add Credential Details](/images/addcredentialsdetail.PNG)

You will also have the option to test the credentials that you just entered, which is helpful to make sure there are sufficient privledges.

![Test Credentials](/images/testcredentials.PNG)

Once all of the credentials have been added to the Keychain, you have completed the configuration of your Keychain.  **Well done!**

![Credentials Added](/images/credentialadded.PNG)


#### Creating a Scan Scope
Now that we have our Keychain configured, we can move on to creating the Scan Scope

