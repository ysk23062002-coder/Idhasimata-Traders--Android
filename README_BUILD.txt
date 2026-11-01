IDHASIMATA TRADERS - ANDROID PROJECT + MOBILE CLOUD BUILD

This ZIP contains Android source code and a GitHub Actions workflow. It is NOT itself an APK.
The workflow can build a debug APK on GitHub's cloud servers, so a laptop is not required.

MOBILE-ONLY BUILD STEPS (Android phone):
1. Download and extract this ZIP on your phone (Files app > Downloads > ZIP > Extract).
2. Open https://github.com in Chrome and sign in or create a free account.
3. Create a NEW repository named idhasimata-traders-android. Choose Public for the simplest free Actions setup. Do not add a README, license, or .gitignore.
4. Open the new empty repository. Choose Add file > Upload files.
5. Upload the CONTENTS of the extracted IdhasimataAndroidProject folder, including the hidden .github folder. The .github/workflows/android-apk.yml file is essential. If the phone's file picker hides .github, use GitHub's browser upload in desktop-site mode, or tell me what you see and I will guide you.
6. Commit the upload to the main branch.
7. Open the repository's Actions tab. Select "Build Idhasimata Traders APK" and tap "Run workflow" if it has not started automatically.
8. Wait for the workflow to finish with a green check mark. Open that successful run and scroll to Artifacts.
9. Download "Idhasimata-Traders-debug-APK". Extract the downloaded artifact ZIP; inside is app-debug.apk.
10. Tap app-debug.apk and allow Chrome/Files to install apps from this source if Android asks. Only install the APK you built from your own repository.

BUILD DETAILS:
- Uses Java 17, Android SDK Platform 35, Android Gradle Plugin 8.7.3, and Gradle 8.9.
- GitHub Actions workflow uses the official Gradle setup action and uploads the APK as a workflow artifact.
- Workflow source: .github/workflows/android-apk.yml

IMPORTANT LIMITATIONS:
- This is a prototype app, not a production ordering system.
- Real OTP authentication, backend/database, order storage, inventory, admin authorization, and payment processing are not implemented.
- Admin preview is not secure and must not be used to manage real customer data.
- UPI payment is not connected; WhatsApp order drafting and COD are demo-level only.
