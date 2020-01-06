---
lab:
    title: 'Lab 03: Build a campaign'
    module: 'Module 6: Introduction to Dynamics 365 Marketing'
---

# MB-901: Dynamics 365 Fundamentals 
## Module 6, Lab 3 - Build a campaign

**Prerequisites:** Prior to performing the steps of this lab, perform the following tasks: 
1. Go to **Marketing** > **Files**
1. Click **New**
1. Click **Add files**
1. Uploads at least one image from your desktop.
1. Click **Upload**

**Optional:**  

1. In your Dynamics 365 instance, go to **Settings** > **Data Management**. 
1. Select **Sample Data**. 
1. If the sample data isn't installed, select **Install Sample Data**. The sample data might take a few minutes to appear, but you can continue to use the application while it's installed. 
1. Select **Close**. 

## Build a campaign

### Scenario

You need to create a customer journey that executes a one-time email blast.

### Instructions
1. Go to **Marketing** > **Customer Journeys**. This takes you to a list of existing customer journeys. Select **New** on the command bar.
1. The **New Customer Journey** page opens with the **Select a Customer Journey Template** dialog box shown. Select **Blank template**, and then choose **Select**. The dialog box closes, and your selected template is copied to your new journey.
1. Now you are looking at the customer journey designer, where you will assemble a pipeline that defines each step of the journey. Like all journeys, this one starts with the participants, who in this case are the people you specify as part of a market segment. Drag a **Segment Group** tile from the **Toolbox** tab onto the first position of the pipeline.
1. Select the expand button at the lower-right corner of your new **Segment Group** tile to view the member segments of this group. Right now, there's just one, so select it.
1. With the nested segment still selected, open the **Properties** tab to the right of the canvas. The **Properties** tab provides settings that apply to the selected tile. Set the **Segment** to the name of the segment that you want to target with your campaign.
1. Go back to the **Toolbox** tab and drag an **Marketing email message** tile to the space immediately to the right of the **Segment Group** tile.
1. With the new **Email** tile still selected, open the **Properties** tab again. Set the **Marketing Email Message** to the name of the message that you created earlier in the Create engaging emails section of this lab.  
1. Until now, you've been working on the **Designer** tab. Now go to the **General** tab, where you can name your journey and configure its run schedule. Make the following settings here:
 - **Name:** Enter a name for the customer journey that you can easily recognize later. This name is internal-only.
 - **Start Date Time:** Enter the time when the journey should begin processing contacts. When you select the field, a suggested default time is provided.
 - **End Date Time:** Enter the time at which the journey should stop processing contacts. All actions will stop at this time, even if some contacts are still in the middle of the journey. If you're just testing, allow a couple of weeks.
 - **Time Zone:** Select your local time zone (if needed). The other dates and times on the page will be displayed relative to this zone. 
 - **Content Settings:** This should already be set to the default content settings record set for your instance. 
1. On the command bar, select **Save** to save the work you've done so far.
1. To make sure your journey includes all required content and settings, select **Check for Errors** in the command bar. **Dynamics 365 Marketing** checks it and then displays results. If errors were found, you'll see a message at the top of the window and various indicators to show where the problems are. For example, if one of your tiles is misconfigured, you'll see an error count above the relevant tile, and you can read details about the error by selecting the tile and opening its Properties tab.

If you followed this procedure and your email message is live, your journey should pass the error check. If it doesn't, read the error message, fix the reported issue, and try again until it passes.
1. Your journey is now ready to go. To start it running, publish it by selecting **Go Live** on the command bar.

Dynamics 365 Marketing copies the journey to its email marketing service, which executes the journey by processing contacts, performing actions, and collecting results during the time it is set to run. The journey's **Status Reason** is updated to Live.
1. It might take several minutes for your messages to get sent, so allow some time for them to arrive in your inbox. After they do, open them and load the images. Then you can go back to Dynamics 365 Marketing and see how your journey is going. The **Designer** tab now shows information and results for each tile from your pipeline. Open the **Insights** tab to see detailed analytics.
