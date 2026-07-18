# Skip Intro Videos In Majesty Gold HD

Majesty Gold HD has a hidden preference that can skip the startup intro videos and load
straight to the main menu.

## Easiest Method

1. Download the latest ZIP from the GitHub release page.
2. Extract the ZIP.
3. Double-click `Enable Skip Intro Videos.bat`.
4. Start Majesty Gold HD normally from Steam.

To undo it, double-click `Restore Intro Videos.bat`.

## What The Helper Does

The helper edits this file:

```text
Documents\My Games\MajestyHD\MajXPrefs
```

It changes:

```xml
<IntroVideo>1</IntroVideo>
```

to:

```xml
<IntroVideo>0</IntroVideo>
```

It also creates a backup first.

## Manual Method

You can also right-click Majesty Gold HD in Steam, open Properties, and add this launch
option:

```text
-nointro
```

## Why This Is Not A Workshop Mod

Majesty loads Workshop mods from the in-game Mods menu, after startup. The intro-video
choice happens before the menu loads, so a Workshop mod cannot reliably change it.
