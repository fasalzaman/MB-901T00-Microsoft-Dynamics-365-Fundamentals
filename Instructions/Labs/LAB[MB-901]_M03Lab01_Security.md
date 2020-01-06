---
lab:
    title: 'Lab 01: Security'
    module: 'Module 03: Dynamics 365 security'
---

# MB-901: Dynamics 365 Fundamentals 
## Module 3, Lab 1 - Security


## Exercise 1: Explore security roles in Dynamics 365 model-driven applications

**Scenario:** As a system administrator, you need to find out what are the available out of the box security roles of Dynamics 365.

### Instructions:
1. In order to navigate to Dynamics 365 Settings dashboard, add the following: 

``
      ?settingsonly=true
`` 

at the end of the URL link of your Dynamics 365 business applications. The following example resembles a sample only and does not work if you navigate to it.

``
https://crmmYOURID.crm.dynamics.com/main.aspx?settingsonly=true
``

2. The **System** settings dashboard appears.
3. Use the **Dynamics 365** > **Settings** menu from the action pane to see the menu items. From the **System** group area, select **Security**
4. The **Securtity** dashboard appears. From the dashboard select **Security roles**. 
5. Here, you can see all of out of the box security roles in Dynamics 365.
6. Select **Sales Manager** role. Select **Core Records** tab. By using the **Security role** form, you can change security settings for this role in different functional areas.

## Lab 2: Explore security roles in Dynamics 365 Finance and Operations applications

**Scenario:** The HR department of USMF has requested to remove access to the Accounts receivable clerk role in Dynamics 365 Finance and Operations applications for an employee who has changed role. You, as a system administrator need to exclude Accounts receivable clerk role for the employee.

### Instructions:

1. Go to **System administration** > **Security** > **Assign users to roles**.
1. In the tree, select **'Accounts receivable clerk'**.
1. Click **Manually assign** / **exclude users**.
1. In the list, select a user.
1. Click **Exclude from role** to exclude the selected users from the role.
1. To remove exclusions, select the users that you want to remove exclusions for, and then click **Reset status**. 

**Scenario:** The HR department of USMF has requested having a rule for segregation of duties for **Access benefits workspace** as the first and **Approve production journal** as the second duty. You, as a system administrator need to create the rule.

### Instructions:

1. Go to **System administration** > **Security** > **Segregation of duties** > **Segregation of duties rules**.
1. Click **New**.
1. In the **Name** field, enter a name for the rule.
1. In the **First duty** field, click the drop-down button to open the lookup.
1. In the list, find and select the first duty that is controlled by the rule.
1. In the list, click the link in the selected row.
1. In the **Second duty** field, click the drop-down button to open the lookup.
1. In the list, find and select the second duty that is controlled by the rule.
1. In the list, click the link in the selected row.
1. In the **Severity** field, select the severity of the risk that occurs when the same user or role performs both duties.
1. In the **Security risk** field, enter a description of the security risk.
1. In the **Security mitigation** field, type a value.
1. Enter a description of the actions that you take to mitigate the security risk. 
For example, you can mitigate the risk by conducting more detailed reviews of the process, by conducting a monthly managerial review, or by sharing resources with other departments.
1. Click **Save**.

## Lab 3: Enhance security by encrypting your data

**Scenario:** You, as a system administrator need to change and copy the organization encryption key.

### Instructions:

1. Navigate to Power Platform Admin center ![https://admin.powerplatform.microsoft.com](https://admin.powerplatform.microsoft.com)  

1. These settings can be found in to **Environments** > [select an environment] > **Settings** > **Encryption** > **Data encryption**.
1. In the upper-right corner of the screen, select **Settings**  > **Personalization Settings**.
1. Scroll down to the very bottom of the **Set Personal Options** dialog box, and then choose **View your user information**.
1. Select the different areas such as **Summary**, **Details**, or **Administration** to see details about your profile.
1. Select an environment and go to **Settings** > **Encryption** > **Data encryption**.
1. In the **Change Encryption Key** box type the new encryption key and then select **Change**.
1. Select **OK** in the confirmation message and then select **Close** to exit the **Data Encryption** page.

We strongly recommend that you make a copy of your data encryption key.

1. Sign in with the **System Administrator** or **System Customizer** security role or equivalent permissions.
1. Select an environment and go to **Settings** > **Encryption**.
1. In the **Data Encryption** dialog box, select **Show Encryption Key**, in the **Current encryption key box** select the encryption key, and copy it to the clipboard.
1. Paste the encryption key into a text editor such as Notepad.

**Note:** By default, model-driven apps in Dynamics 365 generate a passphrase that is a random collection of Unicode characters. Therefore, you must save the system-generated passphrase by using an application and file that supports Unicode characters. Some text editors, such as Notepad use ANSI coding by default. Before you save the passphrase using Notepad, select Save As, and then in the Encoding list, select Unicode.

1. As a best practice, save the text file that contains the encryption key on a computer in a secure location on an encrypted hard drive.
