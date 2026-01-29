# dwm Override-Redirect Windows Patch

This patch allows `override-redirect` windows to behave properly in dwm.  
It was originally added to support applications like Krita’s on-canvas color selector, but it applies generally to any application using override-redirect windows.

## Patch Details

- Target: dwm 6.7
- Features: Handles override-redirect windows to prevent focus loss or mapping issues.
- Includes: Adds `#include <X11/XF86keysym.h>` to handle media keys. Remove if you don't want/need media keys.

## Installation

1. Download or clone this repository:

```bash
git clone https://github.com/tristengrant/dwm-override-redirect-windows.git
cd dwm-override-redirect-windows

