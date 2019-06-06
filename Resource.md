## Status Bar is White

  `<item name="android:statusBarColor">@android:color/transparent</item>`
Remove above line of code in `values/styles/styles.xml(v21)`


## DataBinding doesn't generate the Binding classes
  
  Enable Databinding in app manifest, 
  Make the layouts as dataBinding layouts,
  Clean & Rebuild the project
  
## MainApplication class is not found the project

  Create a custom class `AppX` extends from Application()
  In the Manifest file, under `<Application>` tag, add `android:name=".AppX"`

## Browse the App's database in Android studio
   - open `Device File Explorer`, which is now built-in directly into Android Studio.
   - navigate to /data/data/[your.package.name]/databases folder, right-click on your database file and Save As… (The app must be compiled using a debug build variant, otherwise you won't be able to browse its data directory.)
   - install database navigator plugin or hit [https://sqlitebrowser.org/]
