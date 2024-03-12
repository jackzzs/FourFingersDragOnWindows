[![Release](https://img.shields.io/github/v/release/jackzzs/FourFingersDragOnWindows?label=Download%20version)](https://github.com/jackzzs/FourFingersDragOnWindows/releases/latest)
[![TotalDownloads](https://img.shields.io/github/downloads/jackzzs/FourFingersDragOnWindows/total)](https://github.com/jackzzs/FourFingersDragOnWindows/releases/latest)

## Overview and fork description
This program can bring the macOS-style three-finger dragging functionality to Windows computers, to select text or perform other selecting operations.

You can also optionally implement middle-button dragging using four fingers.

Forked from [ClementGre/ThreeFingersDragOnWindows](https://github.com/ClementGre/ThreeFingersDragOnWindows), and mainly adds support for four-finger middle-button dragging on its basis, out of the need for middle-button dragging as a commonly used view rotation operation in many programs, especially games and 3D software.

Thanks to the original author for bringing such a good software.

This fork follows the MIT License used by the original author.

## Preview
<p align="center">
  <img src='https://raw.githubusercontent.com/jackzzs/FourFingersDragOnWindows/main/ThreeFingersDragOnWindows/Assets/Screenshot-1.png' alt="App screenshot: Touchpad tab" width='700'>
  <img src='https://raw.githubusercontent.com/jackzzs/FourFingersDragOnWindows/main/ThreeFingersDragOnWindows/Assets/Screenshot-2.png' alt="App screenshot: Three Fingers Drag tab" width='700'>
  <img src='https://raw.githubusercontent.com/jackzzs/FourFingersDragOnWindows/main/ThreeFingersDragOnWindows/Assets/Screenshot-3.png' alt="App screenshot: Other Settings tab" width='700'>
</p>

## Installation

Download the zip package from [Github Release](https://github.com/jackzzs/FourFingersDragOnWindows/releases) and run `FourFingersDragOnWindows.exe`.

You can enable the `Run at Startup` option from the `Other Settings` page of the program.

You may need to have the Windows App SDK redistributable installed. You can download it from this page: [https://learn.microsoft.com/en-us/windows/apps/windows-app-sdk/downloads](https://learn.microsoft.com/en-us/windows/apps/windows-app-sdk/downloads).

## How to use

Make sure to disable the "Tap twice and drag to multi-select" behaviour and all of the defaults 3-finger and 4-finger swipe behaviour
via ``Touchpad settings`` in windows preferences for the drag to work without interferences.

To open the configuration pane, click the FourFingersDragOnWindows tray icon on the Windows task bar.

## Build and Execute

The app can be built and run in Microsoft Visual Studio or Jetbrains Rider.

## Libraries used

The app is WinUI 3 app, that uses the [Microsoft.UI.Xaml](https://docs.microsoft.com/en-us/windows/apps/winui/winui3/) library.

Other libraries used:
- [emoacht/RawInput.Touchpad](https://github.com/emoacht/RawInput.Touchpad) Allows to get the raw input of the touchpad (included in the source code as TouchpadHelper.cs).
- [HavenDV/H.NotifyIcon](https://github.com/HavenDV/H.NotifyIcon) API for Windows taskbar tray icon in a WinUI app.
- [dahall/TaskScheduler](https://github.com/dahall/TaskScheduler) API for Windows TaskScheduler (used for the skipUAC).
