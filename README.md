# Subtle Handheld Overlays Collection for Onion OS on Miyoo Mini

The goal of this project is to make it look like classic handheld games are played on a screen with a matching resolution. It is not about creating a photorealistic replica but rather a subtle way to trick your brain into believing that you see physically larger pixels. Flat and jagged pixels get tranformed into a warm and inviting texture. It's not a scientific recreation, it's a nostalgic approximation without unneccessary decoration.

Scaling many different resolutions and aspect ratios to fit a 640x480 screen without artifacting and shimmering is not easy, but I think in the end I got there.

Color systems use a subtle pixel grid that gently shapes and approximates individual pixels. Monochrome LCD handheld systems use a different grid that hints at gaps between the LCD crystals.

Everything is intentionally subtle to avoid negatively affecting image quality while still adding a nostalgic feeling, as if you were playing on a low-resolution display. Lens shadows, rounded corners, and similar embellishments are intentionally omitted to keep the focus on pixel structure and enjoy the Miyoo Mini’s bright IPS display.

Portrait/square overlays add decorative bezels on the sides while landscape overlays shift the rendered image upward with a filter and place the system logo below. This effectively tricks the brain, making the black bars less distracting.

## System Previews and Settings

### Game Boy (GB)

![Subtle_GB preview](.previews/Subtle_GB_Preview.png?v=10)

```text
Quick Menu
	On-Screen Overlay
		Display Overlay: On
		Overlay Preset: Subtle_GB
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

### Lynx

![Subtle_LYNX preview](.previews/Subtle_LYNX_Preview.png?v=10)

```text
Quick Menu
	On-Screen Overlay
		Display Overlay: On
		Overlay Preset: Subtle_LYNX
Settings
	Video
		Scaling
			Integer Scale: Off
			Keep Aspect Ratio: On
		Image Interpolation: Bicubic
		Video Filter: Subtle_LYNX (or any other way to offset up for 9px)
```

### Game Gear (GG)

![Subtle_GG preview](.previews/Subtle_GG_Preview.png?v=10)

```text
Quick Menu
	On-Screen Overlay
		Display Overlay: On
		Overlay Preset: Subtle_GG
Settings
	Video
		Scaling
			Integer Scale: Off
			Keep Aspect Ratio: Off
		Image Interpolation: Bicubic
```

### Supervision

![Subtle_SUPERVISION preview](.previews/Subtle_SUPERVISION_Preview.png?v=10)

```text
Quick Menu
	On-Screen Overlay
		Display Overlay: On
		Overlay Preset: Subtle_SUPERVISION
	Core Options
		Internal Palette: Game Boy Pocket
Settings
	Video
		Scaling
			Integer Scale: Off
			Keep Aspect Ratio: On
		Image Interpolation: Bicubic
```

### Mega Duck

![Subtle_MEGADUCK preview](.previews/Subtle_MEGADUCK_Preview.png?v=10)

```text
Quick Menu
	On-Screen Overlay
		Display Overlay: On
		Overlay Preset: Subtle_MEGADUCK
Settings
	Video
		Scaling
			Integer Scale: Off
			Keep Aspect Ratio: On
		Image Interpolation: Bicubic
```

### Game Boy Color (GBC)

![Subtle_GBC preview](.previews/Subtle_GBC_Preview.png?v=10)

```text
Quick Menu
	On-Screen Overlay
		Display Overlay: On
		Overlay Preset: Subtle_GBC
Settings
	Video
		Scaling
			Integer Scale: Off
			Keep Aspect Ratio: On
		Image Interpolation: Bicubic
```

### Neo Geo Pocket (NGP)

![Subtle_NGP preview](.previews/Subtle_NGP_Preview.png?v=10)

```text
Quick Menu
	On-Screen Overlay
		Display Overlay: On
		Overlay Preset: Subtle_NGP
Settings
	Video
		Scaling
			Integer Scale: Off
			Keep Aspect Ratio: On
		Image Interpolation: Bicubic
```

### WonderSwan (WS)

![Subtle_WS preview](.previews/Subtle_WS_Preview.png?v=10)

```text
Quick Menu
	On-Screen Overlay
		Display Overlay: On
		Overlay Preset: Subtle_WS
Settings
	Video
		Scaling
			Integer Scale: Off
			Keep Aspect Ratio: On
		Image Interpolation: Bicubic
		Video Filter: Subtle_WS (or any other way to offset up for 12px)
```

### Game Boy Advance (GBA)

![Subtle_GBA preview](.previews/Subtle_GBA_Preview.png?v=10)

```text
Quick Menu
	On-Screen Overlay
		Display Overlay: On
		Overlay Preset: Subtle_GBA
Settings
	Video
		Scaling
			Integer Scale: Off
			Keep Aspect Ratio: On
		Image Interpolation: Bicubic
		Video Filter: Subtle_GBA (or any other way to offset up for 10px)
```

### Pokemon Mini (POKE)

![Subtle_POKE preview](.previews/Subtle_POKE_Preview.png?v=10)

The Pokémon Mini overlay requires a unique approach. Due to the ultra-low resolution, a fully upscaled image results in gigantic pixels that quickly strain eyes and brain. Furthermore, games often place text and art right at the screen's edge. Because of generous padding around the physical display this wasn't an issue on original hardware, but scaling the image to the very edges of a modern retro handheld makes UI elements hard to parse.

To solve this, I opted for integer scaling. This slightly reduces the pixel size and leaves room for padding around the gameplay area. Finally, to achieve a softer, warmer feel, I added a very subtle layer of film grain. Without it, the chunky pixels look a bit too flat and digital.

Because of the much higher resolutions of the other LCD handhelds, namely GameBoy, MegaDuck and Supervision, I didn't treat them this way. Their pixel grid is fine enough and sprite placement rarely needs additional padding. The dimensions also don't allow for easy padding at consistent sizing anyway.

```text
Quick Menu
	On-Screen Overlay
		Display Overlay: On
		Overlay Preset: Subtle_POKE
Core Options
		LCD Filter: None
Settings
	Video
		Scaling
			Integer Scale: On
			Keep Aspect Ratio: On
		Image Interpolation: Bicubic
		Video Filter: Subtle_POKE (or any other way to offset up for 16px)
In-Game
	Adjust contrast for transitions to match the bezel
```

### Nintendo DS (NDS)

![Subtle_NDS preview](.previews/Subtle_NDS_Preview.png?v=10)

```text
Menu + Start
	Overlay: Subtle_NDS.png
```

### Apotris (GBA)

![Subtle_Apotris preview](.previews/Subtle_Apotris_Preview.png?v=10)

```text
Quick Menu
	On-Screen Overlay
		Display Overlay: On
		Overlay Preset: Subtle_Apotris
Settings
	Video
		Scaling
			Integer Scale: On
			Keep Aspect Ratio: On
		Image Interpolation: Nearest Neighbor
		Video Filter: Subtle_Apotris
In-Game
	Settings
		Graphics
			Aspect Ratio: 4:3
```

## Installation

### Miyoo Mini / Miyoo Mini Plus (OnionOS)

1. Copy the `RetroArch` and `Emu` folders from this repository to your SD card root and merge it with the existing folders.
2. On the device, open a game, then the Quick Menu and configure RetroArch as described below each preview.
3. Don't forget to save the override for Content Directory (or Game, in case of Apotris)

### Other 640x480 Handhelds (Generic)

As these are mostly simple PNG files made for RetroArch, it's probably compatible with pretty much any 640x480 retro handheld.
See if you can find where you have to copy the overlays.
Please reference a guide for your specific handheld and operating system / firmware. It's probably very similar.
If the offset filters are not compatible, please look for offset / crop functions or shaders for your OS.

## Credits

These overlays were inspired by the work of u/1playerinsertcoin. His Perfect_SYSTEM overlays collection is phenomenal!

All pixel grids and bezels were created entirely by myself, except for the GBA grid. The GBA grid is a heavily modified version of Perfect_GBA by u/1playerinsertcoin, because it is exceptionally good.
