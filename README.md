# Auvix Music by Kazee — Android APK project

This is an Android app project that bundles the Auvix interface inside an Android APK. It opens as an app (not in the phone's external browser) and includes the current prototype UI.

## Included in this prototype
- Dark navy / neon blue Auvix branding
- Demo sign-in screen (not real authentication)
- Song-link saving
- Audio file picker from Android
- Playlists and favorites UI
- Playlist snapshot sharing/import UI
- Browser local storage for demo data

## Important limitations
- This project is APK-ready source code, not a compiled APK. This environment has no Android SDK/Gradle installed, so it cannot compile the APK here.
- The email/password screen is only a local demo; it does not create secure accounts or sync data between phones.
- Playlist sharing is a text snapshot. Real shareable links between devices require an online backend.
- A URL by itself is not the song audio. Offline playback needs audio actually saved locally or a provider's authorized offline feature.
- Imported audio files selected in this prototype are playable for the current app session, but persistent media-library management and robust background playback need native implementation.
- Streaming-provider links (such as YouTube or Spotify) are not converted to audio files and their access rules are not bypassed.

## Build an APK using GitHub Actions (phone-friendly)
1. Create a new empty GitHub repository.
2. Upload the contents of this folder to the repository root (including `.github/workflows/android.yml`).
3. Open **Actions** and enable GitHub Actions if prompted.
4. Run **Build Auvix Music APK** (or push to the `main` branch).
5. After the workflow succeeds, open the run and download the artifact named `auvix-music-debug-apk`.
6. Extract the artifact ZIP and install `app-debug.apk` on your Android phone. If Android asks, allow your browser/file manager to install apps from that source.

Do not share your GitHub password or access tokens. Only install APKs you built and trust.
