# Changelog

Each version's section becomes the notes the app shows for that update (`npm run release:manifest`). Write it for players, not developers.

## [0.1.1]
- **Update announcement:** a new version now shows in the middle of the window when you open Nyarchive, with what's new and an Update now button. It downloads, installs and restarts by itself; your clips, settings and Pro stay.
- **Discord status:** friends who see you using Nyarchive get a "Get Nyarchive" button under your status.
- **Community:** Nyarchive's TikTok, YouTube and GitHub, as small icons at the bottom of the sidebar and in Settings → Community. A Discord server is coming soon.

## [0.1.0]
First public version.

- **Clip Studio:** instant replay, recording, screenshots, system sound and microphone on separate tracks, global hotkeys, a folder per game, HDR10 capture and crash recovery.
- **Editor:** a multitrack timeline with trims, splits, transforms, colour, speed, text, fades, keyframes and effects (denoise, sharpen, AI upscaling, frame interpolation, motion blur), plus a music search over your own songs.
- **Compressor:** compress to an exact file size, constant quality or a bitrate, with sample encodes and batches.
- **AI tools:** Real-ESRGAN upscaling and RIFE smooth motion, installed with one click.
- **Themes:** anime presets, your own picture as the background with matched colours and gradients, saved themes, cat ears and paw prints.
- **Setup:** one-click FFmpeg install in Settings → Encoders & FFmpeg.
- **Updates:** checks for new versions at startup (you can turn this off) and installs them with one click.
- **Nyarchive Pro:** an optional one-time purchase (14.99 €, one PC at a time, movable) for AI video upscaling, AI smooth motion, your own gradients, your own sounds and a custom logo. Everything else is free. AI picture upscaling stays free. Settings → Nyarchive Pro compares Free and Pro, activates your key and lets you move it to another PC.
- **Tip jar:** a link to Ko-fi, for voluntary tips.
- **4K:** record and export in 4K and up to 144 fps with Pro. Nyarchive checks which of your encoders can handle 4K and tells you if one can't. Free records and exports up to 1080p at 60 fps.
- **Watermark:** recordings, replays, screenshots and exports carry a small Nyarchive watermark. Change its size and position (or drag it) in Settings → Watermark; Pro can remove it or show your own logo.
- **Themes:** the option to follow Windows' light/dark mode was removed; your current theme stays. UI gradients are part of Pro.
- **Nyarchive Pro page:** Pro has its own page, one click from the crown in the sidebar, and the tip jar has its own button right below it. Custom background pictures (with the app's colours matched to them) are now part of Pro.
- **Reminders:** Nyarchive Free shows a short reminder about Pro and the tip jar at launch and every 5 to 15 minutes. With Pro you can switch them off.
- **Notifications:** a bar shows how long a notification stays. Choose 3 to 10 seconds, or keep them until you close them (Settings → Behaviour).
- **Watermark:** a new size or position now applies straight away, also to instant replay that is already running. The editor shows the watermark on top of your edits, where the export will have it.
- **Screenshots:** like Snipping Tool, the screen freezes the moment you press the key; drag out the area you want or click "Whole screen". The watermark sits in the corner of what you saved, and with the taskbar hidden it stays on the screen instead of the empty space the taskbar left.
- **Instant replay in full-screen games:** when a game takes over the screen (e.g. Rocket League in full screen), Windows ends the screen capture. Nyarchive used to keep buffering sound only, so saving a replay said "no footage". It now starts the capture again by itself within a few seconds.
- **Replays end at the key press:** when a game keeps the graphics card busy, the encoder can fall a few seconds behind. Saving a replay now waits for those seconds instead of cutting them off.
- **Hotkeys:** a key Nyarchive already uses (say F1) can be set again: clicking a hotkey box releases Nyarchive's own keys while it waits. If another copy of Nyarchive is still running (an older install in the tray, or the Pro test build), the hotkey warning says so.
- **Nyarchive Pro can be bought:** Buy Pro opens the checkout, and the key from the purchase e-mail activates Pro. Manage my devices opens the page where you can free a PC.
- **Pro switching off:** a refunded or revoked key now turns Pro off within the hour (and when you open the window again), and a notification tells you that you're back on Free.
- **Screenshots:** the area selection comes up the instant you press the key; the frozen picture follows a moment later and you can start dragging right away. A shutter sound plays when the screenshot is taken (choose it in Settings → Sounds, "Screenshot taken"). Screenshots are also copied to the clipboard, with a notification; switch it off in Settings → Capture.
- **Replays under heavy load:** when the graphics card can't keep up with the capture settings next to a game, Nyarchive now says so once and offers 60 fps or SDR capture. A frozen capture restarts after 8 seconds instead of 14, and a replay that ends before your key press says so.
- **When Pro ends:** frame rate and resolution go back to Free's 60 fps and 1080p (also for a running instant replay), and your own logo leaves the Start menu, Windows search and the taskbar pin too.
- **Found a bug?** Settings → Privacy & diagnostics has the support address and how to report; the Pro page has it for key and purchase questions.
- **Pro switching off** now happens within 5 minutes while Nyarchive is open, and right away when you open the Pro page or come back to the window.
- **Your own logo** now also appears on the Start menu entry (what Windows search shows) and the taskbar pin, not only the desktop shortcut, and every change shows up straight away.
- **Sidebar:** the crown is solid gold and glows while Pro is active.
- **Clean screenshots:** with the taskbar hidden, the empty space it leaves is cut off the picture (not in full-screen games, where that space shows the game).
- **Help where you need it:** a small ⓘ next to settings, effects and encoder options explains them when you hover it, instead of lines of small text everywhere.
- **Tip jar:** follows your theme's colours. Ko-fi and the shop open only after a short "you're leaving Nyarchive" check that names the website.
- **HDR:** HDR recordings and screenshots are now as bright as Windows shows your screen (they were about 2.5× too bright).
- **Smooth 120 and 144 fps:** recordings and replays above 60 fps really have that many pictures now. Before, Windows' screen capture only delivered about 80 new pictures a second and repeated the rest, which looked laggy. This needs the new FFmpeg: Nyarchive offers the update (91 MB) once, and instant replay pauses only for the moment it is swapped in.
- **Your own FFmpeg:** when Nyarchive uses an FFmpeg it found on the PC (for example from winget) that can't record smoothly above 60 fps, Settings → Encoders & FFmpeg now offers Nyarchive's own next to it.
- **Full-screen games:** when a game ends Windows' screen capture (Rocket League does this often), recording continues after a fraction of a second instead of waiting up to 2 seconds, so replays lose less.
- **HDR above 60 fps:** HDR records at the frame rate you set. If your PC's HDR capture delivers fewer new pictures than that (about 70 a second at 144 fps on an RTX 3050), Nyarchive says so once and offers SDR; nothing is changed by itself.
- **Replays end at the key press and play smoothly:** every 2 seconds of buffer used to lose 50-65 ms of picture where the pieces were joined (a small hitch every 2 seconds), and the end of the replay was cut by the sum of those, about 1.6 seconds per minute. The pieces are now joined without gaps, so the replay runs right up to your key press.
- **Capture settings apply right away:** a new frame rate, quality, encoder or HDR setting used to wait until instant replay was turned off and on, so choosing 144 fps kept recording 60. Instant replay now restarts with the new settings by itself (its buffer starts over); during a recording it waits until the recording ends.
- **Faster editor previews:** preview files for HDR clips are made about 17% faster and for SDR clips about 36% faster, and extra audio tracks no longer wait behind the picture.
- **Pro licence protection:** the licence file is now encrypted for your Windows account, so it can't be faked by hand. After this update Pro confirms your licence online once (a few seconds after start); without internet it keeps working for 30 days as before.
- **Faster exports with frame interpolation and motion blur:** these effects can only use one processor core, so exports that use them are now rendered in several parts at once (as many as your cores and free memory allow) and joined without a visible seam. The sound is mixed in one piece, so it stays in sync.
