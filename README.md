# WKS-WD
Instructions on how to export Watson Knowledge Studio Model to Watson Discovery Tooling for custom entity and relations extraction

# Deploy WKS Model and Use in Discovery 
**Prerequisites**


- You built your own WKS Model with tagged entities and/or relations. Example tutorial [here](https://www.ibm.com/cloud/garage/dte/tutorial/wks-tutorial).
## Export WKS Model 

1. In your Watson Knowledge Studio workspace, select Machine Learning Model > Versions page. 

2. Click on “create version.” Enter any meaningful description for the snapshot. Click **OK**.
3.  Click on “**deploy**” beside the version. Select the space or resource group where your Watson Discovery API was instantiated. 
    
![](https://paper-attachments.dropbox.com/s_30AFC27606A74D2BE8BFB6BE341402A28995DF729BBF0BE1EF5D8897ECAB4C92_1563852632516_Screen+Shot+2019-07-22+at+9.16.09+PM.png)

4. Copy and paste your **WKS Model ID** into a text editor after the model is finished deploying. 


## Configure WKS Model ID in Watson Discovery Tooling


1. Click on “catalog” in the navigation bar after signing into cloud.ibm.com

 2. Click on “AI” on the left hand menu and find “Discovery.” 
 3. Click on “create” and choose your plan (lite or paid). 
 4. Launch Watson Discovery tooling once API has been instantiated. 

![](https://paper-attachments.dropbox.com/s_30AFC27606A74D2BE8BFB6BE341402A28995DF729BBF0BE1EF5D8897ECAB4C92_1563853482892_Screen+Shot+2019-07-22+at+11.43.53+PM.png)


 
 5. Click on “upload your own data.” Name your collection. 

![](https://paper-attachments.dropbox.com/s_30AFC27606A74D2BE8BFB6BE341402A28995DF729BBF0BE1EF5D8897ECAB4C92_1563853781438_Screen+Shot+2019-07-22+at+11.47.28+PM.png)

6. Click on “configure data” on the right hand once the collection instantiating is complete. 
![](https://paper-attachments.dropbox.com/s_30AFC27606A74D2BE8BFB6BE341402A28995DF729BBF0BE1EF5D8897ECAB4C92_1563853893120_Screen+Shot+2019-07-22+at+11.48.11+PM.png)

7. Click on your new collection and navigate to the “enrich fields” tab. Click on “+ add enrichments.” 
![](https://paper-attachments.dropbox.com/s_30AFC27606A74D2BE8BFB6BE341402A28995DF729BBF0BE1EF5D8897ECAB4C92_1563853944284_Screen+Shot+2019-07-22+at+11.48.24+PM.png)

8. Select the Discovery feature tags you would like, and then navigate to the “entity” and “relation extraction” tiles where you will can enter your WKS Model ID. Click “add.” 
![](https://paper-attachments.dropbox.com/s_30AFC27606A74D2BE8BFB6BE341402A28995DF729BBF0BE1EF5D8897ECAB4C92_1563853988062_Screen+Shot+2019-07-22+at+11.48.45+PM.png)

9. Click on the name of your collection and upload documents. 

Done! Now you are able to query your entities and relations you created in your WKS model. 


