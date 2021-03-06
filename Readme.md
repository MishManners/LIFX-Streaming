## LIFX Code for Elgato Stream Deck

This is the Python code used to control [LIFX](https://www.lifx.com/) lights with the [Elgato Stream Deck](https://www.elgato.com/en/gaming/stream-deck).

![LIFX](https://github.com/MishManners/LIFX-Streaming/blob/master/Images/Screenshot-2017-09-16-19.31.17.png)

### Python Instructions

Go to [LIFX Cloud token](https://cloud.lifx.com/settings) and grab your API settings/keys from your account. You'll see different keys for each light/scene.

1. Open the .bat file and change the location of where the .pyw file is located. (.pyw means the script will run without oppening the command window).
2. Save .bat file
3. Open .pyw file add the API key for the thing you want to control
4. Add the UUID for the scene you'd like to change (make sure it's the SCENE UUID, not the ACCOUNT UUID). Make any other changes you'd like.
5. Save .pyw file

If you're using .py and not .pyw, you'll need to use the .vbs file to ensure the command window doesn't pop up. To do this, open .vbs file and change the location of where the .py file is located. The .vbs file is simply there to ensure the python script runs in the background.

If you head to [LIFX API](https://api.developer.lifx.com/docs/list-scenes) and scroll to the bottom of the screen, you'll see a key and a list of scenes. Add your API key and it will give you the UUID for every scene you have connected to that API. Use those scenes to activate and control your lights.

Check out the [LIFX Dev Tools and API](https://api.developer.lifx.com/) to grab all your details. Once you have your scene and light keys, you can add them into the file. The .py file will open a command line. .pyw will be without the command line. However Python 3 should start this up without any worries.

### Elgato Stream Deck Instructions

Now all you need to do is map the Python Code to your stream deck.

![Elgato](https://github.com/MishManners/LIFX-Streaming/blob/master/Images/personalized_photo.jpg)

1. Open Elgato Stream Deck (the software)
2. Add a new "Open" button to your deck (you'll find this under "System")
3. Change title, and then point "App/File" to your .pyw file

There you go. You're all set to control your LIFX lights with your Elgato Stream Deck. Note as of Oct 2020, there is a simple LIFX module you can install on the stream deck, however the Python code gives you a lot more control over scenes and effects.


Thanks to [ImSammy](https://www.youtube.com/watch?v=UP3PQu4PlaY) who originally put together the video tutorial. Thanks Sammy for all your hard work.
