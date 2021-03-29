# Connect PI Simulator to IoT Hub

![IoT Hub](images/pi_simulator.png)

Connect a Simulator to your IoT Hub and stream data. 

### In this lab you will

* Learn to create a device using Azure Portal

* Connect the simulator to IoT Hub

* Send telemetry data to Azure

## Create a Device

1. Go to your IoT Hub in the Azure portal, click on **IoT devices** and Click on **+ NEW**

   ![Resource Group](images/new.png)

1. Enter a **Device ID** as **pi-simulator** and click **Save**. 

   ![Resource Group](images/new1.png)

1. Click on the device and copy the Primary Connection String. 

   ![Resource Group](images/connection-string.png)

1. Click on the Pi Simulator icon on the JumpVm desktop.  

1. Replace the connection string with the Primary Connection String copied in the previous step.

   ![Resource Group](images/pi_connection_string_before.png)

1. After you copy the connection string, it should look like below.

   ![Resource Group](images/pi_connection_string_after.png)

1. Click Run and start sending messages. LED will start blinking.

   ![Resource Group](images/pi_message.png)

1. Messages will start flowing into IoT Hub

   ![Resource Group](images/iothub_messages.png)

> **In the next module you can Visualize the Data flowing into IoT Hub**
