# Immersive Handheld Overlays Collection for Onion OS on Miyoo Mini

The goal of this project is to make it look like classic handheld games are played on a screen with a matching resolution and aspect ratio. The bezels are not just decoration, they match the resolution, look and feel of the emulated system, as if they were rendered by that system. So it's not about creating a photorealistic replica but rather a subtle way to trick your brain into believing that you see physically larger pixels on a screen that perfectly matches the aspect ratio of the emulated system. Flat and jagged pixels get tranformed into a warm and inviting texture. It's not a scientific recreation, it's a nostalgic approximation with an immersive enhancement.

Scaling many different resolutions and aspect ratios to fit a 640x480 screen without artifacting and shimmering is not easy, but I think in the end I got there.

Color systems use a subtle pixel grid that gently shapes and approximates individual pixels. Monochrome LCD handheld systems use a different grid that hints at gaps between the LCD crystals.

The grid is intentionally subtle to avoid negatively affecting image quality while still adding a nostalgic feeling, as if you were playing on a low-resolution display. Lens shadows, rounded corners, and similar embellishments are intentionally omitted to keep the focus on pixel structure and enjoy the Miyoo Mini’s bright IPS display.

## System specific overlays and settings

Save overrides per content directory!

### Mega Duck

![Immersive_MEGADUCK-Generic preview](RetroArch/.retroarch/overlay/MEGADUCK/Immersive_MEGADUCK-Generic_Preview.png?v=25)

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
```

### Supervision

![Immersive_SUPERVISION-Generic preview](RetroArch/.retroarch/overlay/SUPERVISION/Immersive_SUPERVISION-Generic_Preview.png?v=25)

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
```

### Game Boy (GB)

![Immersive_GB-Generic preview](RetroArch/.retroarch/overlay/GB/Immersive_GB-Generic_Preview.png?v=25)

Note: GB and GBC aren't centered on screen. They are shifted to the left by a few pixels. To visually balance that quirk the overlay has 3 pixels of transparency on the right hand side, which will be black on device.

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
```

### Game Boy Color (GBC)

![Immersive_GBC-Generic preview](RetroArch/.retroarch/overlay/GBC/Immersive_GBC-Generic_Preview.png?v=25)

Note: GB and GBC aren't centered on screen. They are shifted to the left by a few pixels. To visually balance that quirk the overlay has 3 pixels of transparency on the right hand side, which will be black on device.

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
```

### Game Gear (GG)

![Immersive_GG-Generic preview](RetroArch/.retroarch/overlay/GG/Immersive_GG-Generic_Preview.png?v=25)

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

![Immersive_NGP-Generic preview](RetroArch/.retroarch/overlay/NGP/Immersive_NGP-Generic_Preview.png?v=25)

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
```

### Lynx

![Immersive_LYNX-Generic preview](RetroArch/.retroarch/overlay/LYNX/Immersive_LYNX-Generic_Preview.png?v=25)

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
		Video Filter: Immersive_LYNX (or any other way to offset up for 9px)
```

### WonderSwan (WS)

![Immersive_WS-Generic preview](RetroArch/.retroarch/overlay/WS/Immersive_WS-Generic_Preview.png?v=25)

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
		Video Filter: Immersive_WS (or any other way to offset up for 12px)
```

### Game Boy Advance (GBA)

![Immersive_GBA-Generic preview](RetroArch/.retroarch/overlay/GBA/Immersive_GBA-Generic_Preview.png?v=25)

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
		Video Filter: Immersive_GBA (or any other way to offset up for 10px)
```

### Nintendo DS (NDS)

![Immersive_NDS-Generic preview](Emu/NDS/resources/overlay/Immersive_NDS-Generic-Preview.png?v=25)

```text
Menu + Start
	Overlay: Immersive_NDS-Generic.png
```

### Pokemon Mini (POKE)

![Immersive_POKE preview](RetroArch/.retroarch/overlay/POKE/Immersive_POKE_Preview.png?v=25)

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
		Video Filter: Immersive_POKE (or any other way to offset up for 16px)
In-Game
	Adjust contrast for transitions to match the bezel
```

## Game specific overlays and settings

Save overrides per Game!

### Apotris (GBA)

![Immersive_GBA-Apotris preview](RetroArch/.retroarch/overlay/GBA/Immersive_GBA-Apotris_Preview.png?v=25)

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

## Installation

### Miyoo Mini / Miyoo Mini Plus (OnionOS)

1. Copy the `RetroArch` and `Emu` folders from this repository to your SD card root and merge it with the existing folders.
2. On the device, open a game, then the Quick Menu and configure RetroArch as described below each preview.
3. Don't forget to save the override for Content Directory or Game, depending on the overlay

### Other 640x480 Handhelds (Generic)

As these are mostly simple PNG files made for RetroArch, it's probably compatible with pretty much any 640x480 retro handheld.
See if you can find where you have to copy the overlays.
Please reference a guide for your specific handheld and operating system / firmware. It's probably very similar.
If the offset filters are not compatible, please look for offset / crop functions or shaders for your OS.

## Credits

These overlays were inspired by the work of u/1playerinsertcoin. His Perfect_SYSTEM overlays collection is phenomenal!

All pixel grids and bezels were created entirely by myself, except for the GBA grid. The GBA grid is a heavily modified version of Perfect_GBA by u/1playerinsertcoin, because it is exceptionally good.
