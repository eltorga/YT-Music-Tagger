# 🎵 YT Music Tagger

<p align="center">
  <b>A simple MP3 metadata editor for Windows, built with Electron.</b>
</p>

<p align="center">
  Edit titles, artists, albums, cover art and filenames directly from a modern interface inspired by YouTube Music.
</p>

---

## ✨ About

**YT Music Tagger** is a simple desktop application designed to make editing MP3 metadata easy.

It was created especially for people who organize their own music library or upload personal music files to services such as YouTube Music.

You don't need to know anything about programming or ID3 tags.

Simply open an MP3 file, edit its information, add a cover and press **Save Changes**.

The application modifies the original MP3 directly.

> YT Music Tagger is an independent project and is not affiliated with YouTube, YouTube Music or Google.

---

## 🎧 Features

- 🎵 Open MP3 files directly from your computer
- 🖱️ Drag and drop MP3 files into the application
- ✏️ Edit song title
- 👤 Edit artist
- 💿 Edit album
- 🎤 Edit album artist
- 📅 Edit year
- 🎶 Edit genre
- 🔢 Edit track number
- 🖼️ Add or replace album artwork
- 🖱️ Drag and drop JPG, PNG or WEBP cover images
- 📁 Rename the original MP3 file
- 💾 Save directly to the original file
- ⚠️ Warning when opening another song with unsaved changes
- ⚠️ Warning when closing the program with unsaved changes
- ▶️ Built-in audio preview
- ⌨️ Keyboard shortcuts
- 🌙 Modern dark interface inspired by YouTube Music
- 🔒 Works locally — your music is not uploaded anywhere

---

# 📥 Installation

There are two ways to use YT Music Tagger.

For most users, the easiest method is the one described below.

---

## 1. Download YT Music Tagger

Go to the **Releases** section of this repository.

Download the latest:

```text
YT-Music-Tagger-v1.1.zip
```

After downloading it, extract the ZIP file.

For example:

```text
C:\YT-Music-Tagger
```

> Do not run the program directly from inside the ZIP file.

---

# 🟢 First-time installation

YT Music Tagger is built with Electron, so the development version requires **Node.js**.

## 2. Install Node.js

If Node.js is not installed on your computer, download and install **Node.js 22 or newer**.

Official website:

https://nodejs.org/

During installation, you can leave the default options enabled.

Make sure Node.js is added to the Windows `PATH`.

---

## 3. Open the YT Music Tagger folder

After extracting the downloaded ZIP, you should see files similar to these:

```text
YT-Music-Tagger
│
├── INSTALAR_Y_EJECUTAR_SIN_TERMINAL.vbs
├── EJECUTAR_SIN_TERMINAL.vbs
├── INSTALAR_Y_EJECUTAR.bat
├── EJECUTAR.bat
├── CREAR_EXE.bat
│
├── main.js
├── preload.js
├── renderer.js
├── index.html
├── styles.css
├── package.json
└── README.md
```

---

## 4. Run the installer

For the first installation, double-click:

```text
INSTALAR_Y_EJECUTAR_SIN_TERMINAL.vbs
```

This is the recommended installation method.

The script will install the required dependencies and then automatically launch YT Music Tagger.

The first installation may take a few minutes because Electron and the required packages need to be downloaded.

An internet connection is required only for this installation step.

---

## 🪟 Windows Terminal configuration error

Some Windows installations may display an error similar to:

```text
Error loading settings

Syntax error:
value, object or array expected
```

This error comes from **Windows Terminal configuration**, not from YT Music Tagger.

If this happens, use:

```text
INSTALAR_Y_EJECUTAR_SIN_TERMINAL.vbs
```

instead of:

```text
INSTALAR_Y_EJECUTAR.bat
```

The `.vbs` version installs and launches the application without depending on Windows Terminal.

---

# 🚀 Opening the application after installation

After completing the first installation, you do not need to install everything again.

Simply double-click:

```text
EJECUTAR_SIN_TERMINAL.vbs
```

YT Music Tagger will open.

---

# 🎵 How to use YT Music Tagger

Using the program is very simple.

## 1. Open an MP3

Click:

```text
Abrir canción
```

and select an `.mp3` file.

You can also drag an MP3 directly into the YT Music Tagger window.

For example:

```text
My Song.mp3
```

The program will automatically read the metadata stored inside the file.

---

## 2. Edit the song information

You can modify:

```text
Title
Artist
Album
Album Artist
Year
Genre
Track Number
Filename
```

For example, your original file might be:

```text
01 - My Artist - My Song.mp3
```

But its metadata can be:

```text
Title:
My Song

Artist:
My Artist

Album:
My Album
```

This allows music players and services to display a clean song title even if the physical filename contains additional information.

---

# 📁 Filename vs Song Title

This is an important distinction.

The physical file might be:

```text
01 - My Artist - My Song.mp3
```

while the internal song title can be:

```text
My Song
```

YT Music Tagger lets you edit both independently.

---

## ⚠️ Why `.mp3` is not removed

YT Music Tagger intentionally keeps:

```text
.mp3
```

at the end of the physical file.

For example:

```text
My Song.mp3
```

Removing the extension completely could prevent Windows, music players or other applications from automatically recognizing the file as an MP3.

Instead, simply use:

```text
Title:
My Song
```

The filename remains:

```text
My Song.mp3
```

while the internal title is:

```text
My Song
```

---

# 🖼️ Changing the cover

First open an MP3.

Then drag an image directly onto the cover area.

Supported image formats:

```text
JPG
JPEG
PNG
WEBP
```

You can also click the cover area and select an image manually.

The new artwork will immediately appear inside the application.

However, it is not written to the MP3 until you press:

```text
Guardar cambios
```

---

# 💾 Saving your changes

When you modify any information, YT Music Tagger will show:

```text
Cambios sin guardar
```

Press:

```text
Guardar cambios
```

The program will write the metadata directly into the MP3 you opened.

No new MP3 needs to be downloaded.

No duplicate is intentionally created.

The original file itself is updated.

After saving, the application will display:

```text
Todos los cambios guardados
```

---

# ⚠️ Unsaved changes protection

If you edit a song and try to open another MP3 without saving, the application will warn you.

You can choose whether to:

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

# ▶️ Audio preview

After opening an MP3, an audio player appears inside the application.

You can use it to quickly confirm that you opened the correct song before editing its metadata.

---

# ⌨️ Keyboard shortcuts

```text
Ctrl + O
Open an MP3

Ctrl + S
Save changes
```

---

# 🔒 Privacy

YT Music Tagger works locally on your computer.

Your MP3 files and cover images are not intentionally uploaded to a server.

Editing is performed directly on your local files.

---

# 🧪 Recommendation for your first test

Before editing an important song for the first time, make a copy of it.

For example:

```text
original-song.mp3
```

Create:

```text
test-song.mp3
```

Open `test-song.mp3` in YT Music Tagger.

Change:

```text
Title
Artist
Album
Cover
Filename
```

Press:

```text
Guardar cambios
```

Then open the file in your normal music player or check its properties in Windows.

Once you confirm everything works as expected, you can start editing your normal library.

---

# 🛠️ Running from source

If you prefer using the command line, open a terminal inside the project folder.

Install dependencies:

```bash
npm install
```

Run the application:

```bash
npm start
```

---

# 📦 Building the Windows installer

YT Music Tagger can also be packaged as a normal Windows application.

First install the dependencies:

```bash
npm install
```

Then run:

```bash
npm run build
```

Or simply double-click:

```text
CREAR_EXE.bat
```

After the build finishes, check the:

```text
dist
```

folder.

You should find an installer similar to:

```text
YT Music Tagger Setup 1.0.0.exe
```

After installing it, YT Music Tagger can be opened like a regular Windows application.

---

# 📝 Supported audio formats

Current version:

```text
✅ MP3
```

The application currently focuses only on MP3 files to keep metadata editing simple and reliable.

Possible future support may include:

```text
FLAC
M4A
WAV
OGG
```

---

# 🚧 Planned improvements

Possible features for future versions include:

- Multiple-song editing
- Song library view
- Batch metadata editing
- Batch album assignment
- Batch cover assignment
- Automatic track numbering
- FLAC support
- M4A support
- Better drag-and-drop management
- Windows installer improvements
- Portable version
- Automatic updates

---

# 🧰 Built With

- Electron
- JavaScript
- HTML
- CSS
- Node.js
- node-id3
- electron-builder

---

# ❤️ Purpose

YT Music Tagger was created to make organizing personal MP3 collections easier.

Instead of using complicated professional tagging applications, the goal is to provide a simple interface where you can:

```text
Open → Edit → Add Cover → Save
```

That's it.

---

## ⭐ Support the project

If YT Music Tagger is useful to you, consider giving the repository a ⭐.

Bug reports, ideas and suggestions are welcome through GitHub Issues.
