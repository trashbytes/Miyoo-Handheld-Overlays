# Immersive Handheld Overlays Collection for Onion OS on Miyoo Minis with 640x480 screens

The goal of this project is to make it look like classic handheld games are played on a screen with a matching resolution and aspect ratio. The bezels are not just decoration, they match the resolution, look and feel of the emulated system, as if they were rendered by that system. So it's not about creating a photorealistic replica but rather a subtle way to trick your brain into believing that you see physically larger pixels on a screen that perfectly matches the aspect ratio of the emulated system. Flat and jagged pixels get tranformed into a warm and inviting texture. It's not a scientific recreation, it's a nostalgic approximation with an immersive enhancement.

Scaling many different resolutions and aspect ratios to fit a 640x480 screen without artifacting and shimmering is not easy, but I think in the end I got there.

Color systems use a subtle pixel grid that gently shapes and approximates individual pixels. Monochrome LCD handheld systems use a different grid that hints at gaps between the LCD crystals.

The grid is intentionally subtle to avoid negatively affecting image quality while still adding a nostalgic feeling, as if you were playing on a low-resolution display. Lens shadows, rounded corners, and similar embellishments are intentionally omitted to keep the focus on pixel structure and enjoy the Miyoo Mini’s bright IPS display.

**Important note: In order to properly center squareish systems and to enable subpixel level precision at the edges, I've developed a new edge extension filter, which also replaces the previous offset filter for GBA, LYNX and WS. Instead of simply shifting the image up and down or side to side, this filter duplicates the rows and columns at the edges for seamless overlays even at pixel fractions. So for every system except for Game Gear, which is already 4:3, you have to apply both the overlay as well as the accompanying filter!**

## Supported devices

The table below summarizes which Miyoo models are compatible with these overlays.

| Device              | Resolution  | Supported  |
| ------------------- | ----------- | ---------- |
| **Miyoo Mini Plus** | **640x480** | **✔️ Yes** |
| **Miyoo Mini v1**   | **640x480** | **✔️ Yes** |
| **Miyoo Mini v2**   | **640x480** | **✔️ Yes** |
| **Miyoo Mini v3**   | **640x480** | **✔️ Yes** |
| **Miyoo Flip**      | **640x480** | **✔️ Yes** |
| **Miyoo Flip v2**   | **640x480** | **✔️ Yes** |
| **Miyoo A30**       | **640x480** | **✔️ Yes** |
| Miyoo Mini          | 750x560     | ❌ No      |
| Miyoo Mini v4       | 750x560     | ❌ No      |

## System specific overlays and settings

Save overrides per content directory!

### Mega Duck

![Immersive_MEGADUCK-Generic preview](RetroArch/.retroarch/overlay/MEGADUCK/Immersive_MEGADUCK-Generic-Preview.png?v=31)

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

### Supervision

![Immersive_SUPERVISION-Generic preview](RetroArch/.retroarch/overlay/SUPERVISION/Immersive_SUPERVISION-Generic-Preview.png?v=31)

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

![Immersive_GB-Generic preview](RetroArch/.retroarch/overlay/GB/Immersive_GB-Generic-Preview.png?v=31)

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

![Immersive_GBC-Generic preview](RetroArch/.retroarch/overlay/GBC/Immersive_GBC-Generic-Preview.png?v=31)

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

![Immersive_GG-Generic preview](RetroArch/.retroarch/overlay/GG/Immersive_GG-Generic-Preview.png?v=31)

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

![Immersive_NGP-Generic preview](RetroArch/.retroarch/overlay/NGP/Immersive_NGP-Generic-Preview.png?v=31)

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

### Lynx

![Immersive_LYNX-Generic preview](RetroArch/.retroarch/overlay/LYNX/Immersive_LYNX-Generic-Preview.png?v=31)

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

![Immersive_WS-Generic preview](RetroArch/.retroarch/overlay/WS/Immersive_WS-Generic-Preview.png?v=31)

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

![Immersive_GBA-Generic preview](RetroArch/.retroarch/overlay/GBA/Immersive_GBA-Generic-Preview.png?v=31)

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

![Immersive_NDS-Generic preview](Emu/NDS/resources/overlay/Immersive_NDS-Generic-Preview.png?v=31)

```text
Menu + Start
	Overlay: Immersive_NDS-Generic.png
```

### Pokemon Mini (POKE)

![Immersive_POKE-Generic preview](RetroArch/.retroarch/overlay/POKE/Immersive_POKE-Generic-Preview.png?v=31)

The Pokémon Mini overlay requires a unique approach. Due to the ultra-low resolution, a fully upscaled image results in gigantic pixels that quickly strain eyes and brain. Furthermore, games often place text and art right at the screen's edge. Because of generous padding around the physical display this wasn't an issue on original hardware, but scaling the image to the very edges of a modern retro handheld makes UI elements hard to parse.

To solve this, I opted for integer scaling. This slightly reduces the pixel size and leaves room for padding around the gameplay area. Finally, to achieve a softer, warmer feel, I added a very subtle layer of film grain. Without it, the chunky pixels look a bit too flat and digital.

Because of the much higher resolutions of the other LCD handhelds, namely GameBoy, MegaDuck and Supervision, I didn't treat them this way. Their pixel grid is fine enough and sprite placement rarely needs additional padding. The dimensions also don't allow for easy padding at consistent sizing anyway.

```text
Quick Menu
	On-Screen Overlay
		Display Overlay: On
		Overlay Preset: Immersive_POKE-Generic
Core Options
		LCD Filter: None
Settings
	Video
		Scaling
			Integer Scale: On
			Keep Aspect Ratio: On
		Image Interpolation: Bicubic
		Video Filter: Immersive_POKE
In-Game
	Adjust contrast for transitions to match the bezel
```

## Game specific overlays and settings

Save overrides per Game!

### Apotris (GBA)

![Immersive_GBA-Apotris preview](RetroArch/.retroarch/overlay/GBA/Immersive_GBA-Apotris-Preview.png?v=31)

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

![Immersive_GBC-Tetris-for-Chromatic preview](RetroArch/.retroarch/overlay/GBC/Immersive_GBC-Tetris-for-Chromatic-Preview.png?v=31)

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

As these are no handheld systems with fixed pixel displays, there is no pixel grid. Also most retro gaming systems designed for CRTs don't have a fixed resolution and were designed with a 4:3 aspect ratio in mind anyway, so it's easiest to just make them fullscreen and ignore overscans. The Sega Master System is letterboxed by design and thus needs either black bars or a bezel on a 4:3 screen, so I made one.

Save overrides per Content Directory!

### Sega Master System (MS)

![Immersive_MS-Cropped-Blanking preview](RetroArch/.retroarch/overlay/MS/Immersive_MS-Cropped-Blanking-Preview.png?v=31)

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

### Other 640x480 Handhelds (Generic)

These PNGs can technically be used with pretty much any 640x480 retro handheld, but they are specifically designed for how Retro Arch on Onion OS renders and scales the game. They are also designed to work with a custom filter which shifts, crops and extends the output so that it's placed in a very specific place on screen. If you have a different device or OS they will most likely be misaligned. If the offset filters are not compatible, please look for offset / crop functions or shaders for your OS and/or try to align them in a graphics software yourself by using a screenshot of the game taken on your device.

## Credits

These overlays were inspired by the work of u/1playerinsertcoin. His Perfect_SYSTEM overlays collection is phenomenal!

All pixel grids and bezels were created entirely by myself, except for the GBA grid. The GBA grid is a heavily modified version of Perfect_GBA by u/1playerinsertcoin, because it is exceptionally good.
