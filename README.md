# SmartFood Android V2 — source code

## Build an installable APK
1. Install Android Studio on Windows, macOS, or Linux (a computer is required for this build).
2. Extract this ZIP and open the `smartfood_android_v2` folder in Android Studio.
3. Wait for Gradle sync. JDK 17 and Android SDK 35 are used; install missing SDK components if prompted.
4. Choose **Build > Build Bundle(s) / APK(s) > Build APK(s)** (menu names vary by Android Studio version).
5. Find `app/build/outputs/apk/debug/app-debug.apk` and copy it to your Android phone.
6. Open the APK on your phone and allow installation from that source when Android prompts. Only install APKs you built or trust.

## Features
Offline recipes, ingredient photo capture/preview, manual photo checklist, pantry inventory, macro and calorie calculations, custom meal diary, calorie target estimator, weight chart, backup export/restore. Data is stored locally in WebView storage.

## Important limitations
- **No automatic AI recognition**: image recognition requires a secured online backend/API and consent/privacy design. The photo is used for manual review.
- Nutrition values are approximate hardcoded examples, not verified USDA food composition records; actual portions and cooking methods change totals.
- The personalized calorie calculation is an estimate for adults, not individualized medical advice. It uses Mifflin–St Jeor and activity multipliers.
- No precompiled APK included. No cloud sync. Uninstalling or clearing data may erase records. Export backups regularly.
- This is a WebView-based Android app, not a native Jetpack Compose UI.
