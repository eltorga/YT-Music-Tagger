# 🎵 YT Music Tagger

<p align="center">
  <b>A simple and modern MP3 metadata editor for Windows.</b>
</p>

<p align="center">
  Edit song titles, artists, albums, cover art and filenames directly from a clean desktop interface.
</p>

---

## ✨ About

**YT Music Tagger** is a lightweight desktop application for editing MP3 metadata.

It is designed for users who want an easy way to organize their personal music library without using complicated tagging software.

The application lets you open an MP3 file, edit its metadata, replace its cover art and save the changes directly to the original file.

> YT Music Tagger is an independent project and is not affiliated with YouTube, YouTube Music, or Google.

---

## 🎧 Features

- 🎵 Open `.mp3` files from your computer
- 🖱️ Drag and drop MP3 files into the application
- ✏️ Edit song title
- 👤 Edit artist
- 💿 Edit album
- 🎤 Edit album artist
- 📅 Edit year
- 🎶 Edit genre
- 🔢 Edit track number
- 📁 Rename the physical MP3 file
- 🖼️ Add or replace album artwork
- 🖱️ Drag and drop JPG, PNG or WEBP cover images
- ▶️ Built-in audio preview
- 💾 Save changes directly to the original MP3
- ⚠️ Warning when opening another song with unsaved changes
- ⚠️ Warning before closing the application with unsaved changes
- ⌨️ Keyboard shortcuts
- 🌙 Modern dark interface
- 🔒 Local processing
- ☁️ No cloud upload required

---

# 📥 Download

Go to the **Releases** section of this repository and download the latest version.

For version 1.1:

```text
YT-Music-Tagger-v1.1-English.zip
```

After downloading the ZIP file, extract it to a normal folder.

For example:

```text
C:\YT-Music-Tagger
```

> Do not run the application directly from inside the ZIP file.

---

# 🟢 Requirements

YT Music Tagger currently requires:

```text
Windows 10 or newer
Node.js 22 or newer
```

Download Node.js from:

https://nodejs.org/

During installation, keep the default options enabled.

Make sure Node.js is added to your Windows `PATH`.

---

# 🚀 First-Time Installation

After extracting the ZIP file, open the YT Music Tagger folder.

You should see files similar to:

```text
YT-Music-Tagger
│
├── INSTALL_AND_RUN_NO_TERMINAL.vbs
├── RUN_NO_TERMINAL.vbs
├── INSTALL_AND_RUN.bat
├── RUN.bat
├── BUILD_EXE.bat
│
├── main.js
├── preload.js
├── renderer.js
├── index.html
├── styles.css
├── package.json
└── README.md
```

For the first installation, double-click:

```text
INSTALL_AND_RUN_NO_TERMINAL.vbs
```

This is the recommended installation method.

The installer will:

1. Check if Node.js is installed.
2. Install the required dependencies.
3. Install Electron.
4. Launch YT Music Tagger automatically.

The first installation may take a few minutes because the required packages need to be downloaded.

---

# 🪟 Windows Terminal Configuration Error

Some Windows systems may display an error similar to:

```text
Error loading settings

Syntax error:
value, object or array expected
```

This error belongs to **Windows Terminal configuration** and is not caused by YT Music Tagger.

If this happens, use:

```text
INSTALL_AND_RUN_NO_TERMINAL.vbs
```

instead of:

```text
INSTALL_AND_RUN.bat
```

The `.vbs` installer runs the installation without depending on Windows Terminal.

If the installation itself fails, a file called:

```text
installation.log
```

will be created inside the YT Music Tagger folder.

This file contains the installation error details.

---

# ▶️ Opening YT Music Tagger After Installation

After the first installation, you do not need to install the dependencies again.

Simply double-click:

```text
RUN_NO_TERMINAL.vbs
```

YT Music Tagger will open normally.

You can also use:

```text
RUN.bat
```

if Command Prompt or Windows Terminal works correctly on your system.

---

# 🎵 How to Use YT Music Tagger

Using the application is simple.

---

## 1. Open an MP3 File

Click:

```text
Open song
```

and select an `.mp3` file from your computer.

You can also drag an MP3 directly into the application window.

Example:

```text
My Song.mp3
```

YT Music Tagger will automatically read the metadata stored inside the file.

---

## 2. Edit the Song Information

You can edit:

```text
Title
Artist
Album
Album Artist
Year
Genre
Track Number
Physical Filename
```

For example:

```text
Title:
My Song

Artist:
My Artist

Album:
My Album

Album Artist:
My Artist

Year:
2026

Genre:
Electronic

Track Number:
1
```

---

# 📁 Song Title vs Filename

The song title and the physical filename are different values.

For example, your physical file can be:

```text
01 - My Artist - My Song.mp3
```

while the internal metadata can be:

```text
Title:
My Song
```

This allows music players and services to display a clean song title even if the physical filename contains additional information.

---

# ⚠️ Why `.mp3` Is Not Removed

YT Music Tagger intentionally keeps the `.mp3` extension on the physical file.

Correct:

```text
My Song.mp3
```

The internal metadata title can still be:

```text
My Song
```

Removing the real `.mp3` extension could cause Windows, music players or other applications to stop recognizing the file automatically.

If your goal is to make the song appear without `.mp3` in a music library, edit the **Title** field instead of removing the physical extension.

---

# 🖼️ Changing the Cover Art

First, open an MP3 file.

Then drag an image onto the cover area.

Supported image formats:

```text
JPG
JPEG
PNG
WEBP
```

You can also click the cover area and select an image manually.

The new artwork will appear immediately in the application.

However, the cover is not written to the MP3 until you click:

```text
Save changes
```

---

# 💾 Saving Changes

When you modify any information, YT Music Tagger will display:

```text
Unsaved changes
```

Click:

```text
Save changes
```

The metadata will be written directly to the MP3 file you opened.

No new MP3 needs to be downloaded.

The original file itself is updated.

After saving, the application will display:

```text
All changes saved
```

---

# ⚠️ Unsaved Changes Protection

If you modify a song and try to open another MP3 before saving, YT Music Tagger will warn you.

You can choose:

```text
Cancel
```

or:

```text
Discard changes
```

The same protection is used if you attempt to close the application while there are unsaved changes.

This helps prevent accidentally losing your edits.

---

# ▶️ Audio Preview

YT Music Tagger includes a built-in audio player.

After opening an MP3, you can play the song directly inside the application.

This is useful for confirming that you selected the correct file before editing its metadata.

---

# ⌨️ Keyboard Shortcuts

| Shortcut | Action |
|---|---|
| `Ctrl + O` | Open an MP3 |
| `Ctrl + S` | Save changes |

---

# 🔒 Privacy

YT Music Tagger works locally on your computer.

Your MP3 files and cover images do not need to be uploaded to an external server in order to edit their metadata.

Your music stays on your computer.

---

# 🧪 Recommended First Test

Before editing an important file for the first time, create a copy.

For example:

```text
original-song.mp3
```

Create a copy named:

```text
test-song.mp3
```

Open `test-song.mp3` in YT Music Tagger.

Change:

```text
Title
Artist
Album
Cover Art
Filename
```

Then click:

```text
Save changes
```

After saving, open the file in your normal music player or check its properties in Windows.

Once you confirm everything works as expected, you can use YT Music Tagger with your normal music library.

---

# 🛠️ Running From Source

If you prefer to run the application manually from the command line, open Command Prompt or PowerShell inside the project folder.

Install the dependencies:

```bash
npm install
```

Then run:

```bash
npm start
```

---

# 📦 Building the Windows Installer

To create a Windows installer, first install the dependencies:

```bash
npm install
```

Then run:

```bash
npm run build
```

You can also simply double-click:

```text
BUILD_EXE.bat
```

After the build process finishes, open the:

```text
dist
```

folder.

You should find a Windows installer similar to:

```text
YT Music Tagger Setup 1.1.0.exe
```

After installing it, YT Music Tagger can be opened like a normal Windows application.

---

# 🎶 Supported Audio Formats

Current version:

```text
✅ MP3
```

YT Music Tagger currently focuses only on MP3 files to keep metadata editing simple and reliable.

Possible future support may include:

```text
FLAC
M4A
OGG
WAV
```

---

# 🚧 Planned Features

Possible future improvements include:

- Multi-song editing
- Batch metadata editing
- Music library view
- Batch album editing
- Batch artist editing
- Batch cover art assignment
- Automatic track numbering
- FLAC support
- M4A support
- OGG support
- Better drag-and-drop management
- Portable Windows version
- Automatic updates
- Improved Windows installer
- Additional metadata fields

---

# 🧰 Built With

YT Music Tagger is built using:

- Electron
- Node.js
- JavaScript
- HTML
- CSS
- node-id3
- electron-builder

---

# ❤️ Project Goal

The goal of YT Music Tagger is to provide a simple workflow:

```text
Open → Edit → Add Cover → Save
```

No complicated menus.

No unnecessary tools.

Just simple MP3 metadata editing.

---

# ⚠️ Disclaimer

YT Music Tagger is an independent open-source project.

It is not affiliated with, endorsed by, sponsored by, or officially connected with YouTube, YouTube Music, or Google.

YouTube and YouTube Music are trademarks of Google LLC.

---

# ⭐ Support the Project

If you find YT Music Tagger useful, consider giving the repository a ⭐.

Bug reports, improvements and feature suggestions are welcome through GitHub Issues.
