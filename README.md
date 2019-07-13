# IBAirport
Multi-character portal bot meta for Vtank

This is a portal bot meta to run an entire account of portal bots. I built this for the portal bot on Reefcull, because what he was using was terrible. Now everyone benefits!

Setup:
1. on line 2 of the meta is the character list, just replace what is in there with your characters (I would put these in the order they are listed on your login screen)
Example: setvar[CharacterOne, Immortalbob]
2. on line 3 of the meta are the trigger words for the portals that can be summoned, please match these to the char list (COnePOne = Character One Primary)
Example: setvar[COnePOne, ayan]
3. on line 4 of the meta are the friendly names, please match these to the char list (COnePri = Character one Primary)
Example: setvar[COnePri, Ayan Baqur]
4. on line 5 is the meta file name, if you wish to use multiple bots on the same computer, they will need their own meta file with a unique name. Do not use numbers, spaces, or symbols in the file name.
5. lines 6 and 7 are for the headings that the portals will be summoned. They are using random numbers so if you have your bots all stacked on the same spot they wont summon portals right on top of the last portal summoned (most of the time).
5. lines 8 and 9 are your spam timer and beg for comps timer, these are both in seconds. Standard value is 30 minutes (1800) for spam, and 2 minutes (120) to beg for comps.
6. lines 10 and 11 are for password restricted access. enable usepassword and change the password in the next line.

Headings explained:
0/360 = N
90 = E
180 = S
260 = W
currently the meta is set up to summon between S and W (200, 250) and between W and N (290,340)

If "UsePassword" is enabled:
-bot will sit silent, and only react to @tells, no local chat
-when correct password is received, it will go into normal functionality.
-if no command is sent after password is received, and after 60 seconds, bot will return to only accepting the password
-after a successful portal summon, bot will require the password again.

Notes:
If you want to use parenthesis in your friendly names, you must escape them with a \
Example: Ayan Baqur \(Panopticon\)

Commands Accepted
whereto - @tells your list of triggers, and friendly names to the requester.
help - @tells the requester to use whereto
trigger words - your triggers for summoning portals

Known Issues:
1. Sometimes the server wont process your log out correctly, its not the meta, its the emulator
2. Sometimes the /vt start command wont go through upon login, very rarely

Requiremets:
Decal
Vtank
Mag-Tools
Mag-Filter https://github.com/Mag-nus/Mag-Plugins/releases
