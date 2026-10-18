# For My Dear Sisukaaa ❤️ — Birthday Surprise Website

A static, mobile-friendly romantic birthday website made with HTML, CSS and vanilla JavaScript. It works on GitHub Pages and needs no backend or build tools.

## Files

- `index.html` — the complete website (styles and JavaScript are included).
- `photos/` — the seven original photographs supplied for this website.
- `photos/memory-01.jpg` through `photos/memory-07.jpg` — the gallery photo files.

## Passcode

The playful passcode is `1910`. This is **not real security**: the passcode is checked in browser-side JavaScript, so anyone who views the page source can find it. It is intended only as a fun surprise.

## Publish from an Android phone using GitHub Pages

1. Open GitHub in your browser and sign in.
2. Open the repository you want to use, or create a new repository (for example, `sisukaaa-birthday`).
3. If there is an existing `index.html`, open it and choose the pencil/Edit button. Replace all its content with the contents of this project's `index.html`, then commit the change. Alternatively, delete the old file and upload the new one.
4. Upload the `photos` folder with all seven `memory-*.jpg` files. On mobile, if GitHub won't upload a folder directly, open the repository, choose **Add file → Upload files**, select the seven images from the `photos` folder on your phone, and preserve the filenames. If needed, create the `photos` folder first using **Add file → Create new file** and name it `photos/keep.txt`; upload the photos into that folder, then you can leave or delete `keep.txt`.
5. Commit the uploaded photos.
6. In the repository, open **Settings → Pages**.
7. Under **Build and deployment**, choose **Deploy from a branch**. Set branch to **main** and folder to **/(root)**, then save.
8. Wait a few minutes. The Pages section will show the published URL, typically `https://YOUR-USERNAME.github.io/REPOSITORY-NAME/`.
9. Open that URL on your phone. Test passcode `1910`, all Continue/Back buttons, candle interaction, and every photo. Try it in a private/incognito tab too.

### Important upload note
The website expects these exact relative paths:
- `photos/memory-01.jpg`
- `photos/memory-02.jpg`
- `photos/memory-03.jpg`
- `photos/memory-04.jpg`
- `photos/memory-05.jpg`
- `photos/memory-06.jpg`
- `photos/memory-07.jpg`

Keep the spelling and capitalization unchanged. GitHub Pages paths are case-sensitive.

## Optional background music

The website intentionally does not autoplay music and works without an audio file. To add a royalty-free instrumental you are licensed to use:

1. Put your audio file in the `photos` folder and name it `love-melody.mp3`.
2. In `index.html`, find the commented line:
   `<!-- <source src="photos/love-melody.mp3" type="audio/mpeg"> -->`
3. Remove the `<!--` and `-->` around that line.
4. Commit the change and the MP3. Tap **Play music** on the site to start; tap again to pause.

Do not upload a commercial/copyrighted song unless you have permission to use it. Music is optional and never blocks navigation.

## Photo captions

Captions are in the `captions` array near the top of the JavaScript in `index.html`. To change a caption, edit the matching quoted string. The website includes the supplied photos as-is; the gallery uses `object-fit: cover` inside portrait cards and opens the full image in a lightbox when tapped.

## Troubleshooting

- **Photos missing:** Confirm the images are inside a folder named `photos` at the repository root and filenames match exactly.
- **Pages URL gives 404:** Check Settings → Pages is set to `main` and `/(root)`, then wait a few minutes.
- **Old page still appears:** Refresh the page; on Android Chrome, try a private tab or clear site data for the Pages URL.
- **Music button says to add a file:** This is expected until you add `photos/love-melody.mp3` and uncomment the audio source.
- **Passcode isn't accepted:** Enter `1910` using standard digits.
