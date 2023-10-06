---
title: "Registering the Virtual Appliance" # MODIFY THIS TITLE
chapter: true
weight: 1 # MODIFY THIS VALUE TO REFLECT THE ORDERING OF THE MODULES
---

# Registering the Virtual Appliance 

In order to scan an client environment, a virtual appliance must be deployed in the target network or segment.  We have already deployed the appliance in our AWS sandbox using our Amazon Machine Image (AMI file) available in the AMI directory.

### Capture Appliance ID

Since the virutal appliance is deployed, we now need to register the virtual appliance.  Navigate to the IP address provided in your access email (?) in your browser to log in to the virtual appliance, the default credentials are Username: admin Password: admin

Upon logging in to the appliance, the registration screen will be displayed.  Copy the unique Appliance ID to your clipboard.

![Appliance ID](/images/applianceid.png)

### Generate License Key

Navigate to the CloudSphere Platform at the address provided in your access email and enter the provided Organization to designate the proper tenant.  

![Org Selection](/images/orgselection.PNG)

On the next screen, you can complete the login process using the credentials provided in your access email.

![Credentials](/images/credentials.PNG)

Navigate to the Settings menu in the (bottom left) corner of the UI and click on the Appliances sub-menu.  

![Settings Appliances](/images/settingsappliances.PNG)

Click the Generate License button on the (top left center) of the UI to open the license creation window.

![License Creation](/images/licensecreation.PNG)

Paste the Appliance ID in the first field and name the appliance appropriately (suggested conventions?) then click the Create Appliance button to generate the License.  Copy this license to your clipboard with the icon in the lower right hand corner of the field.  


### Registering the Appliance

With the License copied from the last step, navigate back to the browser tab with the Virtual Appliance and paste the License in to the License Key field and click next. 

![Paste License](/images/pastelicense.PNG)

Select Finish on the next screen and the services running on the Virtual Appliance will restart to complete the registration process.

![Complete Registration](/images/completeregistration.PNG)

Navigate back to the CloudSphere Platform in the Appliances section to confirm the Appliance registration was successful.  

![Confirm Registration](/images/settingsappliances.PNG)

Congratulations! You have successfully installed and registered your CloudSphere Virtual Appliance.



**Additional details related to AWS appliance deployment and configuration available here:**

• *Instructions for AWS Appliance installation* - Appliance Installation - AWS https://docs.cloudsphere.com/hc/en-us/articles/5090846548123-Appliance-Installation-AWS

• *For Configuration use the following* - Configuring the Virtual Appliance https://docs.cloudsphere.com/hc/en-us/articles/5090275699995-Configure-the-Virtual-Appliance

**Additional details related to deployment in non-AWS environments available at the following links**

• *VMware*: https://docs.cloudsphere.com/hc/en-us/articles/5090855184539-Appliance-Installation-VMware

• *Hyper-V*: https://docs.cloudsphere.com/hc/en-us/articles/5090860657819-Appliance-Installation-Hyper-V

• *Azure*: https://docs.cloudsphere.com/hc/en-us/articles/5090858177307-Appliance-Installation-Azure-Marketplace-

• *GCP*: https://docs.cloudsphere.com/hc/en-us/articles/5090847564315-Appliance-Installation-GCP


{{% notice info %}}
<p style='text-align: left;'>
**REMOVE:** With the exception of _index.md, the module folders and filenames should be changed to better reflect their content, i.e. 1_Planning as the folder and 11_HowToBegin as the first submodule. Changing the "weight" value of the header is ultimately what reflects the order the modules are presented.
</p>
{{% /notice %}}

#### Configuring the Keychain 
Now that your Virtual Appliance is registered, we can proceed to Configuring the Keychain

