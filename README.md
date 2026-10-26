# Lacuna — Daily Words for Android

Lacuna is a minimalist Android app with a home-screen widget that displays one uncommon, meaningful word each day, its definition, and a poetic interpretation.

## What is included
- Native Android app written in Kotlin.
- Home-screen widget designed for a dark charcoal / vintage literary look.
- 30 curated entries, including pronunciation, part of speech, definition, and poetic interpretation.
- Daily selection based on the date, so the same word appears in the app and widget on a given day.
- WorkManager periodic refresh for the widget.

## Build an installable APK
This environment does not include the Android SDK or Gradle, so an APK has not been compiled here. Build it using Android Studio:

1. Install Android Studio on a computer from https://developer.android.com/studio
2. Extract this ZIP.
3. In Android Studio, choose **Open** and select the `LacunaDailyWords` folder.
4. Let Gradle sync and install any requested Android SDK platform (API 35) and build tools.
5. Select **Build > Build Bundle(s) / APK(s) > Build APK(s)**.
6. When it finishes, choose **locate** in the notification. The APK is normally at `app/build/outputs/apk/debug/app-debug.apk`.

## Install on your Samsung phone
1. Transfer `app-debug.apk` to your Samsung Galaxy A25.
2. Open the APK from My Files and approve installation from that source if Android asks.
3. Open Lacuna once.
4. Return to the home screen, long-press an empty area, choose **Widgets**, find **Lacuna**, then drag the widget onto the home screen.
5. Resize it if desired.

## Notes
- The word list is bundled offline; no account or internet connection is needed.
- Android controls the exact time a widget refreshes. WorkManager is battery-aware and may refresh later than exactly 24 hours; opening/placing the widget also updates it.
- The current version cycles through 30 curated words. It is a starter app, not a Play Store release.
