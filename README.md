# emojicon
Android library to show emojicon dialog box over soft keyboard

## Forking
This is a fork from `https://github.com/ankushsachdeva/emojicon`. What I have done is create an empty Android Project on Android Studio, then import the module `lib` and `example` from original repository. I didn't change anything on the main source code.


## Install

config your project's gradle
```
	allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}
  ```
Add this to your app module's gradle

	dependencies {
	        compile 'com.github.IHNEL:emojicon:-SNAPSHOT'
	}
  
  
 
## Troubleshoutting 
If you got `Manifest merge error` when rebuild your project,just add `tools:replace="android:icon"` to the file `AndroidManifest.xml` of Android Application module.

`Manifest merger failed : Attribute application@icon value=(@drawable/icon_app) from AndroidManifest.xml`


```
<application
        ...
        tools:replace="android:icon">
```
