![Logo](logo.png) 
# RoyalePowerBI 

>This is a "Fan Content", provided as-is and free of charge, as per Supercell's "Fan Content Polcy". SuperCell is not responsible for or supported this material in any way.

## Objectives
This is intended for PowerBI Beginners willing to use the recently released (August 15th 2018) official Clash Royale® API (https://twitter.com/ClashRoyale/status/1029741854529658880).

It's a mini-tutorial with sample Power BI Report included.

This will be improved overtime, feedback and community improvements are welcome. This first release connects to a single data source, but it's easy to add data from other API endpoints provided by SuperCell®.

## Requirements
You'll need:
* **Power BI Desktop®**, provided by Microsoft for free: https://powerbi.microsoft.com/en-us/desktop/
    * Power BI Desktop® allows anyone to *create rich, interactive reports with visual analytics at your fingertips—for free*
* Account on **Clash Royale® Developer** website: https://developer.clashroyale.com
* Your **Player Tag** and/or **Clan Tag**
    * Player Tag is the code right below your Clash Royale alias in-game (see below)

    

## Instructions
1. Get your Acess _Token_ on Clashroyale developer website
    * Click here (https://developer.clashroyale.com) and register
    * Open the menu on top-right and go to "My Account"
    
    ![Step 1](/images/image1.JPG)
    * Click on "Create New Key"
    * Give it a name, short description and Allowed IPs
        * You may use Google to find your Public IP (https://www.google.com.br/search?q=myip)
     * Click "Create Key" and copy it, you will need it later to setup the connection
1. Get you **Player Tag** in-game, right below your alias

    ![Step 2](/images/image2.jpg)
1. Download the **Power BI** template file named _Royale-PowerBi.pbix_ and open it.
1. In Power BI Desktop click on **Edit Queries** button located in the Ribbon.
1. Select the **battlelog** query in the Query pane on the left and click on **Advanced Editor** in the ribbon.
1. Edit the second line of code replacing 
    * `<PLAYERTAG>` with your **Player Tag** you got from the game on step 2. Replace the **#** character for **%23**, so if your tag is **#1ABCDEF** then insert **%231ABCDEF**.
   * `<TOKEN>` for your token you got on step 1. It is a long string of characters. There should be a space between the word **Bearer** and your token.
1. Click **Done** and then **Close and Apply** in the Ribbon.
1. Your report should be ready, click **Refresh Now** to confirm you have the lastest data.
