# SMART RF PLUS Quick Start

Welcome to SMART RF PLUS, your comprehensive solution for efficient warehouse operations. This guide will walk you through the steps to register a new device and operate it seamlessly within your environment.
## Prerequisite

- **MTF Server Task Reservation**
  - Reserve a task for Smart RF Plus (existing or new).

- **Server Configurations**
  - Specify the MTF protocol (SSH or Telnet):
    - For Telnet: `-N Telnet`
    - For SSH: `-N SSH`
  - Add debug parameters: `-G22,1`

## Sign Up and Subscribe

1. **Sign Up on SmartApps**
   - Go to [SmartApps Registration](https://apps.smart-is.com/register).
   - Fill out the registration form with your name and email, then submit.
   - Verify your email by clicking the link sent to you.

   <img src="./attachments/deviceregistration/signup.png" alt="configuration" style="height: 200px; margin: auto; display: block">
2. **Verify Your Email**
   - Check your email for a verification link.
   - Click the verification link to activate your SmartApps account.


 ### Subscribe to Smart RF PLUS
   - Log in to your SmartApps account.
   - Navigate to the product subscription page.
   - Select Smart RF PLUS from the list and follow the prompts to subscribe.

For detailed instructions, please refer to the [Subscribe to Smart RF PLUS Feature](device_registration.md#subscribe-to-smart-rf-plus-feature) section 

## Profile Group Setup

Profile groups in Smart RF Plus allow you to organize multiple profiles, each representing a different instance. This helps in managing configurations efficiently.

   <img src="./attachments/deviceregistration/profile_group.png" alt="profile_group" style="height: 200px; margin: auto; display: block">

   For detailed instructions, please refer to the [Profile Group](device_registration.md#profile-group) section.

## Defining Profiles within the Group

Profiles represent specific instances within a profile group. Each profile can be configured to connect to different environments.

   <img src="./attachments/deviceregistration/profile.png" alt="profile" style="height: 200px; margin: auto; display: block">


   For detailed instructions, please refer to the [Profile Details](device_registration.md#profiles) section.

## Profile Setup

After defining profiles, you need to configure the profile setup for each profile. This involves specifying the host, port, and warehouse ID (wh_id).


   <img src="./attachments/deviceregistration/profile_setup.png" alt="profile_setup" style="height: 200px; margin: auto; display: block">

   For detailed instructions, please refer to the [Profile Setup Details](device_registration.md#profile-setup) section.

**Generate QR Code for Profile**
   - Click on actions against the profile setup to generate a QR code.

   <img src="./attachments/deviceregistration/profileqr.png" alt="profileqr" style="height: 200px; margin: auto; display: block">

## Download and Install Smart RF Plus

1. **From Google Play Store**
   - Open Google Play Store on your Android device.
   - Search for "Smart RF Plus" and install the app.

   <img src="./attachments/gettingrf/Searchrf.png" alt="Searchrf" style="height: 200px; margin: auto; display: block">
   <img src="./attachments/gettingrf/installrf.png" alt="installrf" style="height: 200px; margin: auto; display: block">

2. **Direct Download from Smart IS Website**
   - Scan the QR code below to go to the Smart RF Plus download page:
     
     <img src="./attachments/gettingrf/appqrcode.png" alt="appqrcode" style="height: 200px; margin: auto; display: block">
     
   - Or visit [Smart IS Website](https://www.smart-is.com/what-we-do/smart-product/rf/).

## Registering New Devices

1. **Open the SMART RF PLUS App on Your Android Device**
   - On your Android device, open the SMART RF PLUS app.
   - Click on the "Register Device" Button.

   <img src="./attachments/deviceregistration/registerscreen.png" alt="registerscreen" style="height: 200px; margin: auto; display: block">

2. **Scan the QR Code**
   - Use the SMART RF PLUS app to scan the QR code displayed on your profile setup screen.

   <img src="./attachments/deviceregistration/scanner.png" alt="scanner" style="height: 200px; margin: auto; display: block">

   - This will automatically register your device with the selected profile setup.
   - Your profile will be displayed under the environment section of the Smart RF Plus home screen.

   **Running script for the bulk devices**
    -  You can run a script on your MOCA system to register multiple devices in bulk. This process helps to avoid the need to restart the task for each individual device registration, streamlining the overall setup.
    For detailed instructions, please refer to the [SQL Script for Device and RF Terminal Creation](concepts.md#what-does-it-need-on-the-server) section.

   ## Connecting to the Environment

 **Connect the Environment**
   - On the RF PLUS home screen, select the environment from the dropdown.
   - Click the "Connect" button to initiate the connection.
   
   <img src="./attachments/basicflow/environment.png" alt="environment" style="height: 200px; margin: auto; display: block">

 **Login Prompt**
   - Enter the username and password for the selected environment.
   - Ensure the credentials are correct to establish a secure connection.
   
   <img src="./attachments/basicflow/Login.png" alt="login" style="height: 200px; margin: auto; display: block">

 **Telnet Session**
   - A telnet session will start, automatically inputting the terminal ID from the QR code along with the login credentials.
   
   <img src="./attachments/basicflow/telnetlogin.png" alt="telnetlogin" style="height: 200px; margin: auto; display: block">

 **Access Smart RF PLUS Home Screen**
   - The work information page will be displayed.
   - Enter your work location and warehouse equipment type. The Smart RF undirected menu will then appear.
   
   <img src="./attachments/basicflow/workinfo.png" alt="workinfo" style="height: 200px; margin: auto; display: block">
   <img src="./attachments/basicflow/undirectedmenu.png" alt="undirectedmenu" style="height: 200px; margin: auto; display: block">

   - You can now access various features and functionalities of the Smart RF PLUS device.

By following these steps, you can quickly get started with Smart RF Plus and enhance your warehouse operations.
