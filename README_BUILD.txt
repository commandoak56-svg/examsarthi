EXAMSARTHI ANDROID APP - BUILD PACKAGE

What this is
- Android WebView app shell for the current Examsarthi preview website.
- Includes the website in app/src/main/assets/index.html.
- Includes an Examsarthi launcher icon and GitHub Actions workflow to build a debug APK in the cloud.
- This is a prototype, not a production learning platform.

IMPORTANT LIMITATIONS
- No production backend, real student login, cloud sync, secure admin dashboard, or verified online content publishing is configured.
- Local demo data stays on the device/browser storage and may be lost if app data is cleared.
- Debug APK is for testing. A public Play Store release requires signing, privacy policy, testing, and production backend/security work.

Build APK using a GitHub account (works from a phone browser)
1. Extract this ZIP on your phone or computer.
2. Create a new empty repository on GitHub named examsarthi-android.
3. Upload all files and folders from this project into the repository root. Ensure build.gradle, settings.gradle, app/ and .github/ are at the root, not nested in another folder.
4. Open the repository's Actions tab and choose "Build Examsarthi APK".
5. Tap "Run workflow" if it has not started automatically.
6. When the run finishes successfully, open the run and download the artifact named "Examsarthi-debug-apk". Extract it to get app-debug.apk.
7. Install the APK on Android. If prompted, allow installation from that browser/files app only if you trust the file you just built.

If Actions is disabled, open repository Settings > Actions > General and enable actions.

Alternative: Open the project root in Android Studio with Android SDK installed and run `gradle assembleDebug`.

This workflow creates a DEBUG APK, not a Play Store signed release. Do not enter real student/private data until backend authentication and security have been implemented and tested.
