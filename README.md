# Rule based Slackbot
This is a chatbot that runs on Python and liases with Slack. The bot needs to be created on Slack first and the webhooks have to be enabled.

The Python program is the core of this bot. 

1. The program makes a direct socket connection to Slack using Real Time Messaging or RTM API given by Slack. 
2. The user's entries are sent into the Python program/chatbot engine
3. The chatbot engine looks up the 1st and 2nd word of the user's entry and compares to the list of commands in an Excel spreadsheet. 
4. If the action is identified then the remaining string is argument for the action.
    e.g. weather of Atlanta
6. The engine identifies the action to be taken and then executes it
7. If the engine cannot identify an action, it just searches on Wikipedia or WolframAlpha for the entire user entry to get an answer
