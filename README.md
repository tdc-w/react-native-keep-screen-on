# react-native-keep-screen-on
Allows for the selective toggling of the KEEP_SCREEN_ON flag.

***CURRENTLY ANDROID ONLY***

## Installation ##

`npm install react-native-keep-screen-on --save`

### In `settings.gradle` add the following lines:

```groovy
include ':KeepScreenOn'
project(':KeepScreenOn').projectDir = new File(rootProject.projectDir, '../node_modules/react-native-keep-screen-on/android')
```

### In `build.gradle` add the following line:

```groovy
compile project(':KeepScreenOn')
```

### In `MainActivity.java` add the following lines:

```java
import com.gijoehosaphat.keepscreenon.KeepScreenOnPackage;
```

```java
new KeepScreenOnPackage(this)
```

## Example usage:

```javascript
import KeepScreenOn from 'react-native-keep-screen-on'
...
//Keep screen on...
KeepScreenOn.setKeepScreenOn(true)

//Reset to default behavior...
KeepScreenOn.setKeepScreenOn(false)
```

## TODO:
1. Add similar support to iOS
