# Flutter-camera-and-location-permission-and-showing-geolocation-to-the-user
Hereby this app, asks the user for camera permission aswell as location permission, and then shows the users location in mathematical coordinates
This has been forked and then modified from this: https://www.youtube.com/watch?v=AoMVol8ZpaA


This is an SS from the actual app: https://imgur.com/lGYoDCI.png


HOW TO DO IT: Since I can't upload this to github as it's too big, I just uploaded main.dart and other dart files, and pubspec.yaml. Just do:


flutter create yourAppName

Then copy these dart files into lib folder, and replace the pubspec.yaml.

Required permissions are this, which must be put inside the projectName/android/app/src/main/AndroidManifest.xml : 

<uses-permission android:name="android.permission.CAMERA" />
<uses-permission android:name="android.permission.ACCESS_BACKGROUND_LOCATION" />
<uses-permission android:name="android.permission.ACCESS_COARSE_LOCATION" />
<uses-permission android:name="android.permission.ACCESS_FINE_LOCATION" />

Not all of these location permissions might be required. I didn't test each of them. You can try each other and find the right one then remove the useless ones.
