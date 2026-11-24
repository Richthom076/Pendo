# Pendo – dating app (web + iPhone + Android + PC)

One codebase: a web app (PWA) that runs on any phone or PC browser, and is
wrapped with Capacitor to produce an Android APK, built automatically by GitHub.

## 1. Put it on GitHub
1. Create a free account at github.com, then tap + > New repository. Name it `pendo`, keep it Public, create it.
2. On a PC: unzip this project, open the folder in a terminal and run:
   git init
   git add .
   git commit -m "First version"
   git branch -M main
   git remote add origin https://github.com/YOUR-USERNAME/pendo.git
   git push -u origin main
   (No Git? On the repo page choose "uploading an existing file" and drag in ALL files,
   including the hidden `.github` folder.)

## 2. Get the APK
1. Repo > Actions tab. "Build Android APK" runs by itself after each push (about 5-8 min).
2. Open the finished run > Artifacts > download `pendo-apk` (a zip) to your phone.
3. Unzip, tap `app-debug.apk`, allow "Install unknown apps" for your browser/Files app, install.

## 3. Website for iPhone and PC
1. Repo > Settings > Pages > Source: GitHub Actions.
2. After the "Deploy website" run: https://YOUR-USERNAME.github.io/pendo/
3. iPhone: open in Safari > Share > Add to Home Screen.
   Android/PC Chrome: menu > Install app.

## Next steps for a real dating site
This version is a working demo: sample profiles, data stored on the device only.
For real users you need a backend (Firebase or Supabase): sign-in with phone/email,
shared profile + photo storage, real matching and chat, moderation (report queue,
photo checks), a privacy policy and terms. Play Store release needs a signed release build.
