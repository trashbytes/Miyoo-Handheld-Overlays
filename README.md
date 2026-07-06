# Subtle Handheld Overlays Collection for Onion OS on Miyoo Mini

This project is not about creating photorealistic overlays for every specific device. The goal is to improve how classic handheld systems look when low pixel-density graphics are upscaled to a 640x480 display, so the image feels less flat and less purely pixel-sharp, and a bit more like playing on a real native screen. It also masks the inherent artifacts of non-integer upscaling.

Color handheld systems use a subtle pixel grid that gently shapes and simulates individual pixels. Monochrome LCD handheld systems use a different grid that simulates the gaps between LCD crystals.

Everything is intentionally subtle to avoid negatively affecting image quality while still adding a nostalgic feeling, as if you were playing on a low-resolution display.

Portrait overlays include decorative bezels on the left and right sides. Landscape overlays shift the rendered image upward with a filter and place the system logo below.

## System Previews and Settings

### Game Boy (GB)

![Subtle_GB preview](RetroArch/.retroarch/overlay/GB/Subtle_GB/Subtle_GB.png)

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

![Subtle_LYNX preview](RetroArch/.retroarch/overlay/LYNX/Subtle_LYNX/Subtle_LYNX.png)

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

![Subtle_GG preview](RetroArch/.retroarch/overlay/GG/Subtle_GG/Subtle_GG.png)

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

![Subtle_SUPERVISION preview](RetroArch/.retroarch/overlay/SUPERVISION/Subtle_SUPERVISION/Subtle_SUPERVISION.png)

```text
Quick Menu
	On-Screen Overlay
		Display Overlay: On
		Overlay Preset: Subtle_SUPERVISION
Settings
	Video
		Scaling
			Integer Scale: Off
			Keep Aspect Ratio: On
		Image Interpolation: Bicubic
```

### Mega Duck

![Subtle_MEGADUCK preview](RetroArch/.retroarch/overlay/MEGADUCK/Subtle_MEGADUCK/Subtle_MEGADUCK.png)

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

![Subtle_GBC preview](RetroArch/.retroarch/overlay/GBC/Subtle_GBC/Subtle_GBC.png)

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

![Subtle_NGP preview](RetroArch/.retroarch/overlay/NGP/Subtle_NGP/Subtle_NGP.png)

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

![Subtle_WS preview](RetroArch/.retroarch/overlay/WS/Subtle_WS/Subtle_WS.png)

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

![Subtle_GBA preview](RetroArch/.retroarch/overlay/GBA/Subtle_GBA/Subtle_GBA.png)

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

![Subtle_POKE preview](RetroArch/.retroarch/overlay/POKE/Subtle_POKE/Subtle_POKE.png)

```text
Quick Menu
	On-Screen Overlay
		Display Overlay: On
		Overlay Preset: Subtle_POKE
Settings
	Video
		Scaling
			Integer Scale: On
			Keep Aspect Ratio: On
		Image Interpolation: Bicubic
		Video Filter: Subtle_POKE
```

### Nintendo DS (NDS)

![Subtle_NDS preview](Emu/NDS/resources/overlay/Subtle_NDS.png)

```text
Menu + Start
	Overlay: Subtle_NDS.png
```

### Apotris (GBA)

![Subtle_Apotris preview](RetroArch/.retroarch/overlay/GBA/Subtle_Apotris/Subtle_Apotris.png)

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
