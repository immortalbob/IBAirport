# IBAirport
Multi-character portal bot meta for Vtank

This is a portal bot meta to run an entire account of portal bots. I built this for the portal bot on Reefcull, because what he was using was terrible. Now everyone benefits!

Setup:
1. on line 1 of the meta is the character list, just replace what is in there with your characters (I would put these in the order they are listed on your login screen)
Example: setvar[CharacterOne, Immortalbob]
2. on line 2 of the meta are the trigger words for the portals that can be summoned, please match these to the char list (COnePOne = Character One Primary)
Example: setvar[COnePOne, ayan]
3. on line 3 of the meta are the friendly names, please match these to the char list (COnePri = Character one Primary)
Example: setvar[COnePri, Ayan Baqur]
4. lines 4 and 5 are for the headings that the portals will be summoned. They are using random numbers so if you have your bots all stacked on the same spot they wont summon portals right on top of the last portal summoned (most of the time).
5. lines 6 and 7 are your spam timer and beg for comps timer, these are both in seconds. Standard value is 30 minutes (1800) for spam, and 2 minutes (120) to beg for comps.

Headings explained:
0/360 = N
90 = E
180 = S
260 = W
currently the meta is set up to summon between S and W (200, 250) and between W and N (290,340)

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
Mag-Filter https://github.com/Mag-nus/Mag-Plugins/releases
