# 🤝HIRE US FOR FULL INSTALLATION🤝

Contact Info: archan.fiem.it@gmail.com, hk.sainaga@gmail.com

# EDR Installation Guide:
  - Now we’re ready to install Elastic EDR First, navigate to the “Fleet” dashboard by clicking on the link under the management tab located on the side menu.

![image](https://user-images.githubusercontent.com/51078911/159172623-c1e1bb4c-c231-4591-b4e0-7b1e8a6d1c8c.png)


  - From the fleet management menu, click “add agent”. Now it’s likely that you’ll be requested to add an integration policy before you can install agents, just follow the wizard and keep the defaults.
  
![image](https://user-images.githubusercontent.com/51078911/159172645-2c5f730b-95d9-47ec-b566-f8c414d7793b.png)

  - We’re going to use the “Enroll in Fleet” option to install the EDR.

![image](https://user-images.githubusercontent.com/51078911/159172653-65e6412f-c8d6-413d-8e93-5d1b4e29b95c.png)

  - First, download the Elastic Agent onto your Windows/Linux Host.
  - Once you have the agent downloaded, keep the default policy selected under the Agent policy.
  - Now we have to Add Agent. Click on the Button and follow the steps from console.

![image](https://user-images.githubusercontent.com/51078911/159172662-d550ae75-d938-4ebe-aaa1-89bfa46f98da.png)

  - If all has gone right, you should see the agent has been successfully enrolled via the fleet dashboard.

![image](https://user-images.githubusercontent.com/51078911/159172667-d66ba884-4a7c-4570-b692-3de4db42e2d2.png)

  - We’re not done yet however, we need to check that data is being ingested correctly into ElasticSearch from our agent. You can do this by navigating to the Data Streams tab. You should see this populated with endpoint data. If there is no data here, check your fleet settings by clicking the settings cog in the top right corner. Ensure that your ElasticSearch settings are properly set to the correct IP and not set to LocalHost.

![image](https://user-images.githubusercontent.com/51078911/159172678-1ddbf98c-adcf-472c-b3ba-e45696cea990.png)
