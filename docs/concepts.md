# Concepts

## What is it?

- **An enhanced experience for the traditional RF users**
  - RF PLUS PLUS provides a significantly improved user experience for those who are accustomed to traditional RF devices. The application leverages modern technology to make warehouse operations more efficient and user-friendly.

- **Utilizes android platform**
  - The application is built on the Android platform, ensuring compatibility with a wide range of modern devices. This choice allows for greater flexibility, ease of use, and access to advanced features available on Android devices.

## How does it work?

- **Running existing MTF forms**
  - RF PLUS PLUS operates by utilizing existing MTF forms. This integration ensures that the app can seamlessly adopt and enhance current workflows without requiring major changes to the underlying systems.

- **Determining device ID and terminal ID through device hardware settings**
  - The app determines the device ID and terminal ID by accessing the hardware settings of the device. This automatic identification process simplifies device registration and management.

- **Showing additional information**
  - RF PLUS PLUS allows for the display of additional information on the RF screens. This can include data from BY sources or external databases, enhancing the user experience with more comprehensive and useful information.

## What does it need on the server?

- **MTF server task reservation**
  - An MTF server task must be reserved for RF PLUS PLUS. This task can be an existing one or a newly created task dedicated to the application.

- **Script to create 1000 devices**
  - Below script run to create device IDs ranging from SM00001 to SM05000. This pre-creation of device IDs ensures that the server task does not need to be restarted frequently, streamlining the registration process.

- **Device registration against the environment**
  - Once the devices are created, they are registered against the desired environment. This registration process ensures that each device is properly configured to interact with the RF PLUS PLUS application and the underlying systems.
