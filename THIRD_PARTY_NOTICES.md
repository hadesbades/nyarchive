# Third-party notices

Nyarchive itself is proprietary software under the end-user licence agreement in [EULA.txt](EULA.txt). The open-source components built into the app, with their full licence texts, are listed in [THIRD_PARTY_LICENSES.txt](THIRD_PARTY_LICENSES.txt). Both files are also installed next to `nyarchive.exe`.

## Programs Nyarchive downloads on request
Nyarchive does not ship these programs. When you click Install in Settings, it downloads them directly from their publishers' release pages, checks the SHA-256, and unpacks them into `%APPDATA%\app.nyarchive.desktop\models`. Nyarchive runs them as separate programs and does not link against them.

| Program | Licence | Downloaded from |
|---|---|---|
| FFmpeg 9.0.2, gyan.dev "full" shared build | GPL-3.0 (includes x264, x265 and other GPL components) | https://github.com/GyanD/codexffmpeg/releases/tag/9.0.2 (source: https://ffmpeg.org/download.html and https://www.gyan.dev/ffmpeg/builds/) |
| Real-ESRGAN ncnn-vulkan 0.2.5.0 | BSD-3-Clause | https://github.com/xinntao/Real-ESRGAN/releases/tag/v0.2.5.0 |
| RIFE ncnn-vulkan 20221029 with the RIFE 4.6 model | MIT | https://github.com/nihui/rife-ncnn-vulkan/releases/tag/20221029 |

The FFmpeg licence text is kept with the download (`models\ffmpeg\LICENSE`). You can also use an FFmpeg you installed yourself (for example `winget install Gyan.FFmpeg`). If you redistribute Nyarchive *together with* an FFmpeg build, you must comply with that build's licence: provide its licence text and the corresponding source or a written offer.

## Fonts
The interface bundles **M PLUS Rounded 1c** (© The M+ Project Authors) and **Nunito** (© The Nunito Project Authors), both under the SIL Open Font License 1.1, via the Fontsource packages. Text clips in the Editor use fonts installed on your system.

## Pictures
Background pictures you choose are copied into `%APPDATA%\app.nyarchive.desktop\backgrounds` for your own use as wallpaper. Pictures found through the image search belong to their creators; Nyarchive does not redistribute them.
