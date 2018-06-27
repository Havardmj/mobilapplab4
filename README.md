# mobilapplab4
School lab assignment 4.

Linter Error : Cannot resolve Symbol 'Theme' in styles.xml = <style name="AppTheme" parent="Theme.AppCompat.Light.DarkActionBar">

Accordin to https://developer.android.com/guide/topics/ui/look-and-feel/themes This is right syntax, and the app works, without throwing any build exception/error.

Linter Error : 'Incompatible Gradle Versions' : Newest version of com.firebaseui:firebase-ui-database/auth is incompatible with deployed sdkversion 27. Search of compatible version, and got 3.3.0. This version synced and builds. But the Linter throws error, and suggest too switch to to appcompat-v7:27.1.1 instead of appcompat-v7:27.1.0 , but then I get Sync error instead. Current libs is accepted by gradle sync/build - Lint also complains about Obsolete build, but this build support current SdkVersion for my phone.

Lint throws warnings on test cases set up by android studio.

Lint throws many Spelling typos : e.g project package name : 'com.example.havardmj.chatapplication'

The Idea:

Users of the app can post text messages that are seen by everyone. The app is like a single chat room, that everyone having the app installed, participates in. When the app is in foreground, it works as real-time chat app, ie. messages appear as they happen, and the user can enter new messages. Self-messages should appear in the view, too. When the app is not in the foreground, the background service should periodically check for new messages (time to pull configured by preferences, similar to Lab 2). When new message is available, the Notification should be used, to communicate that to the user. The user can start the foreground activity from the Notification.

Checklist:

The repo URL is correct. The project has a Readme file. 

 The code is well structured, and well organised. 

 There are no secret credentials in the repository. 

 There are no Linter warnings, or, the warnings are documented and justified in the project Readme file. 

 The app starts and provides a user with a unique global nickname, that the user can edit/modify.

 The user is not able to modify previously chosen Nickname, after accepting it.  The nickname is stored in private preferences of the app. 

 The main screen of the app has two tabs with nice icons: Messages Feed, and Friends List. (Note: Everyone is everyone's friend and everyone follows everyone - one global chat room).

 The user can enter new message from the Feed tab. This can be achieved either inlined with the message list (the UI has the messages list and a TextEdit field with the button), or, through an Action Button that opens up a message editor/submit ability as separate from the List of messages. Discuss with the app author the choice they have made. 

 When new message is typed and submitted it automatically shows up in the message feed. (Note: self-messages are shown)

 When new message is typed and submitted it automatically shows up in the messages for the user nickname in the Friends list. 

 When the second app is installed (phone or emulator), the two participants can see each other messages, and they are shown in Friends List view. 

 The Friends List tab lists nicknames ONCE only (no duplications).

 When the app is gone from foreground, and new message is posted by another user, within the predefined timeframe, the background service will post a Notification that shows up on the user phone. The notification can be used to open the app (or bring it back to the foreground).


