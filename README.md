# Subtle Handheld Overlays Collection for Onion OS on Miyoo Mini

The goal of this project is to make it look like classic handheld games are played on a screen with a matching resolution. It is not about creating a photorealistic replica but rather a subtle way to trick your brain into believing that you see physically larger pixels. Flat and jagged pixels get tranformed into a warm and inviting texture. It's not a scientific recreation, it's a nostalgic approximation without unneccessary decoration.

Scaling many different resolutions and aspect ratios to fit a 640x480 screen without artifacting and shimmering is not easy, but I think in the end I got there.

Color systems use a subtle pixel grid that gently shapes and approximates individual pixels. Monochrome LCD handheld systems use a different grid that hints at gaps between the LCD crystals.

Everything is intentionally subtle to avoid negatively affecting image quality while still adding a nostalgic feeling, as if you were playing on a low-resolution display. Lens shadows, rounded corners, and similar embellishments are intentionally omitted to keep the focus on pixel structure and enjoy the Miyoo Mini’s bright IPS display.

Portrait/square overlays add decorative bezels on the sides while landscape overlays shift the rendered image upward with a filter and place the system logo below. This effectively tricks the brain, making the black bars less distracting.

## System Previews and Settings

### Game Boy (GB)

![Subtle_GB preview](.previews/Subtle_GB_Preview.png?v=3)

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

![Subtle_LYNX preview](.previews/Subtle_LYNX_Preview.png?v=3)

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
		Video Filter: Subtle_LYNX
```

### Game Gear (GG)

![Subtle_GG preview](.previews/Subtle_GG_Preview.png?v=3)

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

![Subtle_SUPERVISION preview](.previews/Subtle_SUPERVISION_Preview.png?v=3)

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

![Subtle_MEGADUCK preview](.previews/Subtle_MEGADUCK_Preview.png?v=3)

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

![Subtle_GBC preview](.previews/Subtle_GBC_Preview.png?v=3)

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

![Subtle_NGP preview](.previews/Subtle_NGP_Preview.png?v=3)

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

![Subtle_WS preview](.previews/Subtle_WS_Preview.png?v=3)

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
		Video Filter: Subtle_WS
```

### Game Boy Advance (GBA)

![Subtle_GBA preview](.previews/Subtle_GBA_Preview.png?v=3)

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
		Video Filter: Subtle_GBA
```

### Pokemon Mini (POKE)

![Subtle_POKE preview](.previews/Subtle_POKE_Preview.png?v=3)

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
		Video Filter: Subtle_POKE
In-Game
	Adjust contrast for transitions to match the bezel
```

### Nintendo DS (NDS)

![Subtle_NDS preview](.previews/Subtle_NDS_Preview.png?v=3)

```text
Menu + Start
	Overlay: Subtle_NDS.png?v=3
```

### Apotris (GBA)

![Subtle_Apotris preview](.previews/Subtle_Apotris_Preview.png?v=3)

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

## Credits

These overlays were inspired by the work of u/1playerinsertcoin. His Perfect_SYSTEM overlays collection is phenomenal!

All pixel grids and bezels were created by hand, except for the GBA grid. The GBA grid is an adapted version of Perfect_GBA by u/1playerinsertcoin, because it is exceptionally good and, despite my best efforts, I could not create a grid that produced better results.
