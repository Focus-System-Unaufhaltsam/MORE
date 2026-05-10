# Firebase Setup – MORE UNAUFHALTSAM

## Connected project

- Project ID: `mg-challenge`
- Auth domain: `mg-challenge.firebaseapp.com`
- Storage bucket: `mg-challenge.firebasestorage.app`
- App ID: `1:472289048663:web:c91710542408c80d2c4b12`
- Leaderboard collection: `leaderboard_more-v1`

## Required console settings

1. Open Firebase Console.
2. Select project `mg-challenge`.
3. Enable Firestore Database if it is not active.
4. Go to Authentication → Sign-in method.
5. Enable Anonymous sign-in.
6. Go to Firestore Database → Rules.
7. Replace the rules with the content of `firestore.rules`.
8. Publish.

## Deployment

Copy all files into the GitHub Pages repository root. Do not upload the folder as a nested folder.

The game reads and writes scores through Firebase from `index.html`.
