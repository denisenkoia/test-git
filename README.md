# Voice Guide


### Release

***Android***
- path: C:\androidKey\voiceGuideReleaseKey.jks
- password: 123456
- alias: key0
```
tns build android --release --key-store-path C:\androidKey\voiceGuideReleaseKey.jks --key-store-password 123456 --key-store-alias key0 --key-store-alias-password 123456
```

***IOS***


### Build Option

***При сборке нового приложения меняем файлы***
- package.json (id)
- AndroidManifest.xml (android:label) 
- Info.plist (CFBundleDisplayName, CFBundleName)
- constant.js (DESTINATION_ID, APPLICATION_ID, NOTIFICATION_SUFFIX, NOTIFICATION_ID)

***LvivGuide (branch lviv-guide)***
- id: com.bs.voiceguidelviv
- android:label: "LvivGuide"
- CFBundleDisplayName: "LvivGuide"
- CFBundleName: "LvivGuide"
- DESTINATION_ID: 6;
- APPLICATION_ID: 2
- NOTIFICATION_SUFFIX: 'LVIVGUIDE'
- NOTIFICATION_ID: parseInt('LVIVGUIDE', 32)

***KrakowGuide (branch krakow-guide)***
- id: com.guidexp.krakowguide
- android:label: "KrakowGuide";
- CFBundleDisplayName: "KrakowGuide";
- CFBundleName: "KrakowGuide";
- DESTINATION_ID: 26;
- APPLICATION_ID: 5;
- NOTIFICATION_SUFFIX: 'KRAKOWGUIDE';
- NOTIFICATION_ID: parseInt('KRAKOWGUIDE', 32);

***VoiceGuide (branch voiceguide)***
- id: com.bs.voiceguide
- android:label: "VoiceGuide";
- CFBundleDisplayName: "VoiceGuide";
- CFBundleName: "VoiceGuide";
- DESTINATION_ID: undefined;
- APPLICATION_ID: 3;
- NOTIFICATION_SUFFIX: 'VOICEGUIDE';
- NOTIFICATION_ID: parseInt('VOICEGUIDE', 32);

***VoiceGuide (branch europe-guide)***
- id: com.bs.voiceguideeurope
- android:label: "EuropeGuide";
- CFBundleDisplayName: "EuropeGuide";
- CFBundleName: "EuropeGuide";
- DESTINATION_ID: undefined;
- APPLICATION_ID: 4;
- NOTIFICATION_SUFFIX: 'EUROPEGUIDE';
- NOTIFICATION_ID: parseInt('EUROPEGUIDE', 32);


### Stack

* Nativescript
* Angular
* Node 8.11.2
* npm 5.6.0


### Run ###

***Android***
```
tns run android
```

***IOS***
```
tns run android
```


### Build

***Android***
```
tns build android --bundle
```

***IOS***
```
tns prepare ios --release
```


### CLI generate component

* ng g component components/my-component --skipImport=true