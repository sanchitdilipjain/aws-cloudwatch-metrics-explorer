## AWS Cloudwatch Metrics Explorer

**Introduction**

- Metrics Explorer is a tag-based tool that allows the filter, aggregate, and visualize the metrics by tags and resource properties to enrich observability for the services. 

- Metrics Explorer charts are dynamic, so if a matching resource is deployed after creating a metrics explorer widget and add it to a CloudWatch dashboard, the new resource automatically appears in the explorer widget

-  In this tutorial, we will focus on first creating a Metrics Explorer and then publishing it to a Dashboards

- **Step 1: Creating a Cloudwatch metrics explorer**

   1. Traverse to the <a href="https://console.aws.amazon.com/cloudwatch/">CloudWatch</a> click Explorer under Metrics
   
      <img src="images/image1.png" class="inline"/> 
   
      The screen should look similar to the screenshot shown below
      
      <img src="images/image2.png" class="inline"/> 
   
   2.  Metrics Explorer offers to pick from Generic Templates (Lambda and EC2) or Service Based Templates, where we can select the metric we want to add to a dashboard based on the service selected. Also, we can choose a custom time range to display the chosen metrics, or select the default range from 1h-1w
   
       <img src="images/image3.png" class="inline"/> 
   
   3.  Select on the drop-down which says Empty Explorer and select the lambda by runtime generic template
   
       <img src="images/image4.png" class="inline"/> 
   
   4.  Select ECS from the drop-down and provide 1w in the top right
   
   5.  Under the From the search bar, select All values( * ), then click Services.
   
       The screen should look similar to the screenshot below
       
       <img src="images/image5.png" class="inline"/> 

- **Step 2: Publishing to Dashboards**
   
   1. Select Add to Dashboard button in the top right corner  
   
   2. Click Create new, then enter ECS-demo-dashboard as the dashboard name and click Create dashboard
   
      <img src="images/image6.png" class="inline"/> 
       
      <img src="images/image7.png" class="inline"/> 
   
   3. Click the Explorer widget, then click create
   
      <img src="images/image8.png" class="inline"/> 
      
      <img src="images/image9.png" class="inline"/> 
   
   4. Along with simple simple dashboard publish, we can also perform complex operation like Replay Dashboard, Share Dashboard, etc.

      <img src="images/image10.png" class="inline"/> 
