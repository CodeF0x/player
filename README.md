# 🎼 Violin

![screenshot](docs/images/screenshot.png)

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

- The album cover gets cropped sometimes: that's an issue with how certain CSS properties work in Electron. Maybe there will be a fix in future releases of Electron, but by now, this cannot get fixed.
- "Laggin" elements when opening a folder and loading music files into the file list: that's also an issue with Electron, but I don't know what causes it. (Replicating the problem in a "normal" browser was not successful, no lagging in Firefox and Chrome, even with a greater amount of HTMLElements that get appended to the DOM)

##### Report an issue

You can report issues [here](https://github.com/CodeFox/violin/issues). Please try to lable correctly. (Bug, feature request, etc.)

## ⬇️ Download and install it

[Get it here.](https://github.com/CodeF0x/violin/releases)

## 🔨 Pack it yourself & create a installer

#### Pack it yourself

1. Clone the repository `git clone https://github.com/CodeF0x/violin.git`
2. Install dependencies `npm install`
3. Pack it for your system:
   - `npm run package-mac`
   - `npm run package-linux`
   - `npm run package-windows`

#### Create a installer

(Steps 1 - 3 from above)

4. Create installer for your system (you must be on the system you want to create an installer for):
   - `npm run create-installer-mac`
   - `npm run create-installer-linux` (this creates a .deb package. For other distros, use the created .app file you created in above's step 3)
   - `npm run create-installer-windows` (this creates a standalone-app what is the expected behaviour. If possible, will switch to a "classical" installer later)
