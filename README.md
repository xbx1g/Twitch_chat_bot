Code Description:

This script connects to a Twitch chat via WebSocket and listens for specific keywords in chat messages. When a keyword is detected, the bot sends a corresponding message to the chat, with a cooldown period to prevent spamming. The keywords, messages, and cooldown states are managed dynamically using an array of command objects, simplifying the addition of new commands.
How to Add/Change Commands:

    To Add a New Command:
        Find the commands array in the code.
        Add a new object to the array with the following structure:

        javascript

    { keyword: "NEW_KEYWORD", message: "NEW_MESSAGE", cooldown: false }

    Replace NEW_KEYWORD with the keyword to detect and NEW_MESSAGE with the message to send.

To Change an Existing Command:

    Locate the command in the commands array you want to modify.
    Update the keyword or message properties as needed. For example:

    javascript

    { keyword: "UPDATED_KEYWORD", message: "UPDATED_MESSAGE", cooldown: false }

To Adjust the Cooldown Duration:

    Modify the cooldownDuration variable (in milliseconds) at the top of the script:

    javascript

        const cooldownDuration = 30000; // 30 seconds

        Set the value to your desired cooldown time.

These simple changes will allow you to customize the bot’s behavior to suit your needs.
