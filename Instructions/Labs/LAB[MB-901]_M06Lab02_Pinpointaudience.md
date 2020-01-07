---
lab:
    title: 'Lab 02: Pinpoint your audience'
    module: 'Module 06: Introduction to Dynamics 365 Marketing'
---

# MB-901: Dynamics 365 Fundamentals 
## Module 6, Lab 2 - Pinpoint your audience

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

**Scenario:** You need to set up a collection of segments, which you'll define by using terms that resemble those you already use to describe groups of customers. 
Then you'll use these segments to target marketing initiatives like email-marketing campaigns and customer journeys. Segments like these, which you define by using a set of rules and conditions, are called dynamic segments because membership in these segments changes constantly and automatically based on information in your database. Note: Static segments are populated by adding contacts explicitly, one at a time.

## Instructions

1. Go to **Marketing** > **Contacts**. This takes you to a list of existing contacts. On the command bar, select **New**.
1. The **New Contact** page opens. Fill out the following fields:
 - **First Name:** Enter a fictional first name.
 - **Last Name:** Enter a fictional last name.
 - **Email:** Enter your own email address (or one that you can receive mail from).
 - **Address 1: City:** Enter a fictional city (for this example, we use **Atlantis**). This will make it easy to create a segment that only includes fictional contacts. 

1. On the command bar, select **Save & Close**.
1. Create a second contact similar to the one you just made. Use a different email address and fictional city, but use a different first and last name   .
1. On the command bar, select **Save & Close**.
1. Go to **Marketing** > **Segments**. This takes you to a list of existing segments. On the command bar, select **New**.
1. A pop-up screen will appear, where you can select a segment template. Click **Cancel**.
1. The **New Segment** page opens   . It shows a selection of segment types. We're going to base this segment on properties of contact records alone, so select **Demographic** to create a demographic segment.

1. **Dynamics 365 Marketing** creates a demographic segment, which already includes a query against the contact entity. You can see the **Contact** entity being queried by checking the value shown on the drop-down list at the top of the query block.

1. Your segment currently includes no filters (clause rows), which means it will find all the contacts in your database. But we only want to find the new test contacts that we just created, so let's add a filter..
1. The **Select attribute** field to open a drop-down list that shows all attributes available on the contact entity. Then type "city" to filter the list and choose **Address 1: City** from the list.

1. Two new drop-down lists are now added to the row. Leave the next drop-down list set to **Equals**. This is the operator, which defines the way we are going test values in the **Address 1: City** field of the **Contact** entity. Other operators include **Contains**, **Begins with**, **Contains data**, and more, depending on which type of value (string, number, date, and so on) you are working with.
1. Select the third drop-down list, which contains the ghost text **Enter text** and type the fictional city name that you chose for your test contacts (such as "Atlantis" if that's what you chose).
1. Select the field at the top of the query, which contains the ghost test **Enter segment name** and enter a name for your segment (such as "Contacts from Atlantis").
1. Select **Save** on the command bar to save your segment and then select Go Live to publish the segment (you won't be able to use it in a customer journey until it goes live, even though you've saved it). Dynamics 365 Marketing checks the segment for errors and reports any problems it finds. If an error is reported, fix it and try again. If no error is found, your segment is copied to the marketing services, which make it available for use by a customer journey.

1. Wait for about a minute and then select **Refresh** on the command bar to refresh the page. You should now see that a **Members** tab has been added (if you don't see it, wait a little longer and try to **Refresh** again until you do). When the **Members** tab appears, open it and note that your segment includes the two fictional contacts that you added earlier.
