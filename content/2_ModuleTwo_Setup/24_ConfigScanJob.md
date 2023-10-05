---
title: "Configuring the Scan Job" # MODIFY THIS TITLE
chapter: true
weight: 4 # MODIFY THIS VALUE TO REFLECT THE ORDERING OF THE MODULES
---

<!-- MORE SUBMODULES CAN BE ADDED TO DIVIDE UP THE SETUP INTO SMALLER SECTIONS -->
<!-- COPY AND PASTE THIS SUBMODULE FILE, RENAME, AND CHANGE THE CONTENTS AS NECESSARY -->

# Configuring the Scan Job
Now that we have our Keychain and Scope configured, we can configure our Scan Job

### Create New Scan Job
Navigate to the Discovery menu in the left nav and click on the sub-menu titled Scan Jobs.

In the upper right hand corner, click the blue plus sign.

Add a name to the job and a description as desired and click the button titled Create New Scan Job

### Select Scan Job Type

Confirm the type is set to "Sequential"

### Set the Scan Details

Select the Appliance that you previously registered in the first drop down box

The location field can be selected, but is optional

The Enablings field configures additional details related to the scanning job, including the ability to collect basic performance metrics on each endpoint.  For now, we'll leave this blank, but in live deployments where telemetry data is desired, we'd enable the ServerMetrics option.  This option deploys a lightweight script on each endpoint that reads existing data sources, such as perfmon 

Leave the Maximum duration set to 2 (hours) for now.  This can be used to (minimize the chances a unsuccessful scan job will run before timing out?)

Click the Update button in the upper right hand corner to save the changes

### Add the Scope

Select the previously created scope to add it to this scan job.  Note: you can only add one Scope per Scan Job; if you wish to have multiple Scopes, you will also need multiple Scan Jobs.  

Click the Update button in the upper right hand corner to save the changes

### Add Exclusions (optional)

We won't add any exclusions today, but this is where exclusions to the Scan Job can be added to further refine the scope to omit any endpoints specified.  An exclusion is set up as a Scope, as noted in the previous section.

### Add Keychain(s)

Select the previously created Keychain to add it to the Scan Scope.  Note: you can have multiple Keychains associated with a Scan Job, so if there is a need or desire to separate credentials in to multiple Keychains, this can be accomodated for.

Click the Update button in the upper right hand corner to save the changes

### Add Scheduling (optional)

After an initial scan is completed, it's common for clients to set up a periodic scan of their enviroment to capture changes in communications and performance over a given time period.  

For now, we'll leave this set to the defaul of "Don't schedule scan job", but you'll see that clicking on the "Schedule scan job" option allows you to set the scan frequency.

This is generally set to run daily, but can be run more frequently as appropriate.  Note: If scheduling is enabled, the frequency must be greater than the Maximum duration set in the Scan Details section.

Note: If the ServerMetrics script is enabled, the metrics will be captured every 5 minutes and reported to the system upon each subsequent scan, so there isn't a need to scan multiple times a day to account for variations in utilization.  


{{% notice info %}}
<p style='text-align: left;'>
**REMOVE:** With the exception of _index.md, the module folders and filenames should be changed to better reflect their content, i.e. 1_Planning as the folder and 11_HowToBegin as the first submodule. Changing the "weight" value of the header is ultimately what reflects the order the modules are presented.
</p>
{{% /notice %}}

#### Start Scan Job <!-- MODIFY THIS HEADING -->
Now that your Scan Job is configured, it's time to get the scan running
