School Ride (KidRide) package
=============================

This ZIP contains two folders:
 - kidride-pwa/       -> Progressive Web App (open index.html in a browser or host it)
 - kidride-android/   -> Android-ready web assets and Capacitor skeleton (open README below)

PWA usage:
1. Open kidride-pwa/index.html in a browser (Chrome recommended).
2. To host and enable "Install" behavior, upload the folder to any static host (Netlify, Vercel, Firebase Hosting).
3. The app registers a Service Worker for basic offline caching.

Android (Capacitor) usage (recommended workflow on your development machine):
1. Install Node.js & npm.
2. In a working directory, create a new vite project or use this folder as your 'www' build output.
   Example quick setup:
     - mkdir schoolride-capacitor && cd schoolride-capacitor
     - npm init -y
     - npm install @capacitor/core @capacitor/cli
     - Copy the contents of the 'www' folder from this package into schoolride-capacitor/www
     - npx cap init "School Ride" "com.schoolride.app"
     - npx cap add android
     - npx cap copy
     - npx cap open android
3. Android Studio will open the fully native project. Build and run on an emulator or device.

If you'd like, I can:
 - provide the ready-to-import Android Studio project (this requires a larger generated project)
 - or further customize the UI, add real-time backend, auth, or push notifications.

Enjoy testing the School Ride pilot!