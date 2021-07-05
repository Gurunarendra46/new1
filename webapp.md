# Creating a Web App
<hr>

<b>Step 1:</b> Select Hosting Platefrom - ["Azure Web Apps", "Azure Cloud Services", "Azure VM"]

Choosing a Hosting Platform

Choice - Azure Web Apps

Reasons for choosing Azure Web Apps
<ul>
  <li>Global Scale with High Availability</li>
  <li>Multiple Languages and Frameworks</li>
  <li>Visual Studio Integration</li>
  <li>Security and compliance</li>
 </ul>
 
 Steps below are for creating web app in azure portal
 
 <hr>
 
<b>Step 2:</b>Create a web app in azure

1. For creating web app login to Azure Portal.

2. Select create a resouce and from the marketplace select Web App.

3. Fill in all the basic details
<ul>
  <li>Subsciption</li>
  <li>Resouce Group</li>
  <li>Name- should be unique and it contins the extension .azurewebsites.net</li>
</ul>
<img src="images/basic.png">


4. Review and create your web app.


<img src="images/webapp.png">


<h2>Deploying ASP.Net Core App to WebApp</h2>

We can directly deploy an application without going to the Azure portal.
1. Create a new Asp.Net Core application in Visual Studio.
2. Right click on the project file and select publish.
3. In Publish target window Select ‘Create New’ option and click on Publish button.
4. In Create App Service dialogue box, fill in the Azure Subscription.
<img src="images/vs1.png">

The Visual studio start creating the web app in Azure and deploys the application.

<img src="images/vs2.png">

After you can deploy the web app in the browser.

<img src="images/deployment.png">

<h2>Scaling Apps</h2>

Scaling your app by increasing/decreasing the capability of the resource, in terms of going to higher/lower tier by opting for more/less cores, RAM, and Storage depending on your requirement, this is known as Vertical Scaling.

Scaling your app by increasing/decreasing the number of instances of your server with the same cores, RAM and storage to handle the traffic depending on your requirement, this is known as Horizontal Scaling.

<img src="images/scaling.png">

<h2>App Security</h2>

App Service lets you secure your apps with HTTPS. When your app is created, its default domain name (<app_name>.azurewebsites.net) is already accessible using HTTPS. If you configure a custom domain for your app, you should also secure it with a TLS/SSL certificate so that client browsers can make secured HTTPS connections to your custom domain.

<img src="images/security.png">

<h2>App Monitoring</h2>

Metrics are measures of a resource’s certain characteristics over a given period. For instance, CPU utilization, disk IOPS, number of connections, etc. 
These are typically real-time, and since they are stored as values with a standard collection interval, they are ideally suitable for viewing as graphs to 
help you view results over time.

<img src="images/monitor.png">


Logs contain time-stamped information about changes made to resources. The type of information recorded varies by log source. The log data is organized into records, with different sets of properties for each type of record. The logs can include numeric values such as Azure Monitor metrics, but most include text data rather than numeric values.

<img src="images/logs.png">
