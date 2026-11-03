# Changelog

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
