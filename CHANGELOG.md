# Changelog

All notable changes to Dhunik will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [unreleased]

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