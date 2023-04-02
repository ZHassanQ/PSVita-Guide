Thanks to **[Princess of Sleeping]()** for making **[psp2wpp]()** 

psp2wpp (PS Vita background waveparam replacer) introductory tutorial
written by Havocking92, sorry if there will be mispell, english is not my native language.
Github site: https://github.com/Princess-of-Sleeping/psp2wpp
All credits and thanks to Princess-of-Sleeping.
I’ve put her pinky wave with my comments to archive with this document, i think it’s a good starting point for you. When you see number in it, it’s default value, and if you see„?“ in comment, that means i am unsure of definition that one 😊
Basics and preparation:
• Plugin can use partitions sd0:, host0: and ux0:, i will be using ux0: in this tutorial, as i am used to it.
• It overwrites PS Vita’s original 31 waveparams, with parameters it finds in the data/waveparams/ folder, looking for *.txt files with numbers from 0 to 30. For example, if you want to replace first wave, you need to make waveparam with path ux0:data/waveparams/0.txt.
• To reload wave you have two options, system restart or launch psp2wpp-reload. It can be found on github page.
• Plugin/LiveArea is somewhat „foolhardy“; if you make error in text file, it just don‘t load it after launching psp2wpp-reload, and will stay at last state, or loads original Vita wave after system restart (if you suspect that change you made in waveparam just don’t work, restart system, and if it loads original wave, you’ve made error in it).
• It can also add 32th „hidden“ wave, which i am using it as „work“ wave myself. This wave will be added before first original wave, so consider it as „-1“th wave (not sure if it can be targeted in theme .xml). This requires to place waveparam.txt to ux0:data/ and waveparam.bin (this is „backup“ wave containing Princess-of-Sleeping’s pink wave, system uses it if your waveparam somewhat fails to load. It can be found on github page) in same folder.
• LiveArea ‘s wave selecter icon of waveparam.txt will reloads after system restart.
Waveparam formatting:
• Do not remove/rename/move any parameters or definers. Use only numeric values. Single error breaks whole waveparam file!!
• There is always word „type“, which basically defines group of parameters under it.
• You can use commenting be using „#“ in two ways; on separate line and after value by at least one space.
• You can see my comments in Princess-of-Sleeping’s pink waveparam.txt that will come with this document, use them.
• You can use whole numbers or float falues with 6 decimal points (for ex. 0.534849)
• When defining color, RGBA float code array is used, red, green, blue, alpha (opacity of color, it does not work everywhere). It means you will find four lines for one parameter to define color. Great color picker i am using can be found on https://antongerdelan.net/colour/ . Here’s example of dark purple color:
set_value selecter[1].r 0.720 ​– sets red color
set_value selecter[1].g 0 ​​– sets green color
set_value selecter[1].b 0.980 ​– sets blue color
set_value selecter[1].a 1.000000 ​– sets alpha
• Every value can be float with 6 decimal points. Some values are accepted just in range from 0.000000 to 1.000000 (colors), some can be either negative and positive (position, rotation etc.), some values can be huge (for example wind_speed)
• When editing rotation, keep in mind it uses numbers from -1.000000 to 1.000000 are like saying -360 degree to 360 degree, but you can use either value -3.1415, it will just go around. For example if you want to rotate wave axis by full 180 degree, you have to write 0.5.
 
Editing LiveArea’s wave selecter icon:
Look for first parameter group Select, it will look like this:
type Select
#selecter[0] is bottom color
set_value selecter[0].r 1
set_value selecter[0].g 0
set_value selecter[0].b 0
set_value selecter[0].a 1
set_value selecter[1].r 1
set_value selecter[1].g 1
set_value selecter[1].b 1
set_value selecter[1].a 1
 
selecter[0] defines color of bottom wave, and selecter[1] defines color of top wave. Alpha can be used here.
 
Understanding wave scene:
Here you can see my modified wave.
Every scene contains sky which can have two colors which you can see is yellow and red, defined by zenith and horizon parameters and it also contains sun, which is basically source of light that is also slightly affecting bubbles of LiveArea. Then you can see white wave, which is surrounded by green fog, which can have it’s own light source.
Group​​​Behavior
 
type Select​​​icon colors in LiveArea’s wave selecter
 
type Material​wave color and it’s behavior on light ( mostly reflection)
 
type PointLightSphere​source of light on wave
 
type Fog1​probably second fog, but i don’t see any changes in scene
 
type Fog0​fog surrounding wave, can also emmits it’s own light in center
 
type Sky​sky wave above wave, have two separate parts zenith and horizon. Can also change shape, animation. It also contains sun, it’s own light source.
 
type FFTWave​modifies physical behavior of sky and wave. Influences distortions of sky, waving of wave.
 
type WaveInstance​modifies position, rotation, scale and whole other things of wave
 
type WaveRenderer​should be settings for camera of scene, doesn’t seem to do anything right now
 
 
 
 
 
 
 
Few tips from „pro“ :D
 
My method for quick parameter change is to place psp2wpp-reload app on page, which have set waveparam.txt (-1th wave) as background, open up Vitashell with waveparam.txt, make change, save, keep vitashell opened in folder ux0:data/, just swipe to left to page, open psp2wpp-reload and see what i did.
 
Also there is list of parameters which absolutely affects animation of sky and wave:
 
type Sky:
pos_distortion_scale, grad_distortion_scale, horizon_distortion_scale, horizon_curvature
 
type WaveInstance:
distortion_scale, uv_scale, uv_rotate
 
type FFTWave:
gravity, logA, patch_size
 
 
 
Last word from me:
This is so far what i’ve found out in those tens of hours, you need to try it yourself to understand how to make fine waves, sometimes Sky or Wave will disappear, try to remember what value was there before and change it back or make smaller change.
I hope someone smarter than me will make PS Vita app with sliders or just text boxes and descriptions to make it more user friendly.
