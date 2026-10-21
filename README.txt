CineCam AI - APK build (Capacitor)

Easiest (no installs): GitHub Actions
1. Create a free GitHub account and a new empty repository.
2. Upload ALL files from this folder (keep the .github folder) to the repository.
3. Open the Actions tab, run "Build APK" (it also runs on every upload).
4. When it finishes, open the run and download the "CineCam-AI-apk" artifact. Unzip it to get app-debug.apk.
5. Copy the APK to your phone, tap it, and allow "Install unknown apps" when asked.

On your own computer (needs Node 20, JDK 17, Android SDK):
  npm install && npx cap add android && npx cap sync android
  cd android && ./gradlew assembleDebug
  APK: android/app/build/outputs/apk/debug/app-debug.apk
