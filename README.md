# PDTravelsBot
A Sample BOT project for a Imaginary Travels company


To Run the Project using Microsoft Bot Framework emulator:
Make sure Bot Framework Emulator is installed. 
You can get the same from here: 
https://github.com/Microsoft/BotFramework-Emulator/releases  
=> Download latest version of exe and install the same.
Latest version of Bot Framework Emulator is: botframework-emulator-Setup-3.5.35.exe

Set the PDTravels.BotApp as Startup Project in the Visual Studio.
Hit F5
Then the application will run. Copy the app url (http://localhost:3979/)
Run the BotFramework-Emulator.
In the "Enter your endpoint URL" box paste the copied app url and append /api/messages (http://localhost:3979/api/messages)
Now if you type in some message and send, you should get a response that says what message you sent and the number of characters in it.

Message: Hello World!
Response: You sent Hello World! which was 12 characters

In the Details pane you can see the JSON representation for the messages and responses. (Click on any of the text in the conversation, then the Details pane will show the respective JSON)

Hello World!:
{
  "type": "message",
  "text": "Hello World!",
  "from": {
    "id": "default-user",
    "name": "User"
  },
  "locale": "en-US",
  "textFormat": "plain",
  "timestamp": "2018-04-25T21:57:57.375Z",
  "channelData": {
    "clientActivityId": "1524693468872.14024477482011233.0"
  },
  "entities": [
    {
      "type": "ClientCapabilities",
      "requiresBotState": true,
      "supportsTts": true,
      "supportsListening": true
    }
  ],
  "id": "03gf76jk51if8d"
}

Response:

{
  "type": "message",
  "timestamp": "2018-04-25T21:57:58.101Z",
  "localTimestamp": "2018-04-25T17:57:58-04:00",
  "serviceUrl": "http://localhost:62784",
  "channelId": "emulator",
  "from": {
    "id": "bief1gh96hfl",
    "name": "Bot"
  },
  "conversation": {
    "id": "15m24h1jg40dc"
  },
  "recipient": {
    "id": "default-user"
  },
  "membersAdded": [],
  "membersRemoved": [],
  "locale": "en-US",
  "text": "You sent Hello World! which was 12 characters",
  "attachments": [],
  "entities": [],
  "replyToId": "03gf76jk51if8d",
  "id": "nfl1ll401f0a"
}

In the Log Page you can see the entire interactions (Request / response) log.

Log:
[17:57:44] Emulator listening on http://[::]:62784 
[17:57:44] ngrok not configured (only needed when connecting to remotely hosted bots) 
[17:57:44] Connecting to bots hosted remotely 
[17:57:44] Edit ngrok settings 
[17:57:44] Checking for new version... 
[17:57:45] Application is up to date. 
[17:57:51] -> POST 200 [conversationUpdate] 
[17:57:51] -> POST 200 [conversationUpdate] 
[17:57:57] Warning: The Bot Framework State API is not recommended for production environments, and may be deprecated in a future release. Learn how to implement your own storage adapter. 
[17:57:57] <- GET 200 getConversationData 
[17:57:57] <- GET 200 getPrivateConversationData 
[17:57:57] <- GET 200 getUserData 
[17:57:58] <- POST 200 Reply[message] You sent Hello World! which was 12 characters 
[17:57:58] <- POST 200 setConversationData 
[17:57:58] <- POST 200 setUserData 
[17:57:58] <- POST 200 setPrivateConversationData 
[17:57:58] -> POST 200 [message] Hello World! 
[17:57:58] Warning: The latest bot SDK version is 3.15.0 but the bot is running SDK version 3.8.0. Consider upgrading the bot to the latest SDK. 