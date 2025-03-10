# Incredibox V9CODE REMBUILD TEMPLATE
I only made today cuz rem didnt release the thing yet so uhhhhhhh

# THE GUIDE
I recommend using this site first then you can go back to this: https://boogoxseal.xyz/tools/appjs
![versionexamplev9code](https://github.com/user-attachments/assets/3c61c50a-1232-41e4-90c7-5a5f3f2cae7d)
can be found in the `js/apps.js` file

to change what version you want it on you can change the "versions.v1" to like "versions.v2", "versions.v3", "versions.v4" and so on all the way up to "versions.v9" unless if you want to add a custom version
that requires some css coding and stuff

# LOOPTIME AND TOTALFRAME ANIMATION MANAGEMENT
use this site https://joalor64gh.github.io/LooptimeFinder/ its a wip but its a really great tool to use cuz more was planned for it (only use it if you suck at doing looptimes like me!)

# FOR POLOS
![poloanimearrayexamplev9code](https://github.com/user-attachments/assets/818364f3-4eed-4a7a-9e2f-e2afc274d139)
can be found in the `js/apps.js` file

# FOR BONUSES
![bonusexamplev9code](https://github.com/user-attachments/assets/a67e339e-330e-42be-8501-bd2731867c5d)
can be found in the `js/apps.js` file



# TO CHANGE THE CHECKMARK COLOR
go to css/style.min.css and find the color
its "colV1:" and you can set it to anything like this for example colV1: "#84DCC6" which will change it
but you can set it to anything that fits that versions color

# TO ADD A NEW VERSION
go under the line of 297 and press enter and add this under it for example (change the number to whatever you want like if you want it on v2 change the number to 2) in the apps js file
   ```
   versions.v6 = { // ALIVE
  name: "Alive",
  version: "6",
  date: "2018",
  folder: "asset-v6/",
  looptime: 7111,
  bpm: 135,
  totalframe: 342,
  nbpolo: 7,
  bonusloopA: false,
  bonusendloopA: false,
  colBck: "#110521",
  col0: "#A07DFA",
  col1: "#825FD2",
  col2: "#5F3CA0",
  col3: "#371464",
  col4: "#230A41",
  animearray: [
    {
      name: "1_kick",
      color: "1e96be",
      uniqsnd: true,
    },
    {
      name: "2_snare",
      color: "1e96be",
      uniqsnd: true,
    },
    {
      name: "3_kanye",
      color: "1e96be",
      uniqsnd: true,
    },
    {
      name: "4_tuctuc",
      color: "1e96be",
      uniqsnd: true,
    },
    {
      name: "5_break",
      color: "1e96be",
      uniqsnd: true,
    },
    {
      name: "6_cribasse",
      color: "825fd2",
      uniqsnd: true,
    },
    {
      name: "7_distotut",
      color: "825fd2",
      uniqsnd: true,
    },
    {
      name: "8_screw",
      color: "825fd2",
      uniqsnd: true,
    },
    {
      name: "9_shaolin",
      color: "825fd2",
      uniqsnd: true,
    },
    {
      name: "10_shower",
      color: "825fd2",
      uniqsnd: true,
    },
    {
      name: "11_basse",
      color: "e11419",
      uniqsnd: true,
    },
    {
      name: "12_hou",
      color: "e11419",
      uniqsnd: true,
    },
    {
      name: "13_clav",
      color: "e11419",
      uniqsnd: true,
    },
    {
      name: "14_synth",
      color: "e11419",
      uniqsnd: true,
    },
    {
      name: "15_yah",
      color: "e11419",
      uniqsnd: true,
    },
    {
      name: "16_hurry",
      color: "f06400",
      uniqsnd: true,
    },
    {
      name: "17_good",
      color: "f06400",
      uniqsnd: true,
    },
    {
      name: "18_mind",
      color: "f06400",
      uniqsnd: true,
    },
    {
      name: "19_haha",
      color: "f06400",
      uniqsnd: true,
    },
    {
      name: "20_wow",
      color: "f06400",
      uniqsnd: true,
    },
  ],
  bonusarray: [
    {
      name: "Alive",
      src: "v6-b1-alive-hb",
      code: "4,6,9,14,18",
      sound: "bonus-alive",
      loop: 3,
    },
    {
      name: "Busta",
      src: "v6-b2-busta-hb",
      code: "1,2,8,11,16",
      sound: "bonus-busta",
      aspire: "aspire-busta",
      loop: 3,
    },
    {
      name: "VR",
      src: "v6-b3-vr-hb",
      code: "3,8,11,12,20",
      sound: "bonus-vr",
      aspire: "aspire-vr",
      loop: 3,
    },
  ],
};
   ```

# TO ADD A VERSION
something like this
``` 
<!--  
HOW TO USE IT:
• <line> category is used to create a new line (using more than 3 might cause issues)
• name="TEXT" is the name of the icon
• ID="NUMBER" is the ID of the icon
• color="#HEX" is the color of the title and checkmark
• locked="true/false" is the lock status of the icon, if its locked it will be impossible to open
• customName="true/false" if its enabled, it will use name of your version instead of the one from the switch-bt-title-tiny@2x.png
• customIcon="asset-v1/ICON.png" is the path to the icon, removing customIcon will use the default one from switch-bt-visu-1@2x.png
• hidden="true/false" if its enabled, it will hide the icon from the list
 -->

<icons>
  <line>
    <icon name="Template" ID="1" color="#666" locked="false" customName="true" customIcon="asset-v1/icon.png" hidden="false"></icon>
    <icon name="Example" ID="2" color="#666" locked="false" customName="true" customIcon="asset-v2/icon.png" hidden="false"></icon>
  </line>
</icons>
```

its a example but just use a text editor like notepad++ or VS Code it will be helpful editing how version you want!

# MAKE YOUR MOD SUPPORTED FOR IOS?
simple in the `js/script.min.js` file find the sndext = "ogg" and vidext = "webm" and change ogg to mp3 and webm to mp4 (BUT IT DOES REQUIRE YOU TO CONVERT STUFF) in build

# WHAT I RECOMMEND FOR CONVERTING (to make your mod have ios support)
for audio i recommend https://online-audio-converter.com/ the reason is because you dont have a limit used it before and it was great!

for video i recommend https://www.freeconvert.com/webm-to-mp4


# MAIN QUESTION FOR PORTING V8 CODED MODS TO V9?
will the !0 or the !1 work?
The answer to that is yes
But I highly still recommend putting the app js thru the vercel js site to get a more accurate result!
