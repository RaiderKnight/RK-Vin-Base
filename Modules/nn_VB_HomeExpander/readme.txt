NickNo's HomeExtensions (LifePlay) ReadMe, Change Log and TODO List
===================================================================

ReadMe
********

HomeExtensions (HE) allows you to add more rooms and life to your home.

Before you are able to use a room you need to build it. Select "Build a new room (HE)" when at home to do so.
When building a room you can choose between DIY (if you got enough energy, fitness etc.) or hire workers to do the job for you.

It will take between 6-10 hours to build the room, depending on your choice.

If you go for the DIY route its cheaper, takes longer but you gain some fitness, intelligence, muscle etc - if you let the workers do it, its more expensive but faster.

If you constructed a second and/or third bedroom you can rent it to earn some money... Or do lewd things with your tenants. ;-)

Renting rooms to others
~~~~~~~~~~~~~~~~~~~~~~~
The bedrooms 2+3 can be let to others.
Just select "Manage rented rooms (HE)" from the home menu.

If you want someone from your contacts to move in
- the person must not be married
- the person must like you (rapportwithplayer > -10)
- Chances are better if the person is dating you

If you put the rooms on advertising anybody may move in.

To collect your rent use the action "Collect rental fee (HE)" action.
This is available weekly. (Or in larger intervalls.)

Tenants may also move out randomly!

Lewd scenes and how they work
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
There are several lewd scenes that either trigger randomly or by doing certain actions:
- Go to the bathroom
- Go to a rented room (WIP)
- Go to the Kitchen (WIP)
- Be in your office (WIP)
- Be alone and in your home

These scenes lead to different outcomes depending on the rapport the actor has with you as well as its
- perversion
- arousal
- masochist stat

If perversion and arousal are high you have the chance to encounter a sex scene, also if the person is submissive enough.

Rapport, Perversion and Arousal stats will raise by regularily by checking on the tenants wherever they are.
(Rapport may also decrease if you disturb Tenants too often!)

Known problems
~~~~~~~~~~~~~~

Prob: Sleeping tenants are not sleeping
A: If you visit one of your tenants at night, you may get a sleeping 
scene but the actor does something else. This is due to a bug in LP 3.18 where the 
animations do not play as intended. Vinfamy is working on it.

---------------------------------

Prob: Random (non HE) scenes seem to hang
A: This happens in the rare moment when a Home Expander scene is 
running and the game engine decides to trigger a random event that needs the sceneUI.
Workaround: Click the red "Emergency" text in the bottom right corner to exit the random scene.

------------------------------------

Prob: I see two "Go to the bathroom" actions
A: The original "Go to bathroom" is hard wired into the game.
If you want to get rid of it, open the file 
'LifePlay\Content\Modules\vin_Base\Actions\basicneeds\go_to_the_bathroom.lpaction'
with your text editor and remove the "home, " from the WHERE line, keeping the rest.

--------------------------------------

Prob: Sometimes the "Manage rented rooms" action shows no tenants
A: Yep, I can confirm this. But yet I do not know how to solve it.
I think I found a "dirty" workaround and implemented it.
If it still happens please close and reopen the menu.

--------------------------------------

Prob: If I interact with Tenants in the new rooms we end up in my bedroom.
A: Yep... magic. Or better: We are still working on this. 
The 3D background is lost with each interaction. Wait for LP 3.19 ;)



Change Log
************

Version 0.4 (06.01.2021):
-> Requires LP 3.18 !!!
- Tenants now may be encountered in the livingroom or kitchen, they act like other AI controlled NPCs
- Tenants may now be encountered in their rooms, they act like other AI controlled NPCs
- Tenant rooms will be locked / populated depending on the daytime and work of tenant.
- Tenants usually sleep from 23-6 and are away from 10-16
- Peeking through the keyhole added for bath and tenant rooms. You may either: 
    - see a sex scene (30%)
    - get caught with the sneaking mini game coming up to esacpe (30%)
    - see noting interesting
- Spy cam can be used if installed. Will result in not being caught when spying.
- Spy cam quest "Master Spy!" added (rewards if all rooms have cams)
- Camera position and focus change for spycam & key hole "feeling"
- Added 3 interactions with tenants to ask them to
  - never lock their doors
  - walk around in undies
  - walk around naked
  -> All interactions will just work. They do not have any text or conditions (yet).

Version 0.3 (30.12.2020):
- Added option to let bedroom 2+3 to tenants
- Added scene for random tenant applications
- Added scene where tenant moves out due to random circumstances...
- Added scene for random bathroom events (if alone, can also be triggered manually by going to the bathroom)
- Bathroom party quest added
- Added scene to meet one or both tenants in the kitchen 
- Added scene to meet one or both tenants in their rooms 
- Bedroom 2+3 redesigned to fit their purpose better...
- Fix: Collect rent will now work properly on first try. (It paid out a little too much :))
- Name of the mod changed to "HomeExtensions"

Version 0.2 (28.12.2020):
- Rooms (other than bathroom) now need to be unlocked by building them (see readme)
- 3rd bedroom added
- Kitchen added
- Other 3D rooms enhanced, spawn point for player set
- All rooms have doors now... ^_^
- If Player has a dog it will show up randomly in rooms
- Ability to rent bedroom 2+3 added
    -> Currently tenants do not show up. Need to discuss this with Vinfamy.
    -> This is not a bug in the mod or the game. I bet I am using the modding API in a way Vinfamy did not plan it ... yet. :D
- Rent can be collected weekly (or at larger intervalls but no less than 7 days)


Version 0.1 (28.12.2020):
- Initial release based on F95 idea https://f95zone.to/threads/lifeplay-v3-17-vinfamy.11321/post-4808049


TODOs (Planned features by NickNo)
************************************
Developer
- Add special interactions to the NPCs / rooms
- Add scene where NPC cannot pay rent and needs to do other services
- Let tenants have intercourse or hate e/o (WIP)
- Let tenants have dates with other NPCs
- Add more quests
- Use intoxication of tenants for certain events

PRIO 1
- Make use of weekdays as soon as an API exists

PRIO 2
- If player has relatives randomly show them

PRIO 3
- Also rent rooms to submissive ppl

Feature Requests (Requested by others)
****************************************
LifePlay Patrons will be served first!

REQEST: Example request
FROM: NickNo (Discord)


Developer & Tester Notes
**************************

You can call the debug menu using the following #-key command: nn_he_debug
In this menu you can 
- enable all rooms / cams
- disable all rooms / cams
- kick all tenants out
