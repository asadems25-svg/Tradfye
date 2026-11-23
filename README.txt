TRAD FYE ANDROID WEBVIEW PROJECT

This is a simple Android app shell named "Tradfye". It opens:
https://tradfye.com/

WHAT IT DOES
- Opens the website inside the app.
- Supports the Android Back button.
- Opens links to other domains in the phone's browser.
- Uses HTTPS only and disables file/content access in the WebView.

IMPORTANT
The app does not unlock private beta access or bypass the website's access-code gate.
The website currently identifies itself as a private beta, so its own access requirements
will still apply. This wrapper does not connect a wallet, place trades, or store passwords.

BUILD APK
1. Install Android Studio on a computer.
2. Open Android Studio > Open, then select this "TradfyeAndroid" folder.
3. Allow Android Studio to sync Gradle and install any requested Android SDK.
4. Select Build > Build Bundle(s) / APK(s) > Build APK(s).
5. Android Studio will show the generated APK location.

Requirements: Android Studio with JDK 17 and Android SDK Platform 35.
Package: com.tradfye.app


CLOUD BUILD NOTE
A GitHub Actions workflow is included at .github/workflows/build.yml.
However, this project still needs a Gradle Wrapper (gradlew, gradlew.bat and
gradle/wrapper files) before the workflow can build. Upload this folder to a
GitHub repository, add the Gradle Wrapper, then run Actions > Build Tradfye APK.
Download app-debug.apk from the workflow's Artifacts section.
