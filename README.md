# GOTY Bingo

A one-page bingo card for the awards night. Everyone writes their own predictions, then crosses them off when they happen. A full row, column or diagonal plays the win animation and the sound.

## Put it online with GitHub Pages

1. Create a new public repository on GitHub.
2. Upload `index.html` and `1.mp3` to the root of the repo (keep the file name `1.mp3`).
3. Go to **Settings → Pages**. Under **Build and deployment**, choose **Deploy from a branch**, pick `main` and `/ (root)`, then save.
4. After a minute your site is live at `https://YOUR-USERNAME.github.io/REPO-NAME/`. Send that link to your friends.

## How it works

- **Add prediction** fills the next empty square. You can also tap any empty square.
- Tap a filled square to cross it off with a red X. Tap again to undo.
- **Edit squares** turns on edit mode: tap a square to change or delete it.
- Pick 3×3, 4×4 or 5×5. A line only counts when every square in it is filled and crossed.
- Each person's card is saved in their own browser (localStorage), so every friend has their own card on their own device. There is no server.
- The sound button mutes the win sound.
