# My New Project

Demo project for presentation at [Zlot Programistów Delphi 2024](https://www.bsc.com.pl/zlot-programistow-delphi-2024/).

Slides: https://castle-engine.io/zlot2024

Using [Castle Game Engine](https://castle-engine.io/).

## 3D assets credits and licenses

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