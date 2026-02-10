# CAMLbot-CE

CAMLbot (Conversation And Machine Learning bot) is a simple chatbot I've been working on. It's currently capable of learning and responding based on a large collection of scripts: keywords, responses, and priorities. After some training it can hold a basic conversation.

DISCLAMER!!
----
This program is currently under a lot of development and I probably won't remember to update this ReadMe often enough, so realize that a lot of stuff here may quickly become outdated!

SETUP INSTRUCTIONS
-------------------
The first time you download the program, make 3 lists named ʟCMDS, ʟOTPT, and ʟN.
Store {0} into all of them.

CAMLbot starts with no scripts. You'll need make those on your own. It starts with a handful of helpful commands for you to use.

COMMANDS (BUILT-IN)
--------------------
CLEAR - Clears all keywords & responses (ʟCMDS, ʟOTPT, ʟN)

BACKUP - Make a backup copy of the current commands and outputs (stores to ʟCBACK, ʟOBACK, and ʟBACK)

RESTORE - Restores keywords from a backup (see BACKUP)

NEW - Creates a new script (see MAKING A NEW SCRIPT)

GARBAGE - Collects garbage (see LIMITATIONS)

CALC [expression] - Evaluates a numeric expression (so you can still call it a calculator)

BYE - Exits the program

MAKING A NEW SCRIPT
--------------------
To make a new script, do one of two things:
a) Type "NEW", or
b) Type literally anything the calculator doesn't recognize
After either of these, CAMLbot will prompt you to enter a new script. First, input the keyword you want CAMLbot to recognize. After the keyword, input the desired output for that keyword. If that keyword is in any input, it will respond accordingly. Finally, enter the priority. This just means that if your input has more than one keyword in it, the higher-priority one determines the output.
That's pretty much it.

LIMITATIONS
--------------------
- Due to the limitations of TI-BASIC, lists can only hold 999 values, so that's the limit for the number of characters you can store.

- Every time you make something high priority, a "0" is added to the list (stupid TI-BASIC... or is it stupid me?). These 0s add up over time, so you'll need to type "GARBAGE" to do a garbage collect every so often or you'll run out of list space.

- The more commands you input, the slower CAMLbot gets. That's just an inherent property of the program, so be aware that it gets quite slow.

- CAMLbot archives its lists for security purposes, so you can't edit them outside of the program unless you unarchive them (which I recommend you don't do unless you're debugging something weird).

- Don't make any scripts that have built-in commands as keywords (e.g. GARBAGE, BYE, NEW) or they probably won't work as expected.

- If by some cruel coincidence you have another program that needs any lists with the same names as this program's, I don't know what to tell you ¯\\_(ツ)\_/¯

CREDITS
--------------------
- Me for almost everything
- lafferjm in 2006 for a simple Text-to-List and List-to-Text converter I didn't think of for some reason
- spiCE_456 for unknowingly bringing SetUpEditor to my knowledge
- Cars and Ice Cream for the icon editor I used
- ELIZA (the chatbot) for inspiration
- ChatGPT at some point I think but I honestly don't remember
- All of Cemetech for emotional support and Ans optimization documentation

Bug reports are very welcome at https://www.cemetech.net/forum/viewtopic.php?p=314532#314532
