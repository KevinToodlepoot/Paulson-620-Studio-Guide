---
sidebar_position: 2
---

# Atmos Renderer

Using the Atmos Renderer application on the computer begins to get a bit more complicated than just using the integrated Pro Tools renderer. We will use Pro Tools Aux I/O to route the audio to the Renderer and back into Pro Tools to the speakers. Here are the steps to achieve using the Atmos Renderer application for mixing.

## DADman

The first thing you'll want to do is ensure that DADman is configured to support your session. For a mixing session, using the Atmos Renderer application, the files loaded for DADman should read "ERR_Main.dms" and "ERR_Pancakes_PlusHP.dmprof"

<!-- Insert a picture of the toolbar on Dadman where somebody could read the profiles. -->

Next, ensure that your Source is properly selected. For non-Atmos mixing, you will select the source "Pro Tools". 

<!-- Insert a picture of the proper source selected. -->

## Atmos Renderer

Open the "Dolby Atmos Renderer" application located on the left of the computer's dock.

<!-- image -->

Navigate to the preferences by either going to Dolby Atmos Renderer>Preferences in the toolbar, or pressing command+, . Now ensure the driver is set up so that Audio Driver is "Core Audio", audio input device is "Dolby Audio Bridge", and audio output device is "Pro Tools Audio Bridge 16".

<!-- image -->

## Pro Tools

Now, while keeping the Atmos Renderer application open, navigate to your Pro Tools session. 

### I/O

Go to Setup>I/O and navigate to the Output tab. In the bottom left of the window, ensure that "Apply to all tabs" is checked and select "Import Settings". The I/O file to import is "ERR_ATMOS_RENDERER.pio". After loading the I/O file, you should be able to scroll all the way to right and see an output device called "Dolby Audio Bridge" with all the objects as well as the bed mapped to it.

<!-- image -->

<!-- link to "What if I don't see the objects mapped? -->

Next, navigate to the "Dolby Atmos" tab. Ensure that the renderer box is checked [1]. Set the renderer to "External Renderer" [2] and set the Renderer Host to "ORR-DAW-MacPro.local" [3]. Now you can easily set up the Bed and Objects by navigating to the bottom and selecting "Pull objects from Renderer" [4].

### Routing

Now for each track in your Pro Tools session, you should be able to assign it to an object and see the signal in the Atmos Renderer application.

<!-- image -->

Now, to get output, go back into your Pro Tools session and create a new 7.1.4 Aux track. Set this track's input to be "Pro Tools Audio Bridge (7.1.4)" and the output to be "Output (7.1.4)". This track allows you to monitor what's coming from the Dolby Atmos Renderer. 

<!-- image -->

Everything should be good to go now, and you should be able to assign tracks as objects and use the 7.1.2 Bed. 