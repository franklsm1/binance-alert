A Node-RED app to poll the Binance API every minute to compare the list of trading pairs and send a text message with the new pairs if there are any.  

## Getting Node-RED instance running locally
Run the following commands:
1. `npm install -g node-red`
2. `cd ~/.node-red`
3. `npm install node-red-node-twilio` (needed to add twilio nodes)
4. `node-red`

Then visit: http://localhost:1880

## Binance Alerts Bot Import and Setup
##### 1.) Copy the contents of [nodes.json](../master/nodes.json) into your Node-RED editor using the import clipboard feature.

![alt tag](https://github.com/franklsm1/SlackChannelBot/blob/master/import.PNG)


##### After importing your flow should look similar to this:
![alt tag](../master/exampleFlow.png)

##### 2.) Add your twilio credentials and configure the twilio node
 Note: You can sign up for a free twilio account [here](https://www.twilio.com/try-twilio)

##### 3.) Finally deploy the application and your binance alert bot is up and running!
