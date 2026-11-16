# HISHH MONEY MANAGER — Android APK project

A lightweight native Android WebView wrapper around an offline-first finance tracker. It stores transactions in the app's local WebView storage on the device; no account, server, or network permission is required.

## Build an APK using only your Android phone (GitHub Actions)

1. Extract this ZIP on your phone (Files app → Downloads → ZIP → Extract).
2. In Chrome, sign in to GitHub and create a **new public or private repository** named `hishh-money-manager`.
3. Upload the **contents** of this folder (not the enclosing folder) to the repository. Make sure `.github/workflows/build-apk.yml` is included. GitHub's mobile website may hide dot-folders; if it does, use GitHub Desktop on a computer or upload the project using the GitHub web interface's Add file → Upload files after enabling hidden files in your file manager.
4. Open the repository → **Actions** → **Build HISHH Money Manager APK** → **Run workflow** (or wait for the push workflow).
5. Open the completed green workflow run → **Artifacts** → download `HISHH-MONEY-MANAGER-debug-apk`.
6. Extract the downloaded artifact ZIP. Tap `app-debug.apk` and allow Chrome/Files to install unknown apps if Android asks.

## Build on a computer with Android Studio

1. Open this project folder in Android Studio.
2. Install Android SDK Platform 35 and JDK 17 if prompted.
3. Run **Build → Build Bundle(s) / APK(s) → Build APK(s)**.
4. The debug APK is at `app/build/outputs/apk/debug/app-debug.apk`.

## Features

- Monthly income, expenses, and net balance
- Income sources: Business, Freelancing / Editing, Pocket Money, Other Income
- Expense categories and descriptions
- Monthly savings target with progress bar
- Recent transactions and individual deletion
- CSV export and JSON backup
- Local-only storage; no sign-in or internet connection required

## Important storage note

Data is stored locally inside the app. Clearing app storage or uninstalling the app can erase it. Use **Backup data** regularly and keep the JSON backup somewhere safe. This starter app is not a bank account or accounting/tax system.
