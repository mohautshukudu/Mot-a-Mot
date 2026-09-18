# Mot à Mot

A free, no-account web app for learning the ~2,000 most common French words, ranked by how often they appear in film and TV subtitles.

## How it works

- **Batches.** You start with 10 words. When you finish a batch, your first-try average sets the size of the next one:
  - 90% or more: 10 more words
  - 80% or more: 5 more
  - under 65%: 5 fewer

  Batches stay between 10 and 50 words, and you can change the cap in Settings.
- **Study.** Each word has an emoji, a Wikipedia photo (nouns only), its gender, audio and an example sentence. You can hide the meanings to quiz yourself.
- **Three levels per batch, in order:**
  1. **Match**: pick the meaning, or pick the French word.
  2. **Listen**: hear the word and pick its meaning.
  3. **Type**: see the English and type the French. Missing accents still count as correct, but the app flags them.

  You need your pass mark (80% by default, right first time) on all three levels to unlock the next batch. Anything you miss comes back in the same test until you get it right.
- **Review.** Finished words come back on a spaced schedule: 1, 3, 7, 14, 30, 60 and then 120 days.
- **Word forms.** Example sentences highlight the word, and when it appears in a changed form (suis for être, chiens for chien) the app says which form it is. Tap the ? for a short grammar primer.
- **Read.** The Read tab pulls a random French Wikipedia article, highlights the words you've learned, and tells you what share of the passage you know. Tap any highlighted word for its meaning and pronunciation.
- **Already know some French?** Go to Settings → "Already know some French?" to skip ahead.
- **Progress** is saved in your browser. Settings → Backup gives you a code you can use to move your progress to another device.

## Put it on GitHub Pages (about 5 minutes, no coding)

1. Sign in at github.com and click **New repository**. Name it `mot-a-mot`, make it **Public**, and click **Create repository**.
2. On the new repo page, click **uploading an existing file**. Drag in `index.html`, `words.js` and this `README.md`, then click **Commit changes**.
3. Go to **Settings → Pages**. Under "Build and deployment", set Source to **Deploy from a branch**, Branch to **main** and the folder to **/ (root)**, then click **Save**.
4. Wait about a minute and refresh. Your app will be at `https://YOUR-USERNAME.github.io/mot-a-mot/`.
5. **On iPhone:** open that link in Safari, then Share → **Add to Home Screen**. It opens full screen like an app.

To update the app later, upload the new files to the repo again. Your progress isn't affected because it's stored on your device.

## Audio

Pronunciation uses your device's built-in French voice, so it's free and there's no API.

- **iPhone:** Settings → General → Read & Speak → Voices → French. Download a French (France) voice (the "Enhanced" and "Premium" ones sound best), then fully close the app and reopen it.
- **Android:** Settings → Text-to-speech → install French.

## Credits

- **Word ranking:** OpenSubtitles 2018 French frequency list by Hermit Dave ([hermitdave/FrequencyWords](https://github.com/hermitdave/FrequencyWords), CC BY-SA 4.0), grouped into dictionary forms using spaCy's lookup tables.
- **Meanings and example sentences:** written for this app.
- **Photos:** loaded live from Wikipedia.
