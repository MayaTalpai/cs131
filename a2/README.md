1.) What the command does 
Command: chat 

>The chat command is a mimick of a chatbot. A user an use the chat command to interact with a "bot" that has minimal pre-programmed responses

>The "chat bot" spits out a response to certain question or phrase. More responses can be expanded upon. 

>The user input and output from this command is sent to a chat.log so you can look back at conversations with chat. 

>The chat has some API interative capabilites such as https://wttr.in/?format to get weather information and https://official-joke-api.appspot.com/ to have the chat bot tell you a joke. 

>A cron was set up in crontab to clear the chat.log every 14 days via clear_chat
>0 0 */14 * * /bin/bash /mnt/scratch/mayasu24/cs131/a2/clear_chat

>This could also be used to write quick notes to yourself that are timestamped if you need to quickly keep track of "sticky note" type messages and when you left those notes

>In future iterations of this (with more free permissions) I would make this more public. This would make it  a more "chatroom" type enviroment where other users could also use the chat command and leave messages in a chatroom for a group with timestamps. 
 

2.) Why and when this command is useful 
This command makes getting certain information more "human like" such as date, weather, jokes, greetings, and goodbyes. You can use this command to mimic the GUI you might see in a Windows(cortana) OS. Beyond mimicking a chat bot you can use this a somewhat quick way to keep track of notes that may require a time stamp as all responses are recorded in chat.log.  If this were in a more public directory this can be used as an informal or formal chatroom akin to Slack or AOL instant messenger.
 
3.) How you can use this command 
I can use this command to get some preprogrammed responses that I might find amusing or heelpful such as figuring out the weather, the date, or user information. I can write myself notes that are journal like and time stamped. There are also ability to incorpeate more APIs that interest you. Again another way this can be implimented is in a more chatroom like enviroment. 


4.) Examples (copy/paste results) - I copied pasted from the chat.log (but also all of this is also echoed into the teminal real time) 
>Fri Jun 28 00:01:33 EDT 2024 - Maya : hello
>
>Fri Jun 28 00:01:33 EDT 2024 - ROBO-MAYA: Hello, Maya! How are you today?
>
>Fri Jun 28 00:01:44 EDT 2024 - Maya : goodbye
>
>Fri Jun 28 00:01:44 EDT 2024 - ROBO-MAYA: Bye, Maya. Hope to Talk soon
>
?Fri Jun 28 00:02:07 EDT 2024 - Maya : whats todays date?

>Fri Jun 28 00:02:07 EDT 2024 - ROBO-MAYA: The current date is Fri Jun 28 00:02:07 EDT 2024
>
>Fri Jun 28 00:02:30 EDT 2024 - Maya : who am i?
>
>Fri Jun 28 00:02:31 EDT 2024 - ROBO-MAYA: mayasu24
>
>Fri Jun 28 00:02:52 EDT 2024 - Maya : whats the weather?
>
>Fri Jun 28 00:02:52 EDT 2024 - ROBO-MAYA: Weather report:
>

      \   /     Sunny
       .-.      +29(27) °C
    ― (   ) ―   ↘ 17 km/h
       `-’      16 km
      /   \     0.0 mm

>Fri Jun 28 00:03:18 EDT 2024 - Maya : tell me a joke
>
>Fri Jun 28 00:03:18 EDT 2024 - ROBO-MAYA: {"type":"general","setup":"Why did the A go to the bathroom and come out as an E?","punchline":"Because he had a vowel movement.","id":319}
>
>Fri Jun 28 00:06:11 EDT 2024 - Maya : Hey, just a quick note to myself. I want to keep track of this time to log my "lunch" Ill log this again to track when I get back from lunch
>
>Fri Jun 28 00:06:30 EDT 2024 - Maya : Im back from my lunch. A quick lunch
>
>Fri Jun 28 00:07:48 EDT 2024 - Maya : Hey, Bob! This is a note for you if this were in a public directory you would have permission to also use this command and add to this chat log! I did make the permissions for this chmod 777 for future implications.

