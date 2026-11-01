# QuizForge

**A free quiz app and question bank creator for students.**
Build your own question banks, import them from CSV, and practise with quizzes that give instant explanations and track your progress. It works in the browser, installs on your phone like an app, and works offline after the first visit.

## Why it exists

QuizForge was created by **Vincent Akachukwu Daniel**, a university student just starting out. He wanted a way to practise on his own with questions collected from class lectures, textbooks and other places, keep them all in one spot, and share them with classmates. What began as a personal study tool is now free for anyone to use.

## Who it is for

- University and school students who want to practise past questions
- Study groups who want to share question banks
- Teachers and tutors who want a quick way to build quizzes

## Features

- **Question bank creator:** add questions with options, difficulty, subject, topic, an explanation and an optional image (snap a page from a notebook or paste one)
- **CSV import and export:** upload a file or paste CSV text directly, and download your bank as a backup
- **Quiz engine:** choose subject, topic, difficulty and number of questions, in practice mode (instant feedback) or exam mode (results at the end, with time per question)
- **Shuffled options** so the correct answer never sits in the same slot
- **Results and history:** score, topic breakdown, failed questions to review, retry, share or download
- **Math formatting:** `m^-2` becomes m⁻², `H_2O` becomes H₂O, `<=` becomes ≤, and more
- **Installable and offline:** add it to your home screen and keep studying without internet
- **Safe deletes:** deleting everything requires typing a confirmation word
- **Share, rate and support:** invite friends, rate the app, and support the creator

## Quick start

1. Open the app and go to the **Bank** tab.
2. Add questions with the form, or import a CSV.
3. Go to **Home**, pick a subject, level and number of questions, and start.

### CSV format

```
subject,topic,difficulty,question,A,B,C,D,correct,explanation,image
Science,Biology,Easy,Which organelle produces most of the cell's energy?,Nucleus,Mitochondrion,Ribosome,Golgi body,B,Mitochondria produce most of the cell's ATP.,
```

Only `question`, `A`, `B` and `correct` are required. `correct` is a letter from A to D. Use the **Download template** button in the Bank tab for a ready-made file.

## Files

| File | Purpose |
| --- | --- |
| `index.html` | The whole app |
| `manifest.webmanifest`, `icon-192.png`, `icon-512.png` | Make the app installable |
| `sw.js` | Offline support |
| `robots.txt` | Lets search engines index the app |

## Hosting

Upload all files to any HTTPS static host (GitHub Pages, Firebase Hosting, Netlify). Installing as an app needs HTTPS.

## Optional setup

Edit these values near the top of the script in `index.html`:

- `WA`: your WhatsApp channel link
- `CLD`: your Cloudinary cloud name and unsigned upload preset (for explanation images)
- `CREATOR_PHOTO`: link to your photo. Open the app's About page with `#owner` on the end of the address to upload one and get the link.
- `WEB3_KEY`: a free access key from [web3forms.com](https://web3forms.com) so ratings are emailed to you automatically. Without it, the rating opens the user's email app with the rating filled in.

## Your data

Questions, history and settings are stored in your own browser. Nothing is sent anywhere, except images (to your Cloudinary account) and ratings (by email).

## Coming next

A shared library of approved question banks, cloud saving, and more tools for studying with friends.

## Credits and copyright

Original idea, design and code by **Vincent Akachukwu Daniel**.
© Vincent Akachukwu Daniel. All rights reserved. Please share the link rather than copying or republishing the app as your own.
