# Changelog

## [0.8.11] - 2026-11-04

#### Added
- **Trim camera edges**: Remove the left, right, top and bottom edges separately without enlarging the remaining image.

#### Changed
- **Organized camera settings**: Camera selection is available only in the Camera tab; appearance, trimming, display and satellite options are grouped in collapsible sections.
- **Consistent recording icon**: A red dot and white REC identify recording regardless of recording mode. Built-in icons now use colors.

#### Fixed
- **Display selection**: Small rounding differences in screen dimensions no longer prevent matching the selected monitor.

## [0.8.10] - 2026-11-04

#### Added
- **Multiple audio sources for video recordings**: Select and mix up to 20 devices and apps, each with its own volume.
- **Audio format options**: Choose MP3 bitrate, sample rate and channels; WAV additionally supports 16-bit and 24-bit audio.
- **Mouse pointer capture**: Turn mouse pointer capture on or off for screen recordings.

#### Changed
- **Clearer help and update settings**: Feedback and support are now under Help and Logs. Update settings and status are arranged vertically.
- **Recording settings**: Audio and video recordings have separate save locations and relevant format settings.

#### Fixed
- **Mouse pointer during screen recordings**: Screen capture uses a different method intended to prevent cursor flicker while preserving the pointer in the recording.
- **Camera preview**: Camera access errors are displayed and the preview can be retried.
- **Folder picker**: The dialog opens at the configured recording folder.

## [0.8.8] - 2026-11-03

#### Changed
- **Organized recording settings**: Sources, Audio, Video, Formats, Save Locations and Camera now have dedicated tabs.
- **Separate recording folders**: Audio and video recordings can use separate save locations. The existing folder is initially retained for both.

#### Fixed
- **Camera preview restored**: The live preview is visible again in camera settings and is released when leaving the Camera tab.
- **Camera satellite shown only when needed**: The satellite appears only during an active or paused camera recording, or a screen recording with a camera, when satellite display is enabled.
- **Move Orbit right up to the taskbar**: The visible wheel and an active camera satellite can be moved directly to the taskbar without covering it.

## [0.8.7] - 2026-11-03

#### Changed
- **Movable Notification and Alert Windows**: Error and status dialogs can now be freely dragged across screens and multiple monitors using the mouse.
- **Safe Video Conversion & Source Retention**: When converting MKV recordings to MP4, the original file is strictly verified before deletion and safely retained if any stream discrepancies are detected.
- **Reliable Update Checksum Verification**: The built-in updater resolves and verifies installer checksums even more reliably, ensuring that corrupted or incomplete downloads are safely blocked.

#### Fixed
- **Camera Device Conflicts Between Preview and Recording**: The settings camera preview and the satellite camera blob can now run alongside video recording without "camera busy" errors.
- **Protection Against In-Recording Camera Switches**: Switching the active camera in settings is safely locked while a recording is in progress, preventing capture interruptions.
- **Audio in Video Recordings**: Audio handling when starting and stopping video recordings has been stabilized.
- **Segment Retention on Unexpected Capture Errors**: If a video recording process is interrupted unexpectedly, all intact recorded video segments are safely preserved on disk.

## [0.8.6] - 2026-11-03

#### Added
- **H.265 / HEVC Video Encoders**: Added support for modern hardware-accelerated H.265 / HEVC encoding (NVIDIA NVENC, Intel Quick Sync, AMD AMF) and CPU encoding for smaller file sizes at identical visual quality.
- **Camera Zoom and Pan Framing**: Smoothly zoom in on the camera image and adjust horizontal and vertical pan offsets in video settings to frame the shot exactly as desired.
- **Adjustable Camera Blob Size and Position**: Dedicated sliders in video settings allow fine-tuning of the camera blob size and placement angle around the wheel.

#### Changed
- **Click-Through in Transparent Window Areas**: The transparent desktop space outside the visible wheel and camera bubble now passes mouse clicks directly through to underlying windows and the desktop.
- **Clean Settings Window Docking**: The Orbit wheel now docks to the settings window with an exact 16-pixel visual gap without empty space.
- **Expanded Alert Dialogs**: Error and status alerts are now presented in an enlarged, scrollable dialog across the full screen overlay.

#### Fixed
- **Persistent Camera Display Resolved**: The camera preview at the wheel rim now only appears during active camera recordings and automatically dismisses when stopped.
- **Live Video Feed in Camera Blob**: During recordings, the camera blob displays the live camera stream instead of a static recording placeholder.
- **16:9 Camera Clipping at 3 O'Clock and 9 O'Clock**: Rectangular camera bubbles at 0° and 180° angles are no longer clipped by window borders.
- **Buffer Overflows and Recording Aborts**: Resolved audio buffer overflows and unexpected recording interruptions during simultaneous webcam and desktop capture.
- **Restoring Collapsed Wheel**: Re-opening the wheel via the global shortcut or system tray now reliably restores the wheel even when previously collapsed.

## [0.8.5] - 2026-11-03

#### Fixed
- **Build and Release Pipeline Stabilization**: Fixed an automated packaging issue so that all 0.8.4 improvements (orbital camera blob, webcam hardware exclusivity, and window focus stabilization) are reliably delivered via the built-in updater.

## [0.8.4] - 2026-11-02

#### Added
- **Orbital Camera Blob on the Orbit Wheel**: The live camera preview now docks directly onto the Orbit wheel and can be freely rotated 360° around the wheel using mouse drag-and-drop.
- **Customizable Camera Shapes (16:9 or Circle)**: The camera blob can be switched between a widescreen 16:9 rounded rectangle and a compact circular shape.
- **Wheel Collapse Mode**: Clicking "Close" collapses the main Orbit wheel while keeping only the camera preview floating on the desktop.
- **Hide Camera Blob in Screen Recordings**: When "Hide Orbit from screen recordings" is enabled, the docked camera preview is also invisible in the recorded output.

#### Fixed
- **Recording Aborts with Camera and Screen Capture**: Resolved camera device exclusivity conflicts ("Device in use") and subsequent FFmpeg terminations (SIGTERM) when starting recordings.
- **Window Shifting with Discord and Spotify**: Maximized application windows now keep their full screen size and position instead of being de-maximized and shifted 10% downwards and sideways.

## [0.8.3] - 2026-11-02

#### Added
- **Hide Orbit from Screen Recordings**: Option in video settings to make the Orbit wheel invisible during screen captures so it does not appear in recorded videos.
- **Floating Live Camera Preview**: Option to display your own webcam feed as a floating bubble directly on the desktop during recordings.
- **Camera Zoom and Crop (100% – 300%)**: Zoom slider in video settings to smoothly crop and focus the camera frame (e.g. tightly on the face).
- **Drag & Drop Camera Positioning**: The camera overlay position can now be adjusted directly via mouse drag-and-drop in the settings preview.
- **Direct MP4 Recording**: When MP4 is selected, recordings are written directly to MP4 without an intermediate MKV and without leftover duplicate files.

#### Fixed
- **Camera Buffer Overflow Under Load**: Resolved capture interruptions caused by real-time buffer overflows during combined webcam and screen recordings.
- **Audio/Video Lip Sync in Recordings**: Audio and video now remain strictly synchronized even under CPU spikes or dropped frames.
- **Spotify & Discord Window Focus**: Minimized windows now reliably stay open in the foreground when brought up from the Orbit wheel instead of immediately closing.
- **Windows Permission Prompts (UAC)**: Administrator permission prompts no longer crash screen recordings; capture pauses safely and resumes automatically.
- **Source Deletion After Remuxing**: When configured, the original MKV source file is now reliably removed after a successful and verified MP4 remux.

## [0.8.2] - 2026-11-02

#### Added
- **Bring running apps to the foreground**: Clicking an already running application on the Orbit wheel (such as Spotify or Discord) now immediately restores and focuses its existing window instead of launching a duplicate instance.

#### Changed
- **Always hide wheel on app launch**: Launching an application from the Orbit wheel now hides the wheel across all close modes, including when "Stay open" is active.

#### Fixed
- **Missing app icons in the app launcher**: Fixed missing icons for Microsoft Store apps (such as Spotify), Squirrel apps (such as Discord), Steam games, and Windows system tools.

## [0.8.1] - 2026-11-02

#### Added
- **Recording settings on the wheel**: A new tile in the recording menu opens the video and recording settings directly in the right section.
- **Expanded video options**: Added more resolutions (4K UHD, 1440p QHD, 480p SD) and frame rates (24 FPS, 120 FPS) along with clear explanations for encoders and quality presets.

#### Changed
- **Integrated alert dialogs**: Recording alerts and error messages now appear as a movable dialog directly in front of the Orbit wheel instead of hidden system message boxes.

#### Fixed
- **Screen and camera recording startup**: Fixed recording aborts when capturing across multiple displays, while the camera preview is active, or with slower-initializing cameras.
- **Automatic camera selection**: Starting a camera recording without a prior selection now automatically uses the first available camera.

## [0.8.0] - 2026-11-02

- Screen and webcam recording: Capture displays and windows directly from the Orbit wheel in sync with system audio and microphone.
- Smart camera overlay: Add a picture-in-picture webcam with circular, rounded, or custom mask shapes into your recordings.
- Hardware-accelerated video: Automatic detection and use of NVIDIA NVENC, Intel QuickSync, and AMD AMF for smooth 1080p recording at 60 FPS.
- Lossless MP4 remuxing: Safely repack robust MKV captures into MP4 immediately after recording or manually in settings.
- Visual progress ring: The rainbow border along the Orbit wheel displays real-time progress while remuxing or converting.

## [0.7.1] - 2026-11-02

- Made the shortcut for opening the Orbit wheel configurable in settings.
- Fixed the layout of release notes in the update window.

## [0.7.0] - 2026-11-02

- Smart app catalog on the wheel: Clicking the plus icon in the apps menu now opens a searchable catalog of all installed Windows programs to quickly add apps with their authentic icons.
- Reliable launch of protected Windows tools: Task Manager and system utilities now launch cleanly from the wheel without permission errors.
- Improved file display: Longer filenames wrap cleanly onto two lines, hover tooltips show the complete path, and files automatically display the authentic icon of their default application (e.g. media player for videos).
- Full usability during recordings: Apps, files, and bookmarks can now be managed on the wheel even while an audio recording is active.
- Window dragging during saving: The Orbit wheel can now be grabbed and moved by its center hub even while converting or saving a recording.
- Fixed notification and error banners being clipped at the bottom window edge.

## [0.6.1] - 2026-11-01

- Fixed the layout when quickly adding files and apps.
- Improved the jiggle animation and remove button in edit mode.

## [0.6.0] - 2026-11-01

- Dedicated sections for Bookmarks and Files: Alongside apps, you can now manage web bookmarks and files directly on the Orbit wheel and in settings, opening in your default browser or associated application.
- Quick in-wheel management: Plus and minus controls in the wheel center allow fast item creation (including one-click paste from clipboard) or removal using an iOS-style jiggle edit mode.
- Corrected app icons: Resolved authentic icons for Brave and the Windows Task Manager.

## [0.5.9] - 2026-11-01

- Enhanced download stats on the wheel: The center hub now shows real-time download speed, estimated remaining time, and transferred data volume alongside the percentage.

## [0.5.8] - 2026-11-01

- Connected Orbit wheel tiles without gaps and smoothed transitions between descriptions.
- Improved feedback submission and privacy in diagnostic logs.
- Fixed restarting an update download after cancellation.
- Improved the app launcher for scripts.

## [0.5.7] - 2026-11-01

- Stabilized wheel dragging under Windows scaling.
- Made update downloads and feedback submission more reliable.
- Improved app launch error reporting and added changelogs to the app.

## [0.5.6] - 2026-11-01

- Show download progress on the wheel after closing the update window.
- Added automatic update checks when opening the wheel and in the background.

## [0.5.5] - 2026-11-01

- Improved wheel dragging, docking and transitions between displays.
- Made the app launcher in settings easier to navigate.

## [0.5.4] - 2026-11-01

- Added original Windows application icons to the app launcher.
- Improved update notifications and interaction between the wheel and settings.

## [0.5.3] - 2026-11-01

- Added paging from the wheel center, app renaming and more display options.

## [0.5.2] - 2026-11-01

- Added and improved wheel dragging, positioning and app file selection.

## [0.5.1] - 2026-11-01

- Fixed an app launcher startup error.

## [0.5.0] - 2026-11-01

- Added the app launcher, multiple wheel pages and configurable tile counts.
- Added session logs and a feedback section.

## [0.4.2] - 2026-11-01

- Added the new Omega Orbit icon for the application and notification area.

## [0.4.1] - 2026-11-01

- Show download, conversion and saving progress on the edge of the Orbit wheel.

## [0.4.0] - 2026-11-01

- Open the new update window directly from the Orbit wheel.
- Improved the display of release notes during and after downloads.
- Improved the update section in settings.

## [0.3.0] - 2026-11-01

- Show progress while converting and saving recordings.
- Fixed an error when stopping a recording more than once.
- Check for and download updates directly from the Orbit wheel.
- Made audio settings easier to navigate and added help and a log.
- Fixed a Windows startup issue.

## [0.2.0] - 2026-11-01

- Open the Orbit wheel at the mouse pointer with a keyboard shortcut.
- Record audio from several sources at once into a single file.
- Choose WAV or MP3 in audio settings or directly from the audio wheel.
- Find saved recordings in Explorer from the audio wheel.
- Configure the recording folder, language, wheel size and Windows startup.
- Download and install updates directly in Omega Orbit.
