# Neon Snake Android project

This project wraps the existing Neon Snake HTML game as an Android app using Capacitor and builds a debug APK with GitHub Actions.

## For a beginner using only an Android phone

1. Sign in to GitHub in your browser and create a new repository named `neon-snake-android`.
2. Upload the contents of this folder to the repository (not the ZIP file itself). Make sure `.github/workflows/build-apk.yml` is included.
3. In the repository, open **Actions**. If prompted, enable workflows.
4. Choose **Build Neon Snake APK** and tap **Run workflow**. You can also let it run after pushing to the `main` branch.
5. Wait for the run to finish with a green check mark.
6. Open the completed run, scroll to **Artifacts**, and download `neon-snake-debug-apk`.
7. Extract the downloaded ZIP on your phone. Tap `app-debug.apk` to install it. Android may ask you to allow installs from your browser or file manager; only enable this for the source you trust.

## Notes

- The APK produced is a debug APK for personal testing, not a signed release for Google Play.
- The app ID is `com.neonsnake.game`. Change it before publishing publicly.
- This workflow generates the Android project during the cloud build, so the Android Studio project is not included in this ZIP.
- If GitHub Actions is unavailable for the account/repository, a different cloud build service or a computer with Android build tools will be needed.
