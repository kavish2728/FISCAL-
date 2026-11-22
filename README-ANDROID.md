# Fiscal Fable CFO — Internal Workspace (Android)

This is the Android packaging setup for the lightweight internal workspace. It is **not client-facing** and contains no AI agents.

## Features
- Overview: client/report/task counts
- Clients: add and manage internal client records
- Reports: create, edit, save, search and print/export reports
- Tasks: assign tasks to clients and track due dates
- Documents: report/document list view
- Local-only storage; no login, backend, cloud sync or AI

## Build an APK using GitHub Actions
1. Extract this ZIP and upload the contents to a new GitHub repository (the `index.html` must be at repository root).
2. Open the repository's **Actions** tab.
3. Select **Build Fiscal Fable CFO Android APK** and press **Run workflow**, or push to `main`/`master`.
4. Wait for the build to complete successfully.
5. Open the completed workflow run and download the artifact named **Fiscal-Fable-CFO-Android-APK**.
6. Extract the artifact and install `app-debug.apk` on Android. If prompted, allow installation from that source.

## Local Android build
Requires Node.js 20+, Java 21, and Android Studio/Android SDK.

```bash
npm install
npx cap add android
npx cap sync android
cd android
./gradlew assembleDebug
```
APK output: `android/app/build/outputs/apk/debug/app-debug.apk`.

## Storage note
The app uses browser local storage inside the Android WebView. Data is saved on this device and may be lost if app storage is cleared or the app is uninstalled. This version does not synchronize across devices or team members. Back up important client information separately.
