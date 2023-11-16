---
title: "Data Review" # 
chapter: true
weight: 3 # 
---

# Reviewing your AWS Cloud Quick Assessment Results

**Now that your accounts are scanned, let's review the results**

### Data Review

Following completion of the Cloud Job(s), the output will be available to you in two primary sections of the platform, Inventory and Insight Consoles.

The Inventory section of the platform will highlight your entire AWS inventory in logical categories including Compute, Network, Storage, Database, etc.  

![Inventory main](/images/invmain.PNG)

To view the details, just click on a category of interest and you will be taken to an expanded, subcategorical view of the inventory.  

![Inventory category](/images/invcat.PNG)

Double click on any line item to see expanded details about that service/resource, including mapping to other services/resources

![Explorer details](/images/expdetails.PNG)

Select the Configuration tab to see more granular detail related to the service/resource in question.  

For actionable insights, let's navigate to the Insight Consoles to learn more about the opportunites for enhancing your Cloud accounts.  

![Opt Console main](/images/optconsolemain.PNG)

You'll see your are presented with four categories of optimization opportunities, relcamation, rightsizing, modernization and performance.  Each category has high level savings estimates, along with with additional detailed dashboards and reports on each category shown on this screen. 

First, let's take a look at the Reclamation dashboard

![Reclamation Dashboard](/images/recdash.PNG)

Within this dashboard, there are numerous reclamation opportunities identified across various service categories:
1. **Cloud Instances (EC2):** Identify idle or stopped EC2 instances.
2. **Storage Volumes (EBS):** Discovery unattached or idle EBS volumes.
3. **Database Instances (RDS):** Identify idle or stopped RDS instances.
4. **Load Balancers (ELB)):** Detect load balancers that are idle, have no active targets or no healthy targets.
5. **IP Addresses (EIP)):** Locate Elastic IP Addresses that are not attached to an EC2 Instance or are attached to a non active EC2 instance.  

![Reclamation Dashboard Details](/images/recdashdetails.PNG)

The savings associated with each category is highlighted and the dashboards are highly interactive so you can drill down to whatever level of granularity needed to make the savings recommendations easily actionable.  

Next up, we'll review the Rightsizing Dashboard and the insights it helps to unlock

![Rightsizing Dashboard](/images/rsizedash.PNG)

With this dashboard, we can see opportunites for cost savings through rightsizing of EC2 and EBS resources.  Again, you can use the interactive charts to segment the data to aid in the savings opportunity exploration and execution.  

![Rightsizing Dashboard Details](/images/rsizedashdetails.PNG)

In addition to identifying over-provisioned resources that present savings opportunities, the platform will also provide suggestions related to under-provisioned resources that could benefit from an upgrade in performance.  These recommendations will ensure your resources are appropriately balancing cost and performance as needs change over time.  


Next, we have our Modernization Dashboard, which captures savings opportunities across four possible categories including: 

1. **Windows License Optimization:** Identify instances which are candidates to move from Windows to Linux operating systems saving on Windows OS license costs.
2. **MS SQL License Optimization:** Discover MS SQL Servers running on Windows which may be migrated to Linux based instances freeing the Windows OS license costs
3. **Cloud Instance Generation Modernization (EC2):** AWS recommends running EC2 instances on the latest generation of instance types as you will get the best performance typically at a lower cost.
4. **Storage Volume Type Modernization (EBS):** Similar to instances, it is recommended to store your data on the latest genreation of EBS volumes again gaining performance benefits without increasing costs.

![Modernization Dashboard](/images/moderndash.PNG)

Each category has a corresponding dashboard with pointed insights that can be quickly translated in to savings.  

![Modernization Dashboard SQL](/images/moderndashsql.PNG)

Finally, there is the Performance Dashboard, with pointed insights to ensure your cloud services are running at optimal performance.  

![Performance Dashboard](/images/perfdash.PNG)

Insights include:

1. **Cloud Instances (EC2):** Removing unused security group rules from the security group of a running instance can improvoe overall performance.
2. **Storage Volumes (EBS):** Using high IOPS volumes with an instance that is not EBS Optimized will result in less than desired performance while still incurring the higher cost of the storage.
3. **Security Groups:** Like with running instances, it is good practice to ensure your security groups do not contain a high number of rules which can lower the performance of your system.

![Performance Dashboard](/images/perfdash2.PNG)


#### There you have it.  In a matter of minutes, you can scan your AWS accounts and get immediate insights that are actionable for enhancing your performance and reducing your cloud spend.


