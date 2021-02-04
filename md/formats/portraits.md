# Portraits

Portraits refer to large character used throughout the game, notably:

- **Battle Portraits** - Portraits used in the battle mode character select. The lowest resolution weighing in at 80px x 64px resolution. 16 colours.

- **Story Portraits** - Portraits used throughout story mode. These are a bit larger, weighing in at 96px x 96px. 16 colours.

## Editting

It is recommended to edit portraits with [GBAGE](?a=tools/gbage)'s compressed graphics editor. GBAGE has tools to repoint your portraits if they end up larger than the in-game ones and also their palettes if they also end up larger, alongside a relatively intuitive interface.

## Battle Portraits

<p align="center">
    <img src="res/formats/portraitBattle1.png">
    <br>
    <img src="res/formats/portraitBattle2.png">
    <br>
    <i>Knuckles' portrait as it appears in-game and as it is stored in the ROM.</i>
</p>

Battle portraits in game display as 80x64, however are stored as 64x80, with the last two tiles of each row being moved into the bottom of the image in a pattern of ``1, 2, 3, 4`` ``5, 6, 7, 8``.

They are sprite indexes 28 - 35 in GBAGE.

It is worth noting that in-game there is quite a few oppurtunities for the image to be cut off:

<p align="center">
    <img src="res/formats/portraitBattleSafe.png">
    <br>
    <i>Areas where the battle portrait can be cut off. Rule will cut off the top if selected by Player 2, arrows will cut off if it's currently being selected and the striped area will cutoff if it's on the right side of the screen.</i>
</p>

For custom battle portraits, it's recommended that they keep the white outline and that if required they cut off around the selection box.

<p align="center">
    <img src="res/formats/portraitBattleCut.png">
    <br>
    <i>Selection box cutoff demonstrated by Emerl's portrait.</i>
</p>

## Story Portraits

<p align="center">
    <img src="res/portraits/eggman.png">
    <br>
    <img src="res/formats/portraitStory.png">
    <br>
    <i>Eggman's portrait as it appears in-game and as it is stored in the ROM.</i>
</p>

Battle portraits in game display as 96x96, however are stored as 64x144, with the last four tiles of each row being moved into the bottom of the image in a pattern of ``1, 2`` ``3, 4`` ``5, 6`` ``7, 8`` ``9, 10`` ``11, 12``.

They are sprite indexes 399 - 431 in GBAGE.