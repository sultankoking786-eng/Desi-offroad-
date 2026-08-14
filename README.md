# Desi Offroad — Standalone APK Project

Backend dependency removed; profile/progress use localStorage.

## Build
1. Install Node.js + Android Studio.
2. In this folder run `npm install`.
3. Run `npx cap add android`.
4. Run `npx cap sync android`.
5. Run `npx cap open android`.
6. Android Studio → Build → Generate APK(s).

Note: Three.js is still loaded from jsDelivr, so first launch needs internet.


## Phone-only GitHub Actions build

1. Create a GitHub repository.
2. Upload every file from this project, including `.github/workflows/android.yml`.
3. Open **Actions** in the repository.
4. Run **Build Desi Offroad APK** (or push to `main`).
5. After the workflow succeeds, open the workflow run.
6. Under **Artifacts**, download `desi-offroad-debug-apk`.
7. Extract the downloaded artifact and install `app-debug.apk` on Android.

This workflow builds a debug APK automatically; it does not sign a Play Store release APK.
