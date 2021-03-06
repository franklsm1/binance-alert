A Node-RED app/bot that polls the Binance API every minute (configureable) to check for new coin listings and sends a text message with the new coin(s) name if there was any.

## Prerequisites
- basic knowledge around opening up and using a terminal
- git command line utility installed
- node v6 and up installed (verify using `node -v` command)
- npm v3.10 and up installed (verify using `npm -v` command)

**Note:** You can download and install the latest version of node and npm from [here](https://nodejs.org/en/download/) or the git CLI from [here](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) if you do not have them installed

## Getting Binance Alerts bot installed and running locally
#### 1.) Run the following commands so install and start the app:
1. `git clone https://github.com/franklsm1/binance-alert.git`
2. `npm install`
3. `npm start`

Then visit: http://localhost:1880

##### Your Node-RED instance should look similar to this:
![alt tag](../master/exampleFlow.png)

#### 2.) Add your twilio credentials and configure the twilio node
1. Double click on the red twilio node to open the UI
2. Click the pencil image to add your Twilio Account SID, From phone number, and Token found on your [twilio console](https://www.twilio.com/console)
3. Click the **Add** button to add your Twilio credentials
4. Fill out the **To** phone number in the Twilio node UI with your number
5. Click the **Done** button to save everything
 
 **Note:** You can sign up for a free twilio trial account [here](https://www.twilio.com/try-twilio). You get free text messages with "Sent from your Twilio trial account - " prefixed to ll of your messages, which is no big deal.

#### 3.) Deploy the application and your binance alert bot is wired up and running!
**Example:**

![alt tag](../master/image.png)

## Deploy to AWS (optional)
Check out [this guide](https://nodered.org/docs/platforms/aws) on how to deploy Node-RED to AWS and run the bot there
