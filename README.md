### Building

1. Make sure you have [gradle](http://www.gradle.org/) installed and in the path.

2. Download and extract [Android SDK](http://developer.android.com/sdk/index.html).

3. Set `ANDROID_HOME` environment variable to the SDK location.

4. Install the following packages using `Android SDK manager`. You can run it with `$ANDROID_HOME/tools/android update sdk`

    |Package                   |Version                                                      |
    |--------------------------|-------------------------------------------------------------|
    |Android SDK Tools         |latest                                                       |
    |Android SDK Platform-tools|latest                                                       |
    |Android SDK Build-tools   |same version as `android/buildToolsVersion` in `build.gradle`|
    |Android API / SDK Platform|same version as `android/compileSdkVersion` in `build.gradle`|

5. Build APK

        gradle build

6. Install APK to the attached device

        gradle installDebug