# hide-discord-blocked-messages
JavaScript bookmark to run that will stop all blocked messages from displaying.

Copy the code from "block.js" into a bookmark's URL field and run it when starting Discord from the Web browser.

It should also work if you copy everything after "javascript: " and run it from one of the desktop clients.

PLEASE NOTE: MUST BE RUN EVERY TIME DISCORD LOADS (INCLUDING REFRESH).

Change the interval time to whatever you want, but due to the number of comparisons it makes, it might cause lag under 2000 milliseconds, at least if you have a less-powerful processor (although, my testing could also just have been done when Discord decided to do its normal lagging, but can't hurt, either way -- 2 seconds vs. 1).

Works by looping through each instance of messages starting with the "messageGroupBlocked" class and changing the CSS style for display to "none" (had to use a starting-with search, b/c Discord loves to give these things random names...). Little more process intensive than my growmoji script, b/c it needs to check each class that begins with it.

A keen eye might notice that this is a modified copy of the README from my growmoji repo 😹😹😹
