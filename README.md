
# Train Driver 2 Stream Deck Profiles

I always wanted to be able to play TD2 using Stream Deck. The implementation for this is not so easy to do, but I have now found a way that works. 

## Authors

- BravuraLion


## Current Profiles

- Stream Deck XL Profile for ET41
- Stream Deck XL Profile for EP08
- Stream Deck XL Profile for EN57
- More on the way


## Installation

Before you can use the Profiles, you have to Setup Stream Deack that in runs with Admin Rights. The Profiles will not work if Stream Deck is running without that rights. You can find a very good Tutorial for that here: http://skylark-creative.com/blog/run-elgato-stream-deck-as-administrator-in-windows-10 

Method B: Kill Stream Deck Process, Run Stream Deck as Admin

Next Copy the Stream Deck Folder from Github to your C: Driver that the path to the AutoHotkey, Picture and Profiles Folders look like this: C:\StreamDeck\TD2

After that, Open Stream Deck, Go to the Profile Manager and Select "Import Profile" and select the Profile you want to use.

The Profile should be now loaded to Stream Deck. If the Icons are missing, you can re add them via the Pictures Folder


    
## FAQ

#### Why does Stream Deck have to run as Admin?

Since Train Driver 2 itself runs in Admin mode, Stream Deck must also be running in Admin mode in order to send the hotkeys to the game.

#### Why do you use the Autohotkeys.exe for the Shunting Function

This is because the game does not recognize the hotkeys via the normal Stream Deck hotkey function of NUM* and NUM/. It also does not work with Barraider. I have already reported this issue to https://www.reddit.com/r/SteamDeck/comments/14qaph0/numpad_and_not_working_as_hotkeys/. Other games have problems with this too. If you don't trust the Exes, you can build it yourself with Autohotkey https://www.autohotkey.com/ A template for the code can be found in the Autohotkey folder. Currently i have no alternative to solve that issue.

#### Windows Reports the AutoHotkey Exes as Virus

Jeah happened to me too, false positive


## Lessons Learned

It was exciting to see that NUM/ and NUM* are sent differently depending on the program and certain programs do not perceive this as correct input. Autohotkey has helped me a lot. I will see if this can not be solved better via the API of Train Driver 2.
If so, it would also be conceivable to get the Raildriver to run.
Also I would like to have a MultiHotKey in Stream Deck that can do more than 2 positions. 4 would be ideal, then you can display the switch positions better. It would also be good if this could be linked to a multi action that first focuses on TD2, and then executes the hotkey. That would already work now, but then you don't have different status images for the actions anymore.


