Operating the XY Plotter with MDraw
===================================

**Before you start: do you have the right drivers? You won’t see the
right comm port in mDraw if you don’t!**

**DO NOT CLICK THE ‘UPDATE FIRMWARE’ BUTTON AT ANY TIME IN THIS PROCESS! **

1.  Make sure the XY Plotter is turned off (black switch on mainboard)
    and the USB is unplugged

2.  Make sure that MDraw is not currently running

3.  Make sure that the dipswitches on the servo boards are ‘up’ (away
    from the ‘123’)

4.  Plug USB into computer (the pen holder should twitch – if it
    doesn’t, go to step 19)

5.  Turn XY Plotter on

6.  Start MDraw

7.  In top right drop-down in MDraw, select ‘XY’

8.  In the port section, select the appropriate serial port, then click
    ‘Connect’

    a.  If you get green number/letter pairs after the text ‘open
        success,’ you’re good to go on to the next steps. If not, go to
        step 19

    b.  The pen holder should twitch – if it doesn’t, go to step 19

9.  Click the gear in the upper right, make sure:

    a.  When you physical push the limit switch sensors on the XY
        Plotter, the ‘Limit Switch Status’ should change from 1 to 0 in
        the same order as indicated in the drawing

    b.  Yes, you need to do this *every* time

10. Make sure the width is set to 310 and the height to 360

    a.  Yes, you need to do this *every* time

11. Click the ‘Pen Up’ button. Pen should go up. If it doesn’t, go to
    step 19.

12. Click the ‘Pen Down’ button. Pen should go down. If it doesn’t, go
    to step 19.

13. Click the home button (it’s a house). Carriage should go to
    0x,0y co-ords. If it doesn’t, go to step 19

14. Click the ‘open file button (it’s a folder)

    a.  Choose a SVG or BMP file

15. Place and resize the image

16. Click the play button to start (it’s a triangle)

    a.  Push the pause button (two vertical lines) to pause during an
        image

    b.  Push the stop button (it’s a square) to stop printing (make sure
        to push ‘Pen Up’

17. Make sure you cap the pen/click it closed when you’re done

18. Yay! You did it!

19. PEN DOESN’T GO UP AND DOWN/COMMUNICATION TROUBLESHOOTING STEPS

    a.  Well, that sucks. Here’s what you need to try:

        i.  Shut down MDraw

        ii. Get the XYbot.ino Arduino sketch from this repo (don't grab the 'official' one; it has errors)

        iii. Load it up in the Arduino IDE

        iv. Make sure MDraw isn’t running

        v.  Compile and upload the sketch. Hope you have the right
            Arduino sketch!

        vi. For the pen: try unplugging the pen servo cable, and make
            sure that it’s plugged into the top of the pen servo
            board (slot2). Sometimes you have to give the white servo
            end a little ‘nudge’

        vii. Verify that all servo cables are plugged in/seated, the
            board is switched on, and that the power/USB cables are
            plugged in and in good shape


