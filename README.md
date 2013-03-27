RGBDToolkit-to-Processing
=========================

Allows you to use RGBD Toolkit to capture a scene and then bring the SAME depth info into processing. This is useful for when two projects need to have identical takes/performances.

This sketch takes the PNG image sequence that comes out of RGBD Toolkit and converst it to (X,Y,Z) coordinates. All it is doing right now is creating a pointcloud, but you can change it to do pretty much anything.

Controls:<br />
o: open new folder<br />
up/down arrows: x-axis rotation<br />
left/right arrows: y-axis rotation<br />
w/s: forward/back<br />
a/d: left/right<br />
e/c: up/down<br />
</>: z cutoff<br />
numbers 1 - 9: adjust resolution<br />
SPACE: play/pause

i: toggle info<br />
h: toggle help<br />
r: reset view<br />
    


This does not (yet) take into account the geometric callibration done in RGBD Toolkit, although it seems to be just a matter of modifying the constants in the depthToWorld() function. If anyone wants to play around with this, let me know. I probably won't get to it until it becomes an issue in the project I'm working on.

Make sure you have a good amount of memory allocated for Processing in the preferences if you will be using very long image sequences. If you find that it keeps running out of memory, try pausing playback while you're moving the camera around, and then start it again when you find a good angle.

Feel free to improve the code and make changes. Let me know if you have any questions. I've included a sequence of PNGs so you can try the sketch out.

contact@ivaylogetov.com
