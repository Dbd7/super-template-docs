# Slot Reel Animation Type

There is 2 type of slot reel animation
- Sprite sheet animation
- Symbol blur image animation

# Sprite Sheet Animation

Sprite sheet animation using animation to create slot spining effect instead of symbol moving method.
It onyl apply to certain games only.

![](./res/sprite-sheet-reel-anim.jpg)

Make sure setup `SlotReelSpinAnim` animation first and enable `Slot Reel Spinning With Sprite Sheet`

# Slot Symbol Moving Animation

Slot symbol moving methond. The most common methond to create slot spinning effect.

![](./res/symbol-anim-01.jpg)

Deactivate `Slot Reel Spinning With Sprite Sheet` option. Super-Template default using slot symbol moving method.

![](./res/symbol-anim-02.jpg)

Enable `SlotReelStripPrefab` component for each slot reel. Please make sure *Normal Symbol* and *Blur Symbol* assets place in same SpritAtlas.