# Changelog

All notable changes to Dhunik will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [unreleased]

## [2.4.0] - 2026-10-30
### Added & Improved
- **Customizable Mini-Player Styles**: Personalize your bottom player aesthetic in Settings with selectable designs: Floating Stadium Pill, Full Width Docked Bar, or Floating Vinyl Disc
- **Mini-Player Quick Style Switcher**: Long-press anywhere on the bottom mini-player to instantly summon the style picker sheet with tactile haptic feedback
- **Interactive Track-Skip Swipe with Peek Glimpse**: Swiping left or right on the mini-player smoothly glides the album art and track details while revealing the incoming next or previous track's artwork, title, and tag in real time with spring physics, boundary resistance, and haptics, while keeping the docked player frame stationary
- **Dynamic Speed Dial Ambient Glow**: Home screen dual-tone ambient background dynamically extracts dominant palette colors from your Speed Dial song artwork with smooth cross-fade transitions and graceful fallbacks
- **Universal Playlist Import**: Transfer any public playlist from Spotify or YouTube Music with a single link
- **In-Playlist Song Recommendations**: Discover and add similar songs directly inside your playlists
- **Smart Link Detection Popup**: Automatically prompts to play or import copied Spotify & YouTube links on app open
- **Search Link Resolver**: Paste any Spotify or YouTube song link in search to play it instantly
- **Dynamic Queue Reordering**: Drag-and-drop to reorder songs in Up Next with tactile haptic feedback
- **Ghost Cache & Zero-Latency Gapless Audio**: Seamlessly pre-buffers upcoming queue tracks directly to a lightweight, bounded disk cache in the background, eliminating network buffering delays and dead air between songs with strict memory safety and LRU eviction
- **Apple Music-Style Animated Mesh Gradient**: Dynamic, fluid ambient glow on the Now Playing screen with smooth song-to-song color morphing, frosted diffusion, and zero-rebuild performance optimization
- **AutoEq Live Cloud Integration (8,800+ Headphone Models)**: Search and apply official laboratory-measured acoustic calibration data directly from Jaakko Pasanen's AutoEq database (oratory1990, Crinacle, Rtings, B&K 5128) with local disk caching and real-time hardware EQ sync
- **Interactive AutoEq Frequency Curve Preview**: Tap any headphone profile in the search list to inspect and preview its laboratory frequency response curve dynamically on the top visualizer in glowing amber before applying, complete with one-tap dismiss and zero audio interruption
- **Hardware-Level Loudness Normalization (Auto-Gain)**: Eliminates jarring volume jumps between quiet master tracks and loud YouTube rips automatically using Android's hardware `LoudnessEnhancer` (EBU R128 standard) with quick toggles in Settings and the Equalizer Effects lab
- **Auto-Detect Links Setting**: Toggle copied link prompts anytime in Settings
- **New Playlist Menu**: Tap "+" to create a blank playlist or import an existing one
- **Playlists Discovery Banner**: Quick-access banner in Playlists makes imports effortless
- **Instant Playlist Playback**: Newly imported playlists now load and stream immediately
- **Bottom Nav Search**: Moved search to the bottom navigation bar for quick access
- **Clean Library Page**: Revamped the library interface to reduce visual clutter
- **Speak to Search**: Search songs hands-free using your voice on the search page

## [2.3.1] - 2026-10-28
### Added & Improved
- **Headphone Comfort**: Reduces ear strain and headaches on headphones by blending stereo sound naturally, making music feel like it is playing in an open room
- **Warm Tube Sound**: Adds vintage warmth, rich depth, and crystal-clear vocals to any song
- **Working Equalizer**: Presets (Bass Boost, Pop, Rock, etc.) and custom sliders now genuinely tune your music in real time
- **Cleaner Stats**: Fixed artist names on the Listening Stats page to display clean text without unwanted characters or symbols

## [2.3.0] - 2026-10-28
### Added & Performance Optimizations
- **Massive APK Size Reduction**: Reduced primary download size from ~88.5 MB down to ~30 MB (over 65% reduction)
- **Multi-Architecture Release Packaging**: Automated builds for modern 64-bit devices (`arm64-v8a`), 32-bit devices (`armv7`), and universal fallback
- **R8 / ProGuard Code & Resource Shrinking**: Minified bytecode and eliminated over 16 MB of unused dependency code with zero regressions
- **Asset Optimization**: Converted core assets to high-efficiency WebP and pruned redundant legacy assets
- Guaranteed 100% stability across background playback, lock-screen notifications, YouTube stream extraction, and offline downloads

## [2.2.1] - 2026-10-26
### Fixed
- Fixed an issue where songs in the Speed Dial section would not play when tapped
- Fixed playback for YouTube tracks across Liked Songs, Recently Played, and Library
- Improved music playback reliability and smoother switching between offline and online streams
- Search improvements

## [2.2.0] - 2026-10-25
### Added
- Notification media controls like button: favorite or unfavorite tracks directly from your notification drawer
- Working shuffle mode in Now Playing with instant queue reordering and tactile feedback
- Modern floating pill toast notifications with subtle haptic feedback
- Playful heart bounce animation when liking or unliking songs in Now Playing
- Instant offline access to Home feeds and Quick Picks on app launch
- Speed dial section in the home screen

### Changed & Fixed
- Instant song liking: tapping the heart icon now reacts immediately with zero delay
- Fixed Liked Songs order: your newly liked tracks and playlists now appear right at the top
- Fixed duplicate border styling on floating toast notifications
- Dramatically faster app startup with a seamless, zero-flash launch transition
- Polished notification design and consistent aesthetics across the entire app

## [2.1.0] - 2026-10-08
### Added
- Complete UI/UX revamp of login page, auth sheets, and unauthenticated prompts
- Premium Google Sign-In button with built-in loading states and haptics
- Subtle studio ambient gradient glow at the top of Home screen
- High-resolution, zero-margin header logo asset
- Interactive scrubbable progress bar on Reels with live preview timestamp pill and haptic feedback
- Frosted glass animated Play/Pause center overlay indicator when Reels are paused
- Ambient Spotify-style spinning vinyl visualizer fallback for audio-only Reels tracks

### Changed & Fixed
- Fixed App Header logo alignment and spacing to match the 16dp content grid
- Standardized header height (56dp) with balanced search and avatar midline centering
- Fixed silent audio bug in Reels video playback caused by Android ExoPlayer audio focus preemption
- Optimized YouTube video stream fetching using dedicated video filtering and accelerated native stream URL resolution
- Parallelized Reels discovery prefetching with proactive background stream caching
- Restricted active video controller pool to prevent Android hardware MediaCodec decoder exhaustion

## [2.0.0] - 2026-10-03
### Added
- Major UI changes and optimizations
- Introducing new music source (YouTube)
- Introducing reels
- Brand new OLED dark design with ambient album art glow
- Floating MiniPlayer with swipe-to-skip gestures
- Redesigned Now Playing screen with modern controls
- Interactive synced lyrics with karaoke highlighting and tap-to-seek
- Revamped Song Details page with artist chips and recommendations
- Modern glassmorphic context menus for songs, albums, and playlists
- Home screen Quick Picks and Mood filters
- Account page with listening stats
- Revamp homepage, library, account, setting and all other pages

### Changed
- Sleek floating bottom navigation with Cupertino-style icons
- Improved lock screen controls and notifications
- Faster app navigation and deep linking
- Updated song recommendation engine

### Improvements
- Smoother 60fps animations across all screens
- More reliable high-quality (320 kbps) streaming

## [1.2.9] - 2026-08-07
### Fixed
- Cast bug fixes
### Added
- Account page revamp - stats section
- ui updates
- notification updates

## [1.2.8] - 2026-08-07
### Fixed
- Complete Cast Protocol Rewrite
- Seamless Playback Handoff
- Pause/Resume Reliability
- Background Operation fixes
- Enhanced Cast UX & Syncing

## [1.2.7] - 2026-07-26
### Added
- Welcome screen revamp
- Library page revamp
- Ability to load and play local musics
### Optimizations
- Progressbar updates

## [1.2.6] - 2026-04-25
### Added
- Extended lyrics display mode to now playing page

## [1.2.5] - 2026-03-15
### Added
- Support for Android Auto (Beta)
### Optimizations
- Enhanced lyrics caching mechanism enables faster lyrics loading
- Fixed song recommendations issues
### Removed
- Disabled support for spotify login due to some restrictions

## [1.2.4] - 2025-12-22
### Fixed
- Voice assistant not working
- Voice assistant orb UI
- Audio ducking when assistant speaks

## [1.2.3] - 2025-12-21
### Added
- PUSH notification support
- Restricted Vaayu assistant to authenticated users
### Fixed
- Other bug fixes and optimizations

## [1.2.2] - 2025-12-21
### Fixed
- APK installation failure on certain devices (e.g., Pixel 7) by enabling all APK signature schemes (v1, v2, v3)
- macOS build failure by updating deployment target from 10.15 to 11.0 (required for speech_to_text plugin)
- macOS app crash when clicking voice assistant button (disabled voice assistant on desktop platforms)

## [1.2.0] - 2025-12-20
### Added
- Introducing Dhunik voice assistant "Vaayu" - control your music with your voice
- New voices to the voice assistant Vaayu
- Mood pills to the homepage and removed hero carousel
- Lyrics transliteration feature
- Player controls to now playing bottom sheets
### Fixed
- Stability issue

## [1.1.7] - 2025-12-18
### Fixed
- Reduced minimum characters for search to 2
- Search data load issue when swiped between the tabs
### Added
- Reply mode to the party chat
- Recent Searches in search page
- Context menu to songs in search page
- Setting to toggle bottom player progress bar

## [1.1.6] - 2025-12-17
### Fixed
- Fixed routing inconsistencies for home page and library pages
- Recently played listing metadata issues
- Settings bottom sheet UI issues
- Auto scroll of non-synced lyrics
### Added
- Filter/sort options to library pages
- Revamped homepage and explore page
- Recently played song now appears on the homepage
- Album Context Menu for easy actions on the album page
- More options to playlist context menu
- New settings for more better control
- Dedicated Report Issue option in the account page for reporting any concerns

## [1.1.5] - 2025-12-16
### Fixed
- Cast device detection issue - Added missing permissions

## [1.1.4] - 2025-12-15
### Fixed
- Cast device detection issue

## [1.1.3] - 2025-12-13
### Fixed
- Song restart issue on reordering and adding to queue in party room
- Song reordering issues inside party room
- Blank screen when host ends the party
### Added
- Scroll to bottom inside Party chat
- Added cast support - beta

## [1.1.2] - 2025-12-12
### Fixed
- Tap detection issue with bottom player
- Intermittent No Internet Connection issue
- Artist page song deck view peek issue
### Added
- Swipe carousel effect to bottom player
- Remove song from queue inside party room (For Host)
- Swipe left to remove the song from the queue
- Revamped the Top Searches page
- Lyrics tab in Party Room


## [1.1.1] - 2025-12-11
### Fixed
- Input focus loss issue in chat
- Incorrect user name for typing indication
- Message appearing in reverse order

## [1.1.0] - 2025-12-10
### Added
- Added Song Party Feature - Listen and chat with friends together

## [1.0.10] - 2025-12-05
### Fixed
- Bug Fixes
- Fixed web app compatibility issues while playing the liked song

## [1.0.9] - 2025-12-05
### Added
- Carousel mode in Now Playing page allowing visible preview for user to change the prev/next songs

## [1.0.8] - 2025-11-30
### Fixed
- Synced lyrics scroll & positioning issue 
- Eager fetch lyrics after song is played

## [1.0.7] - 2025-11-30
### Added
- Song link sharing
- URL deeplinking with dhunik.in

## [1.0.6] - 2025-11-30
### Fixed
- App name appearing in lowercase in the app drawer

## [1.0.5] - 2025-11-30
### Added
- Offline playback support
### Fixed
- Fixed offline playback issues
- Other bug fixes and optimizations

## [1.0.4] - 2025-11-30
### Fixed
- Fixed app versioning issues
- Stable version
- May have known auth issue

## [1.0.3] - 2025-11-29
### Added
- Added in app updates

## [1.0.2] - 2025-11-29
### Fixed
- Bug fixes and optimizations

## [1.0.1] - 2024-11-28
### Added
- New user authentication system
- Dark mode support
- Push notifications for important updates

### Changed
- Improved app performance by 30%
- Updated UI design for better user experience
- Optimized image loading

### Fixed
- Fixed crash on startup for Android 12+ devices
- Resolved issue with login not persisting
- Fixed notification sound not playing

### Security
- Updated SSL certificate pinning
- Fixed vulnerability in password storage

## [1.0.0] - 2024-11-15
### Added
- Initial release
- Core features implemented
- Basic user interface
- Login and registration functionality

---

## Categories Explanation

- **Added** - New features
- **Changed** - Changes to existing functionality
- **Deprecated** - Features that will be removed in upcoming releases
- **Removed** - Features that have been removed
- **Fixed** - Bug fixes
- **Security** - Security improvements or vulnerability fixes