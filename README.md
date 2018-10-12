# hisGhost
A-Frame Web VR Project based around grief, loss and anger.

CREDIT
Created in A-Frame
Voice Actor: Emily Rigaux
Voice Recording: Dan Sequiera
Music and Amalgamation of Code: Autrea


LIBRARIES USED
A-Frame

aframe.min.js
source: https://aframe.io/
cnd: https://aframe.io/releases/0.8.2/aframe.min.js

aframe-text-geometry-component.min.js
source: https://www.npmjs.com/package/aframe-text-geometry-component
cdn: https://unpkg.com/aframe-text-geometry-component@^0.5.0/dist/aframe-text-geometry-component.min.js


PROGRAMS USED
3D assets created in Sculptris, polycount decimated in Blender, exported as .obj
Voice recording done in Pro Tools, exported as .wav
Music composition done in FL Studios, exported as .wav


PROCESS AND HICCUPS ALONG THE WAY
1) HICCUP: I attempted to have multiple <a-scene> tags, but A-Frame does not allow for multiple <a-scene> tags in one project;
  
2) HICCUP: To get around problem 1, I attempted to write all of the info through a .js file by targeting the <a-scene> with .innerHTML;
   However, when the <a-assets> tag was rewritten, the .obj assets that were previously loaded had no container and caused an error;
   
3) HICCUP: My next attempt was to use <iframe> to organize each scene and call them when needed, but this caused removed the WebVR controls for mobile;
  
4) HICCUP: I resorted to having one scene with all of the objects already placed in the world, with the camera and lighting animating throughout the experience, but this also did not work on mobile. The camera would only move on desktop.

5) SOLVED: Final solution was to have the camera and lighting stationary with the assets in the scene moving at a steady pace into and out of the lighting to give the illusion of the camera being moved.

6) SOLVED: With Chrome's recent change to how sound is allowed to be played, it causes the soundtrack to be mute in the browser. For now, using an alternate browser is required. I've been using Firefox.
