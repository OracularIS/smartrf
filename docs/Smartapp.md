# Smart Apps Setup

## Overview

The Smart Apps Setup for RF++ involves defining the necessary MTF  parameters to ensure smooth operation. This setup includes the execution of a script to create up to 5,000 devices, identified by IDs ranging from SM00001 to SM05000. By pre-creating these device IDs, the system avoids frequent task restarts, streamlining the registration process and ensuring efficient device management.

## Getting RF PLUS Account

To use Smart RF Plus, users need to register themselves on the SmartApps platform and subscribe to the Smart RF PLUS feature. Follow these steps:

1. **Register on SmartApps**:
   - Visit the [SmartApps registration page](https://apps.smart-is.com/).
   - Fill out the registration form with the required information.
   - Verify your email address to complete the registration process.

2. **Subscribe to Smart RF PLUS**:
   - Log in to your SmartApps account.
   ![Smartapphome](./attachments/Smartapp/smartapphome.png)

   - Select the Smart RF PLUS feature and click subscribe Button.
   ![Rfsubscrib](./attachments/Smartapp/RFsubscribe.png)
   - After clicking on confirmation promt will appear read it and acknowledge to smart-is policy. And click on th submit button.
   ![Confirmationoprompt](./attachments/Smartapp/cofirmation.png)

   - After subscribing Smart Rf plus feature will appear in your menu
  

## Profile Concepts

The profile concept within Smart RF Plus maps each profile to a specific production instance. This mapping allows for precise configuration and management of connections to various production environments, ensuring that each instance operates correctly and efficiently within its designated setup.

## Profile Setup Concepts

Profile setup is critical as it defines the environment and warehouse ID where the MTF tasks will be executed. In this setup, users provide detailed information, including the exact URL and port for the MTF service. The key elements of the profile setup include:

- **Environment**: Specifies the production environment on which the connection will be established. This is crucial for ensuring that the Smart RF Plus application interacts with the correct backend systems.
  
- **Warehouse ID**: Identifies the specific warehouse within the chosen environment. This allows the application to tailor its operations to the particular needs and configurations of the warehouse.

- **MTF Information**: Users must provide the MTF URL and port details. These parameters ensure that the Smart RF Plus application can communicate effectively with the MTF server, executing tasks and retrieving necessary data.

### Profile Setup Process

1. **Define Production Environment**:
   - Specify the exact production environment for the profile.
   - Ensure that all configurations align with the requirements of the production instance.

2. **Add Environment and Warehouse ID**:
   - Input the specific environment details.
   - Include the warehouse ID where the MTF tasks will be executed.

3. **Provide MTF Details**:
   - Enter the MTF URL and port information.
   - Ensure these details are accurate to enable proper communication between the Smart RF Plus app and the MTF server.

By carefully setting up profiles and defining the necessary parameters, Smart RF Plus ensures a robust and efficient connection to the production environments, enhancing the overall effectiveness of warehouse operations.
