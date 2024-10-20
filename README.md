# Test Game Using Blender, Sketchfab, Quaternius, TCastleMoveAttack

Demo project for presentation at [Zlot Programistów Delphi 2024](https://www.bsc.com.pl/zlot-programistow-delphi-2024/).

Slides (in Polish): https://castle-engine.io/zlot2024 .

## Features

This demonstrates creating a simple 3D FPS game, from start to finish. The level, creatures, and win/lose views have been done using:

- [Castle Game Engine editor](https://castle-engine.io/editor)

- [Blender](https://castle-engine.io/blender) (to design base level geometry)

- [Sketchfab](https://castle-engine.io/sketchfab) (to add additional props to the level)

- [Quaternius models](https://quaternius.com/) (to add animated enemies)

- `TCastleMoveAttack` (for ready logic of moving enemies and player hit points),

- `TCastleWalkNavigation` (for ready handling of AWSD and similar keys, typical for FPS games).

The Pascal code (most in `GameViewMain` unit) adds logic to

- Activate _mouse look_ when right mouse button is pressed,

- Show "game win" view when player reaches a certain place in the level,

- Show "game over (lost)" view when player life drops to zero,

- Show player life (hit points),

- Shoot enemy on mouse click.

## Note: Requires Castle Game Engine walk-attack-behavior branch (with TCastleMoveAttack)

Temporary note:

To use this, you need a [Castle Game Engine](https://castle-engine.io/) version with `TCastleMoveAttack` component. This is not yet part of the engine _master_ branch, it's a work in progress, available on [walk-attack-behavior branch](https://github.com/castle-engine/castle-engine/tree/walk-attack-behavior).

Watch out [Castle Game Engine news](https://castle-engine.io/wp/) to know when it will be merged!

Until then, you can get engine branch `walk-attack-behavior` using GIT and [compile it yourself](https://castle-engine.io/compiling_from_source.php) if you're brave :) Contact `michalis@castle-engine.io` if you have questions.

## Screenshots

![Level design in Blender](screenshots/level_blender.png)
![Level design in Blender and Castle Game Engine](screenshots/level_blender_cge_1.png)
![Level design in Blender and Castle Game Engine](screenshots/level_blender_cge_2.png)

![Run designed game](screenshots/level_blender_cge_run.png)

![Adding Sketchab assets 1](screenshots/level_sketchfab_1.png)
![Adding Sketchab assets 2](screenshots/level_sketchfab_2.png)

![Game win](screenshots/win.png)

## 3D assets credits and licenses

Using [Castle Game Engine](https://castle-engine.io/).

- Dungeon based on https://opengameart.org/content/3d-castle-dungeon-tileset-extended nby [rubberduck](https://opengameart.org/users/rubberduck)

    This is in turn using other assets, see `data-source/original_dungeon-tileset-extended/readme.txt` for details.

- Trophy from https://opengameart.org/content/trophy by [JeremyWoods](https://opengameart.org/users/jeremywoods) (license: CC0).

- Multiple [Sketchfab](https://sketchfab.com/features/gltf) models, see `data/sketchfab` for details and links to authors. Licenses are a mix of _Creative Commons Attribution_ and _Creative Commons Attribution NonCommercial_ licenses.

- Skeleton from [Quaternius Pirate Kit](https://quaternius.com/packs/piratekit.html), CC0.

## Building

Compile by:

- [CGE editor](https://castle-engine.io/editor). Just use menu items _"Compile"_ or _"Compile And Run"_.

- Or use [CGE command-line build tool](https://castle-engine.io/build_tool). Run `castle-engine compile` in this directory.

- Or use [Lazarus](https://www.lazarus-ide.org/). Open in Lazarus `game_3d_standalone.lpi` file and compile / run from Lazarus. Make sure to first register [CGE Lazarus packages](https://castle-engine.io/lazarus).

- Or use [Delphi](https://www.embarcadero.com/products/Delphi). Open in Delphi `game_3d_standalone.dproj` file and compile / run from Delphi. See [CGE and Delphi](https://castle-engine.io/delphi) documentation for details.