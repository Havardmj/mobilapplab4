# mobilapplab4
School lab assignment 4.

Linter Error : Cannot resolve Symbol 'Theme' in styles.xml = <style name="AppTheme" parent="Theme.AppCompat.Light.DarkActionBar">

Accordin to https://developer.android.com/guide/topics/ui/look-and-feel/themes This is right syntax, and the app works, without throwing any build exception/error.

Linter Error : 'Incompatible Gradle Versions' : Newest version of com.firebaseui:firebase-ui-database/auth is incompatible with deployed sdkversion 27. Search of compatible version, and got 3.3.0. This version synced and builds. But the Linter throws error, and suggest too switch to to appcompat-v7:27.1.1 instead of appcompat-v7:27.1.0 , but then I get Sync error instead. Current libs is accepted by gradle sync/build - Lint also complains about Obsolete build, but this build support current SdkVersion for my phone.

Lint throws warnings on test cases set up by android studio.

Lint throws many Spelling typos : e.g project package name : 'com.example.havardmj.chatapplication'






Inspired by https://www.youtube.com/watch?v=Xn0tQHpMDnM
