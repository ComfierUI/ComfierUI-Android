# ComfierUI Android

ComfierUI is a dedicated Android client for ComfyUI, designed to make remote workflow creation and execution feel natural on phones, foldables, and tablets.

Rather than replacing ComfyUI, ComfierUI connects directly to your existing ComfyUI host and adapts the interface for touch, smaller displays, device rotation, and mobile navigation.

## Current Version

**0.8.62**

## What ComfierUI Does

ComfierUI wraps the standard ComfyUI web interface in a mobile-focused Android client and adds a large set of touch and layout improvements while preserving access to the desktop feature set.

Highlights include:

- Touch-optimized workflow editing and canvas navigation
- Two-finger canvas pan and zoom
- Mobile-friendly node, menu, dropdown, and text-entry behavior
- Foldable-aware layouts and rotation handling
- Dedicated connection profiles
- Remote use over LAN or private VPN connections such as Tailscale
- Native Android Back-button behavior for ComfyUI panels, dialogs, menus, and app navigation
- Adjustable UI Scale and Connector Offset controls
- Gallery swipe navigation
- Hard Refresh and Disconnect controls
- Android workflow JSON file picker integration
- Mobile-optimized execution controls
- Image Feed support
- Video preview support
- Optional Potato Phone Mode for lower-powered devices
- Built-in Quick Start Guide
- Optional ComfierUI Companion integration

The goal is full ComfyUI functionality without requiring users to sit at the host computer.

## ComfierUI Companion

ComfierUI Companion is an optional open-source ComfyUI extension that adds additional host-side integration for ComfierUI.

It can be installed directly through **ComfyUI Extension Manager** by searching for:

**ComfierUI Companion**

Current Companion functionality includes:

- Companion version detection inside ComfierUI
- Host-side downloads for supported models listed by ComfyUI's Missing Models interface
- Download progress reporting
- Large model files remain on the host computer and do not pass through the Android device

Companion is optional. The core ComfierUI Android client remains functional without it.

Companion source and documentation:

https://github.com/ComfierUI/ComfierUI-Companion

## Connecting to ComfyUI

ComfierUI connects to a running ComfyUI server using its host address.

Typical examples include:

```text
192.168.1.100:8188
