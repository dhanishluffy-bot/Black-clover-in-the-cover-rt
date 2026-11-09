# Black Clover: Magic Wars (Android project)

A small landscape Android game prototype. It runs the included offline HTML5 battle game inside an Android WebView. It includes 10 rival stages, unlock progression, health bars, Asta's Sword Slash / Black Meteorite / Sword Block, and opponent turns.

## Build an APK in the cloud using only a phone

1. Sign in to GitHub in your phone browser and create a **new public repository** named `BlackCloverMagicWars`.
2. Upload the contents of this folder to the repository (not the outer ZIP folder). Make sure `.github/workflows/build-apk.yml` is included. GitHub's mobile website may offer **Add file → Upload files**; if hidden, enable the browser's desktop-site view.
3. Open the repository's **Actions** tab. If GitHub asks, enable Actions.
4. Choose **Build Android APK** → **Run workflow** → **Run workflow**.
5. Wait for the workflow to finish with a green check. Open that run, scroll to **Artifacts**, and download `BlackCloverMagicWars-debug-apk`.
6. Extract the artifact ZIP and install `app-debug.apk` on an Android device. Android may ask you to allow installation from your browser/files app.

The workflow uses GitHub-hosted Ubuntu, Java 17, Gradle 8.9, and Android Gradle Plugin 8.7.3. It builds a debug APK; no signing key is required for testing.

## Local build
Open this folder in Android Studio and run `gradle assembleDebug` (with Android SDK installed). APK output: `app/build/outputs/apk/debug/app-debug.apk`.

## Note
This is a playable prototype with original stylized placeholder fighter drawings, not official Black Clover artwork or an exact reproduction of the anime characters. It is not a published Play Store app.
