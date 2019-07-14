# 🎼 Violin

![size](https://img.shields.io/badge/application%20size:-~55%20--%20132%20MB-yellowgreen.svg) ![platform](https://img.shields.io/badge/runs%20on%3A-windows%20|%20linux%20|%20osx-blue.svg) ![latest releases](https://img.shields.io/github/release-date/CodeF0x/violin.svg?label=latest%20release%3A) [![Codacy Badge](https://api.codacy.com/project/badge/Grade/7549990eb1954df9858c27b21bf0f8ed)](https://www.codacy.com/app/CodeF0x/violin?utm_source=github.com&utm_medium=referral&utm_content=CodeF0x/violin&utm_campaign=Badge_Grade)

![screenshot](docs/assets/screenshot.png)

Violin is a minimalistic and fast music player for Linux, macOS, and Windows.

If you just want to open a folder with your music and start listening instead of importing your songs to Spotify, downloading a huge app that's just overkill for your needs, or your songs are not on streaming platforms, Violin is for you. If that's not the case, you probably won't like Violin.

## 📓 Features

- It's dark themed
- It supports all most common audio file types:
  - mp3
  - wav
  - ogg
  - webm
  - flac
  - mp4
- Shows meta information like album cover, artist and song name if available
- Blazingly fast
- Simple and self-explanatory UI

## 🐛 Bugs / Issues

#### Known Bugs / Issues

- _The album cover gets cropped sometimes_: probably Electron bug -> fix later with new Electron version
- _"Lagging" elements when opening a folder and loading music files into the file list_: also Electron specific issue -> fix later with new Electron version

#### Report an issue

Before reporting an issue, [please check the wiki](https://github.com/CodeF0x/violin/wiki) first. If this didn't help you, you can report issues [here](https://github.com/CodeFox/violin/issues). Please try to lable correctly. (Bug, feature request, etc.)

## ⬇️ Download and install it

[Get it here.](https://github.com/CodeF0x/violin/releases)

## 🔨 Pack it yourself & create a installer

#### Pack it yourself

1. Clone the repository: `$ git clone https://github.com/CodeF0x/violin.git`
2. Install dependencies: `$ npm install`
3. Pack it for your system:
   - `$ npm run package-mac`
   - `$ npm run package-linux`
     - if you want to use Violin on any other distro than a Debian based one, execute the .app file created in this step and skip step 4
   - `$ npm run package-windows`

#### Create a installer

(Steps 1 - 3 from above)

4. Create installer for your system (you must be on the system you want to create an installer for):
   - `$ npm run create-installer-mac`
   - `$ npm run create-installer-linux`
     - this creates a .deb package. For other distros, simply execute the .app file you created in above's step 3
   - `$ npm run create-installer-windows` (not recommended, use the standalone .exe file from step 3 above)
     - this creates a standalone-app what is the expected behaviour. If possible, will switch to a "classical" installer later
