# firebase

For google Vision API to Work:

-Need to create the project on "https://console.cloud.google.com/"
-Enable Billing
-Enable Google Vision API
-setup autentication 
-create service account
- user service key in firebase .env file

For more Infomration https://cloud.google.com/vision/docs/setup

Running locally

Franciss-MBP-2:firebase-trying-again francisbooth$ cd functions/
Franciss-MBP-2:functions francisbooth$ ls
index.js		node_modules		output.txt		package-lock.json	package.json
Franciss-MBP-2:functions francisbooth$ npm run serve

> functions@ serve /Users/francisbooth/Projects/firebase-trying-again/functions
> firebase emulators:start --only functions

i  emulators: Starting emulators: functions
✔  hub: emulator hub started at http://localhost:4400
⚠  Your requested "node" version "8" doesn't match your global version "12"
✔  functions: functions emulator started at http://localhost:5001
i  functions: Watching "/Users/francisbooth/Projects/firebase-trying-again/functions" for Cloud Functions...
⚠  functions: Your GOOGLE_APPLICATION_CREDENTIALS environment variable points to /Users/francisbooth/.gcloud/keys/hcl-commerce-speech-vision-4c7d2f395024.json. Non-emulated services will access production using these credentials. Be careful!
✔  functions[app]: http function initialized (http://localhost:5001/myfirst-firebase/us-central1/app).
✔  emulators: All emulators started, it is now safe to connect.


Publish to firebase

https://firebase.google.com/docs/hosting/deploying

$> firebase deploy

or

$> firebase deploy functions