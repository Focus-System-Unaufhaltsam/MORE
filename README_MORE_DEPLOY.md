# MORE / UNAUFHALTSAM Focus System

This ZIP is built from the Eddie UNAUFHALTSAM blueprint and converted into a MORE-themed, high-contrast focus game.

## Important brand/legal note

No official MORE trademark, logo, product packaging, registered mark or licensed brand asset is included. The included `more_mark.svg` and `more_wordmark.svg` are original placeholder assets created for this deploy package.

Use official MORE assets only if you have explicit rights or permission. Replace `more_mark.svg` in the root folder and keep the same filename if you want the game boxes to use a licensed mark.

## What changed

- Root deploy structure, no broken `eddie-main` nesting.
- English UI, with `UNAUFHALTSAM` intentionally kept as the only German brand word.
- MORE-themed black / cream / signal-orange visual system.
- New Firebase collection: `leaderboard_more-v1`.
- Social @ leaderboard and one-slot ranking retained.
- Wall HUD removed; Wall 30 remains a myth / challenge statement only.
- `legal.html` and `privacy.html` include the LinkGuard only on legal/privacy pages.

## Deploy

Upload all files in this ZIP directly into the repository root:

```txt
Focus-System-Unaufhaltsam/eddie/
```

The root must contain:

```txt
index.html
config.js
legal.html
privacy.html
firestore.rules
more_mark.svg
more_wordmark.svg
```

Then publish the included `firestore.rules` in Firebase.

## Bio link

```txt
https://focus-system-unaufhaltsam.github.io/eddie/
```

After deployment hard-refresh with `Ctrl + F5` or test in an incognito window.


## Firebase connection

This build is connected to the Firebase project `mg-challenge` with app ID:

`1:472289048663:web:c91710542408c80d2c4b12`

It uses the Firebase compat SDKs in `index.html` so it works directly on GitHub Pages without a build step.

Required Firebase settings:

1. Firestore Database must be enabled.
2. Authentication → Sign-in method → Anonymous must be enabled.
3. Publish the included `firestore.rules` file in Firebase Console.
4. The leaderboard collection is `leaderboard_more-v1` and will be created automatically on first valid score save.
