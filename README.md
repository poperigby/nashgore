# Nash's Gore Mod: Vengeance Edition
Version: 1.0<br/>
Requires: GZDoom 4.1.3 or higher<br/>
Official forum thread: https://forum.zdoom.org/viewtopic.php?f=46&t=62641<br/>
Github: https://github.com/nashmuhandes/nashgore<br/>

### Load Order

Please load nashgore.pk3 last (or fairly late) in your load order, to ensure
that no other mod overrides NGM's content.

### Options

Most of the effects in Nash's Gore Mod can be customized. Please visit
the Options menu for more details.

### Special Lump: BLUDTYPE

Nash's Gore Mod introduces a new special lump called BLUDTYPE. You can simply
create a BLUDTYPE.txt and load it after NGM; the lumps will stack.

For example: gzdoom.exe -file nashgore.pk3 bludtype.txt

The BLUDTYPE lump is used to list blood actor classes to override. For
example, Smooth Doom changes the Cacodemon blood type to "Blueblood", which
causes NGM's blood to never appear. To fix that, simply add "BlueBlood"
on a new line into BLUDTYPE.txt.

USAGE: Simply list down blood Actor classes you wish to override, each on a
new line.

A sample BLUDTYPE.txt for Smooth Doom:

```
XBlood
BlueBlood
GreenBlood
```

### Know Issues/TODO List

- Heretic Knight's axe spawns blood (A_DripBlood)
- Crushed/squishy gibs probably don't work correctly with crushing polyobjs
- Ice chunks might get stuck inside solid objects
- When frozen enemies automatically shatter, gibs will not appear
- Wall decals do not look the same as floor blood splats. The reason for this
  is that wall decals cannot be opaque, they can only be shaded with a single
  colour. Fixing this would require GZDoom to implement translatable opaque
  wall decals.

### Credits

Nash's Gore Mod: Vengeance Edition<br/>
© 2006 - 2019 Nash Muhandes

All graphics, sprites and code by Nash Muhandes<br/>
Slope alignment method by ZZYZX<br/>
Sounds by various FreeSound contributors (see below)<br/>
Audio mixed and mastered by Nash Muhandes

Special thanks:

Marisa Heit<br/>
Graf Zahl<br/>
Rachael<br/>
dpJudas<br/>
Gutawer<br/>
phantombeta<br/>
ZZYZX<br/>
Marisa Kirisame<br/>
Caligari87<br/>
Namsan<br/>
m8f<br/>

Sound sources:

https://freesound.org/people/LittleRobotSoundFactory/sounds/270481/
https://freesound.org/people/altfuture/sounds/174634/
https://freesound.org/people/cliftonmcarlson/sounds/345985/
https://freesound.org/people/deoking/sounds/411671/
https://freesound.org/people/Rock%20Savage/sounds/81042/
https://freesound.org/people/altfuture/sounds/174637/
https://freesound.org/people/mattiagreyfox/sounds/202400/
https://freesound.org/people/Hitrison/sounds/251411/
https://freesound.org/people/Hitrison/sounds/251410/
https://freesound.org/people/nicktermer/sounds/259542/
https://freesound.org/people/saturdaysoundguy/sounds/388033/
https://freesound.org/people/LittleRobotSoundFactory/sounds/316534/
https://freesound.org/people/MWLANDI/sounds/85863/
https://freesound.org/people/jvitorml/sounds/393736/
https://freesound.org/people/janbezouska/sounds/399183/

MODDERS:

Feel free to include Nash's Gore Mod in your projects, as long as I am given
credit for it. You must include this text file in your mod. Headers in all
ZScript files must remain intact.

YOU MUST CREDIT "NASH MUHANDES" IF ANY OF MY GRAPHICS OR SPRITES ARE USED
IN YOUR MOD! They are original artwork, please respect my hustle!

You don't need to ask for my permission to embed NGM into your
projects! Happy modding!
