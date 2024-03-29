---
sidebar_position: 1
---

# Pro Tools Renderer

Mixing in Atmos with Pro Tools' integrated Atmos Renderer is the quickest way to get off the ground and mixing in Atmos. It requires minimal setup as well as portability between machines. Follow these steps to ensure a smooth mixing session.

## DADman

The first thing you'll want to do is ensure that DADman is configured to support your session. For a mixing session, using the Pro Tools' integrated Atmos Renderer, the files loaded for DADman should read "ERR_Main.dms" and "ERR_Pancakes_PlusHP.dmprof"

<!-- Insert a picture of the toolbar on Dadman where somebody could read the profiles. -->

Next, ensure that your Source is properly selected. For non-Atmos mixing, you will select the source "Pro Tools". 

<!-- Insert a picture of the proper source selected. -->

## Pro Tools

Now that you have the monitoring system set up, you'll want to ensure the the Pro Tools I/O is properly configured.

### I/O
In Pro Tools, go to Setup>I/O. In the bottom left of the window that pops up, check "Apply to all tabs" and select "Import Settings." The correct I/O will be called "ERR_MAIN.pio"

<!-- image -->

Next, navigate to the "Atmos Renderer" tab. Ensure that the renderer box is checked [1]. Set the renderer to "Internal Renderer" [2]. Now you can easily set up the Bed and Objects by navigating to the bottom and selecting "Pull objects from Renderer" [3].

<!-- image -->

### Routing

Now that you have your I/O set up, open the Renderer by navigating to "Windows>Renderer" or pressing control+command+=. Make sure your monitoring format is set to 7.1.4 (by default it is set to 5.1). 

<!-- image -->

And you're finished! Now you can assign tracks to objects and use the 7.1.2 Bed as an output.