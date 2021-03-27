# Load test with Device Simulator

Learn how to set up a Device Simulator using Azure IoT Suite and Connect to IoTHub

## Create Device Simulator

1. Open parameters.json file in the **Visual Studio code** from the following path : *C:\azure-iot-pcs-device-simulation\azure-iot-pcs-device-simulation-master\deployment\armtemplate*

2. Now replace the parameters.json file as mentioned below:
      
   * **deploymentRegion**: eastus2
   * **aadTenantId**: Copy from the Lab **Environment Details** tab
   * **subscriptionId**: Copy from the Lab **Environment Details** tab
   * **solutionName**: Enter a short unique string and append it with the **Deployment ID** which can be fetched from the Lab **Environment Details** tab
   * **adminUsername**: Provide a username for Virtual Machine.
   * **adminPassword**: Provide a password for Virtual Machine.
  
   > **Note** : Pleae make sure you are providing a unique string for the *solutionName* parameter or else the deployment will fail.

3. Save the parameters.json file.

4. Now Open Command Prompt as **Run as Administrator** and navigate to deployment file.

   ```
   cd C:\azure-iot-pcs-device-simulation\azure-iot-pcs-device-simulation-master\deployment

   ```
5. Now run the following commands to deploy the device simulator in your subscription.

   ```
   npm install
   ```

   ```
   npm run deploy
   ```

Then the script starts running and it might ask you to login multiple times. Please login when required as mentioned in the prompt. The deployment will take approximately 10 minutes to succeed.

6. Once the deployment succeeds, you will be presented with a URL to access the Simulation UI.

7. A new resource group with a IoTHub resource in it. 


## Stream Data to IoTHub

Get connection string of IoT Hub

![Get Connection String](images/06_get_connection_string.png)

Setup simulation with sensors and number of devices

![Simulate Data](images/07_simulate_data.png)

Select the frequency of data flowing into IoT Hub 

![Imported Script](images/08_start_simulation.png "Start Simulation")

## New Devices Created in IoTHub

![Simulation Devices](images/09_simulated_devices.png)
