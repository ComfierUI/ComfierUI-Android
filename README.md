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

or a private VPN/Tailscale address:

100.x.x.x:8188

The app automatically handles the required http:// prefix.

ComfyUI must be configured to accept connections from the device you are using.

Remote Access

For access outside your home network, a private VPN such as Tailscale is strongly recommended.

Do not expose your ComfyUI port directly to the public internet unless you fully understand and secure the environment.

ComfyUI does not provide authentication by default.

Quick Start Guide

ComfierUI includes a built-in Quick Start Guide directly on the Connections screen.

The guide covers:

Home-network access
ComfyUI-Manager Personal Cloud mode
Tailscale remote access
Potato Phone Mode
Installing and using ComfierUI Companion
Device Support

ComfierUI is designed for Android phones, foldables, and tablets.

Recommended
Android 9 or newer
6 GB RAM or more
Practical Minimum
Android 8.1
Approximately 4 GB RAM

Large or visually complex workflows may require more capable hardware.

ComfyUI itself continues running on the host computer, so the Android device does not perform model inference.

Potato Phone Mode

Potato Phone Mode is an optional client-side performance mode intended for older or lower-powered Android devices.

When enabled, it reduces the rendering workload of the ComfyUI interface by:

Limiting workflow-canvas rendering to approximately 30 FPS
Reducing animations and transitions
Reducing compositing effects
Using immediate scrolling behavior

It does not change model generation settings or reduce inference quality on the host.

Foldable Support

ComfierUI includes dedicated behavior for foldable devices.

Layouts adapt between outer and inner displays, portrait and landscape orientations, and smaller screen widths.

The interface is designed around touch interaction rather than simply shrinking the desktop UI.

Downloads and Releases

Official Android builds will be distributed through this repository's Releases section.

Only download ComfierUI from official ComfierUI sources.

Privacy

ComfierUI is designed as a client for connecting directly to a ComfyUI server selected by the user.

A full privacy statement will be available in this repository:

PRIVACY.md

Issues and Feedback

Bug reports and compatibility reports can be submitted through the GitHub Issues section.

When reporting an issue, please include:

ComfierUI version
Android version
Device model
ComfyUI version if relevant
Steps needed to reproduce the issue

Please do not include private IP addresses, authentication credentials, API keys, or other sensitive information in public issue reports.

Source Availability

The ComfierUI Android application is proprietary software and is not open source.

This public repository is provided for:

Releases
Documentation
Privacy information
Issue tracking
Project information

The open-source ComfierUI Companion extension is maintained separately.

Copyright

Copyright © 2026 ComfierUI.

All rights reserved.
