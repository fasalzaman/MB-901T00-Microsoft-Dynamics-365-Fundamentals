---
lab:
    title: 'Lab 03: Enhance security by encrypting your data'
    module: 'Module 03: Recognize Dynamics 365 security'
---

# MB-901: Dynamics 365 Fundamentals
## Module 3, Lab 3: Enhance security by encrypting your data

**Scenario:** You, as a system administrator need to change and copy the organization encryption key.

### Instructions

1. Navigate to Power Platform Admin center.  
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

As a best practice, save the text file that contains the encryption key on a computer in a secure location on an encrypted hard drive.
