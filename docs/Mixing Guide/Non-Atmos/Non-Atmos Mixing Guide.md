

# Non-Atmos Mixing Guide

This guide is for Mixing sessions that do not require the Atmos Renderer. This means you will be mixing and monitoring in Stereo or 7.1.4 channel-based surround. The following steps will guide you through the process of setting up for your mixing session.

## DADman

The first thing you'll want to do is ensure that DADman is configured to support your session. For a mixing session, not using the Atmos Renderer, the files loaded for DADman should read "ERR_Main.dms" and "ERR_Pancakes_PlusHP.dmprof"

<!-- Insert a picture of the toolbar on Dadman where somebody could read the profiles. -->

Next, ensure that your Source is properly selected. For non-Atmos mixing, you will select the source "Pro Tools". 

<!-- Insert a picture of the proper source selected. -->

If you want to monitor on headphones at all, you can do the same thing for the output labeled "Headphones."

<!-- Insert a picture of the source selected on headphones output -->

## Pro Tools

Now that DADman is properly set up, you can go ahead and open your Pro Tools session. 

### I/O
In Pro Tools, go to Setup>I/O. In the bottom left of the window that pops up, check "Apply to all tabs" and select "Import Settings." The correct I/O will be called "ERR_MAIN.pio"

<!-- image -->

### Routing

Now that the I/O is set up, all that's left to do is route your tracks to the proper output. For stereo, simply assign your output to "Output.Stereo". For surround, assign your output to "Output."

<!-- image -->