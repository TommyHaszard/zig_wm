# Zig_wm

This project has been forked from Juicebox - where I've used their native X11 implementation to play around with and  make my own tiling WM.

## Future goals
- Provide an async event loop for X11
  - Currently, we're using a simple blocking event loop to handle events, replies, errors from X11. However, Zig provides great primitives (async, suspend, etc) to create a custom event loop that will allow us to make the library itself a lot more efficient.
- General support for multiple screens
  - Also add support for Xinerama
- Provide a translation layer to connect to/with different bars such as [Lemonbar](https://github.com/LemonBoy/bar). (Perhaps a bar of its own).
