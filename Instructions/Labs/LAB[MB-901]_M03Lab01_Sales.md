---
lab:
    title: 'Lab 01: Explore Dynamics 365 Sales'
    module: 'Module 03: Introduction to Dynamics 365 Sales'
---

# MB-901: Dynamics 365 Sales
## Module 3, Lab 1 – Explore Dynamics 365 Sales

**Prerequisites:** Prior to performing the steps of this lab, perform the following tasks:

1. Create and save a word document with a sample text such as “Guide To Dynamics 365 Sales” in your desktop.
1. Enable **Enhance Email** experience from Sales Hub App Settings. This feature enables the email compose window to open in a pop-up window when a you create a new email from the **Timeline** section.
1. Refresh your browser.

**Optional:**
 
1. In your Dynamics 365 instance, go to Settings > Data Management.
1. Select Sample Data.
1. If the sample data isn't installed, select **Install Sample Data**. The sample data might take a few minutes to appear, but you can continue to use the application while it's installed.
1. Select **Close**.

### Create new contact

1. In the **Dynamics 365 Sales Hub**, navigate to **Customers** > **Contacts**.
1. Click **New**.
1. In the **First Name** field, type **Cameron**.
1. In the **Last Name** field, type **Azadi**.
1. In the **Job Title** field, type **Xbox X-Series Development Manager**.
1. In the **Business Phone** field, type **949-555-1212**.
1. In the **Address 1: Street 1** field, type **1 Microsoft Way**.
1. In the **Address 1: City** field, type **Redmond**.
    - **Note:** if demo data has been uploaded the **Address Suggestions** form will appear. Click **OK**. It will auto populate the **Address 1** fields. 
1. In the **Address 1: Sate/Province** field, type **WA**.
1. In the **Address 1: ZIP/Postal Code** field, type **98007**.
1. In the **Address 1: Country/Region** field, type **United States**.
1. In the **Email** field, type your email alias.
1. Click **Save**.

### Create new lead

1. In the **Dynamics 365 Sales Hub**, navigate to **Sales** > **Leads**
1. Click **New**
1. Click the **Qualify stage** icon.
1. In the **Existing Contact?**  field, select or type **Cameron Azadi**.
- **Note:** Selecting an existing contact while creating a lead record, automatically populates First Name, Last Name, Job Title, Business Phone, Mobile Phone, and Email in the Lead form. Selecting an existing Account, will auto populate the company name in the lead form. This makes it really quick and easy to enter a lead record.
1. In the **Topic** field, type **Likes our Xbox products**.
1. Click **Save**.

### Change system settings

1. Navigate to the **Settings** gear icon in the upper right menu. Use the dropdown to choose **Advanced Settings**.
1. Click the dropdown next to **Settings** and navigate to **Administration** under **System Settings.**
1. Select **Sales** tab.
1. In the **Qualify lead experience** field, select **No**.
1. Click **OK**.

### Qualify the new lead

1. In the **Dynamics 365 Sales Hub**, navigate to **Sales** > **Leads**.
1. Select **Cameron Azadi**.
1. Click **Qualify** button.
1. In the **Qualify Lead** form, click **Contact**. This will change the value from **Yes** to **No**.
1. In the **Qualify Lead** form, click **Opportunity**. This will change the value from **No** to **Yes**.
1. In the **Qualify Lead** form, click **OK**. 
**Note:** The lead will progress to Develop stage.

### Add notes to the new lead

1. In the **Timeline** section, click **+** to add a new **Note**.
1. In the **Title** field, type **Meeting with Cameron regarding the Xbox X-Series**.
1. Click **Add note**.
1. In the **Timeline** section, click **+** to add another **Note** with attachment.
1. In the **Title** field, type **Xbox X-Series product information**.
1. Click the attachment icon and select the word document you have created at the beginning of this lab.
1. Click **Add note**.

### Verify the notes created in the lead from Opportunities

1. In the **Dynamics 365 Sales Hub**, navigate to **Sales** > **Opportunities**.
1. Switch the view by clicking the dropdown menu and selecting **All Opportunities**.
1. Click to select the opportunity **Likes our Xbox products for Cameron Azadi**.
1. Note that the attachment and notes created in the lead form is also available in the opportunity form. 
1. In the **Timeline** section, click **+** to draft and send an **Email**. The email pop-up will appear.
1. In the **Subject** field, type **Xbox X-Series**.
1. Type a message such as “Hi Cameron, thank you for your interest in Xbox X-Series. We look forward to our meeting.” 
1. Optionally, from either the opportunity record or the related records such as contact record by navigating to it, in the background, you can copy and paste any information to the email message without losing the focus and save time.
1. Click **Save**.




