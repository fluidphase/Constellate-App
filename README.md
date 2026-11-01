# Constellate setup

1. Firebase console > create a project (free Spark plan).
2. Build > Authentication > Get started > turn on **Email/Password**.
3. Build > Firestore Database > Create database, then paste `firestore.rules` into the Rules tab and Publish.
4. Project settings > Your apps > Add a **Web app**, copy the config values.
5. Open `www/index.html`, find `const FB={...}` near the top of the script, and replace the PASTE_ values (apiKey, authDomain, projectId, appId).
6. Push to GitHub. Actions > "Build Android APK" > run > download `constellate-apk` from the artifacts.
7. For the website, host the `www` folder (Firebase Hosting or GitHub Pages) and add that domain under Authentication > Settings > Authorized domains.

Accounts use a username + password. Behind the scenes the username becomes a private email address, so there is no password reset.
