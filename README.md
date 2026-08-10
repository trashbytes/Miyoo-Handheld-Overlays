# Immersive Handheld Overlays Collection

The goal of this project is to make it look like classic handheld games are played on a screen with a matching resolution and aspect ratio. The bezels are not just decoration, they match the resolution, look and feel of the emulated system, as if they were rendered by that system. So it's not about creating a photorealistic replica but rather a subtle way to trick your brain into believing that you see physically larger pixels on a screen that perfectly matches the aspect ratio of the emulated system. Flat and jagged pixels get tranformed into a warm and inviting texture. It's not a scientific recreation, it's a nostalgic approximation with an immersive enhancement.

Scaling many different resolutions and aspect ratios to fit a 640x480 screen without artifacting and shimmering is not easy, but I think in the end I got there.

Color systems use a subtle pixel grid that gently shapes and approximates individual pixels. Monochrome LCD handheld systems use a different grid that hints at gaps between the LCD crystals.

The grid is intentionally subtle to avoid negatively affecting image quality while still adding a nostalgic feeling, as if you were playing on a low-resolution display. Lens shadows, rounded corners, and similar embellishments are intentionally omitted to keep the focus on pixel structure and enjoy the Miyoo Mini’s bright IPS display.

**Important note: In order to properly center squareish systems and to enable subpixel level precision at the edges, I've developed a new edge extension filter, which also replaces the previous offset filter for GBA, LYNX and WS. Instead of simply shifting the image up and down or side to side, this filter duplicates the rows and columns at the edges for seamless overlays even at pixel fractions. So for every system except for Game Gear, which is already 4:3, you have to apply both the overlay as well as the accompanying filter!**

## Supported devices

The overlays and filters are specifically designed for Miyoo devices with 640x480 screens running the latest Onion OS. They are not designed to work with other devices and screens, but may work (in part) with other OSes.

| Device              | Resolution  | Operating System | Supported  |
| ------------------- | ----------- | ---------------- | ---------- |
| **Miyoo Mini Plus** | **640x480** | **Onion OS**     | **✔️ Yes** |
| **Miyoo Mini v1**   | **640x480** | **Onion OS**     | **✔️ Yes** |
| **Miyoo Mini v2**   | **640x480** | **Onion OS**     | **✔️ Yes** |
| **Miyoo Mini v3**   | **640x480** | **Onion OS**     | **✔️ Yes** |
| Miyoo Flip          | 640x480     | any              | ⭕ Maybe   |
| Miyoo Flip v2       | 640x480     | any              | ⭕ Maybe   |
| Miyoo A30           | 640x480     | any              | ⭕ Maybe   |
| Miyoo Mini Flip     | 750x560     | any              | ❌ No      |
| Miyoo Mini v4       | 750x560     | any              | ❌ No      |

## System specific overlays and settings

Save overrides per content directory!

### Mega Duck (MEGADUCK)

![Immersive_MEGADUCK-Generic preview](RetroArch/.retroarch/overlay/MEGADUCK/Immersive_MEGADUCK-Generic-Preview.png?v=34)

```text
Quick Menu
	On-Screen Overlay
		Display Overlay: On
		Overlay Preset: Immersive_MEGADUCK-Generic
Settings
	Video
		Scaling
			Integer Scale: Off
			Keep Aspect Ratio: On
		Image Interpolation: Bicubic
		Video Filter: Immersive_MEGADUCK
```

### Supervision (SUPERVISION)

![Immersive_SUPERVISION-Generic preview](RetroArch/.retroarch/overlay/SUPERVISION/Immersive_SUPERVISION-Generic-Preview.png?v=34)

```text
Quick Menu
	On-Screen Overlay
		Display Overlay: On
		Overlay Preset: Immersive_SUPERVISION-Generic
	Core Options
		Internal Palette: Game Boy Pocket
Settings
	Video
		Scaling
			Integer Scale: Off
			Keep Aspect Ratio: On
		Image Interpolation: Bicubic
		Video Filter: Immersive_SUPERVISION
```

### Game Boy (GB)

![Immersive_GB-Generic preview](RetroArch/.retroarch/overlay/GB/Immersive_GB-Generic-Preview.png?v=34)

```text
Quick Menu
	On-Screen Overlay
		Display Overlay: On
		Overlay Preset: Immersive_GB-Generic
	Core Options
		GB Colorization: internal / use color categories
		Current category color for palettes: Nintendo Official
		 > Color Categories
			Nintendo Official: GB - Pocket
		Emulated Hardware (Restart Required): GB
Settings
	Video
		Scaling
			Integer Scale: Off
			Keep Aspect Ratio: On
		Image Interpolation: Bicubic
		Video Filter: Immersive_GB
```

### Game Boy Color (GBC)

![Immersive_GBC-Generic preview](RetroArch/.retroarch/overlay/GBC/Immersive_GBC-Generic-Preview.png?v=34)

```text
Quick Menu
	On-Screen Overlay
		Display Overlay: On
		Overlay Preset: Immersive_GBC-Generic
Settings
	Video
		Scaling
			Integer Scale: Off
			Keep Aspect Ratio: On
		Image Interpolation: Bicubic
		Video Filter: Immersive_GBC
```

### Game Gear (GG)

![Immersive_GG-Generic preview](RetroArch/.retroarch/overlay/GG/Immersive_GG-Generic-Preview.png?v=34)

```text
Quick Menu
	On-Screen Overlay
		Display Overlay: On
		Overlay Preset: Immersive_GG-Generic
Settings
	Video
		Scaling
			Integer Scale: Off
			Keep Aspect Ratio: Off
		Image Interpolation: Bicubic
```

### Neo Geo Pocket (NGP)

![Immersive_NGP-Generic preview](RetroArch/.retroarch/overlay/NGP/Immersive_NGP-Generic-Preview.png?v=34)

```text
Quick Menu
	On-Screen Overlay
		Display Overlay: On
		Overlay Preset: Immersive_NGP-Generic
Settings
	Video
		Scaling
			Integer Scale: Off
			Keep Aspect Ratio: On
		Image Interpolation: Bicubic
		Video Filter: Immersive_NGP
```

### Lynx (LYNX)

![Immersive_LYNX-Generic preview](RetroArch/.retroarch/overlay/LYNX/Immersive_LYNX-Generic-Preview.png?v=34)

```text
Quick Menu
	On-Screen Overlay
		Display Overlay: On
		Overlay Preset: Immersive_LYNX-Generic
Settings
	Video
		Scaling
			Integer Scale: Off
			Keep Aspect Ratio: On
		Image Interpolation: Bicubic
		Video Filter: Immersive_LYNX
```

### WonderSwan (WS)

![Immersive_WS-Generic preview](RetroArch/.retroarch/overlay/WS/Immersive_WS-Generic-Preview.png?v=34)

```text
Quick Menu
	On-Screen Overlay
		Display Overlay: On
		Overlay Preset: Immersive_WS-Generic
Settings
	Video
		Scaling
			Integer Scale: Off
			Keep Aspect Ratio: On
		Image Interpolation: Bicubic
		Video Filter: Immersive_WS
```

### Game Boy Advance (GBA)

![Immersive_GBA-Generic preview](RetroArch/.retroarch/overlay/GBA/Immersive_GBA-Generic-Preview.png?v=34)

```text
Quick Menu
	On-Screen Overlay
		Display Overlay: On
		Overlay Preset: Immersive_GBA-Generic
Settings
	Video
		Scaling
			Integer Scale: Off
			Keep Aspect Ratio: On
		Image Interpolation: Bicubic
		Video Filter: Immersive_GBA
```

### Nintendo DS (NDS)

![Immersive_NDS-Generic preview](Emu/NDS/resources/overlay/Immersive_NDS-Generic-Preview.png?v=34)

```text
Menu + Start
	Overlay: Immersive_NDS-Generic.png
```

### Pokemon Mini (POKE)

![Immersive_POKE-Generic preview](RetroArch/.retroarch/overlay/POKE/Immersive_POKE-Generic-Preview.png?v=34)

```text
Quick Menu
	On-Screen Overlay
		Display Overlay: On
		Overlay Preset: Immersive_POKE-Generic
Core Options
    Video Scale (Restart): 1x
Settings
	Video
		Scaling
			Integer Scale: Off
			Keep Aspect Ratio: On
		Image Interpolation: Nearest Neighbor
		Video Filter: Immersive_POKE
In-Game
	Adjust contrast for transitions to match the bezel
```

## Game specific overlays and settings

Save overrides per Game!

### Apotris (GBA)

![Immersive_GBA-Apotris preview](RetroArch/.retroarch/overlay/GBA/Immersive_GBA-Apotris-Preview.png?v=34)

```text
Quick Menu
	On-Screen Overlay
		Display Overlay: On
		Overlay Preset: Immersive_GBA-Apotris
Settings
	Video
		Scaling
			Integer Scale: On
			Keep Aspect Ratio: On
		Image Interpolation: Nearest Neighbor
		Video Filter: Immersive_GBA-Apotris
In-Game
	Settings
		Graphics
			Aspect Ratio: 4:3
```

### Tetris for Chromatic (GBC)

![Immersive_GBC-Tetris-for-Chromatic preview](RetroArch/.retroarch/overlay/GBC/Immersive_GBC-Tetris-for-Chromatic-Preview.png?v=34)

```text
Quick Menu
	On-Screen Overlay
		Display Overlay: On
		Overlay Preset: Immersive_GBC-Tetris-for-Chromatic
Settings
	Video
		Scaling
			Integer Scale: Off
			Keep Aspect Ratio: On
		Image Interpolation: Bicubic
		Video Filter: Immersive_GBC
```

## Other systems

As these are no handheld systems with fixed pixel displays, there is no pixel grid. Also most retro gaming systems designed for CRTs don't have a fixed resolution and were designed with a 4:3 aspect ratio in mind anyway, so it's easiest to just make them fullscreen and be done with it. On most systems overlays just can't work anyway due to the fact that a PNG file is static, but the resolution of the system may be not and while filters would technically work, any but the simplest ones are very resource intensive and most also don't look great due to scaling artifacts.

With that in mind there is at least one system where it does make sense. The Sega Master System is letterboxed by design and thus needs either black bars or a bezel on a 4:3 screen. Luckily it also has a (mostly) fixed resolution.

Save overrides per Content Directory!

### Sega Master System (MS)

![Immersive_MS-Cropped-Blanking preview](RetroArch/.retroarch/overlay/MS/Immersive_MS-Cropped-Blanking-Preview.png?v=34)

```text
Quick Menu
	On-Screen Overlay
		Display Overlay: On
		Overlay Preset: Immersive_MS-Cropped-Blanking
Settings
	Video
		Scaling
			Integer Scale: off
			Keep Aspect Ratio: off
		Image Interpolation: Bicubic
		Video Filter: Immersive_MS-Cropped-Blanking
```

This is the "Cropped-Blanking" variant, which I suggest you use as the default. Only a few games ever meaningfully use the blanking area and for those which do you can set the "Generic" variant as an override per game. Keep in mind that later versions of the system offer two additional resolutions at 224p and 240p, but they are rarely used. These overlays are made for the standard 192p system and games.

## Installation

### Miyoo handhelds running Onion OS

1. Copy the `RetroArch` and `Emu` folders from this repository to your SD card root and merge it with the existing folders.
2. On the device, open a game, then the Quick Menu and configure RetroArch as described below each preview.
3. If neccessary configure the game as described below the preview.
4. Don't forget to save the override for Content Directory or Game, depending on the overlay

### Other handhelds or opererating systems

These PNGs can technically be used with pretty much any 640x480 retro handheld, but they are specifically designed for how Retro Arch on Onion OS renders and scales the game. They are also designed to work with a custom filter which shifts, crops and extends the output so that it's placed in a very specific place on screen. If you have a different device or OS they will most likely be misaligned.

However, if they are not compatible with your device or OS you can create finetuned custom versions yourself for any resolution. Or just make different ones at 640x480px for Onion OS and share them!

## Make your own (at any resolution!)

### Generator script

I've included the generator script as well as all of my assets at their native resolution so you can create immersive overlays for any target resolution.

### Required files and folders

```text

Minimal setup for any given system.
This will just use the overlay-<width>x<height>.png file to create an overlay for the target resolution.
You can create a high-res grid for the system and it will be scaled to the target resolution, though a handcrafted grid manually optimized for the target resolution may give you better results.

SYSTEM/                                      # system folder, this is where the generated overlays will be stored
├── assets/                                  # assets folder, this is where json config and graphic assets will be stored
│   ├── compose-<width>x<height>.json        # default compose config for this system at this target resolution
│   ├── overlay-<width>x<height>.png         # default overlay image (like a grid for example) for this system at this target resolution
│   ├── screenshot-<width>x<height>.png      # default clean screenshot image for this system at this target resolution

The real fun begins when you add your own Variant folder and make use of individual assets to create your bezels.
Assets should be created at their native resolution and cover either the full width, the full height or both dimensions of the native system resolution. So for example a left bezel for GB or GBC would simply be 16x144px. Prescaling, downscaling, squishing, stretching and pixel perfect placement will then be done by the generator script. This means iterating is super fast, as you don't have to worry about doing all this manually and for every resolution or aspect ratio after each change, simply delete the .cfg file or -Overlay.png an run the script again.
You only have to setup the compose.json once and can create as many bezels at their native resolution as you want and they will be scaled and placed perfectly every time.
A "Generic" variant directory will be created, should it not exist.

│   └── <Variant-Name>/                      # optional variant folder
│       ├── compose-<width>x<height>.json    # optional override compose config for this variant
│       ├── overlay-<width>x<height>.png     # optional override overlay image (like a grid for example) for this variant
│       ├── screenshot-<width>x<height>.png  # optional override clean screenshot image for this variant
│       └── <Asset-Name>.png                 # optional graphic assets like bezels and logos, see explanation for compose.json below
```

You can also omit the resolution on both `overlay.png` as well as `screenshot.png` and it will be used for all resolutions if no override file is present.

### compose-&lt;width&gt;x&lt;height&gt;.json

This must be a valid JSON file, even if you don't have a bezel or grid. Add a key for every asset you want to place, you can use the following paramters for each one:

- `prescale`: prescale the asset (for example `800%` or `300%`), default: `800%`
- `prefilter`: choose the filter used for the prescale step (for example `Point`, `Catrom`, `Lanczos`), default: `Point`
- `scalex`, `scaley`: scale the asset horizontally and/or vertically after prescaling to get non-square pixels (for example `1.0`, `0.8`), default: `1`
- `filter`: choose the scaling filter used for the final resize (for example `Catrom`, `Lanczos`, `Point`), default: `Catrom`
- `gravity`: choose where to place the asset on the canvas (for example `Center`, `NorthWest`, `South`, `East`), default: `NorthWest`
- `left`, `right`, `up`, `down`: offset the asset relative to the chosen gravity by native pixels for finetuning, default: `0`

Example: `GBA/assets/compose-640x480.json`

```json
{
  "bezel.png": {
    "gravity": "South"
  }
}
```

Will place the `bezel.png` asset at the bottom of the screen.

## Credits

These overlays were inspired by the work of u/1playerinsertcoin. His Perfect_SYSTEM overlays collection is phenomenal!

All pixel grids and bezels were created entirely by myself, except for the GBA grid. The GBA grid is a heavily modified version of Perfect_GBA by u/1playerinsertcoin, because it is exceptionally good.
