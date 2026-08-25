# HTML5b
I just found some bugs or things that can be faster in the code and tried to fix them. Also i tried to add a mobile joystick
orginal discription:
An HTML5 port of Cary Huang's flash game [BFDIA 5b](http://bfdi.tv/5b/) using only pureJS and HTML5. All gameplay, level creator, and explore features have been fully implemented.

A lot of the code in here I didn't write. Since actionscript is so similar to javascript; a lot of the code was just copy-pasted from the decompiled swf with some minor reformatting.

## Changes Made

### Bug Fixes
- Fixed searchParams.get() to use parameter names instead of full URLs (Line 113)
- Fixed NaN validation to use isNaN() instead of string comparison (Line 205)

### Performance Optimizations
- Added viewport culling for tiles and characters
- Added bitmap caching for SVG tiles
- Added isInViewport() helper function
- Added getSvgTileBitmap() for tile bitmap caching
### Mobile Controls
- Added on-screen D-pad buttons for mobile users
- Buttons include: Move Left/Right/Up/Down, Jump, Swap Character, Reset Level
- Controls automatically appear on mobile/touch devices
- Buttons support both touch and mouse input