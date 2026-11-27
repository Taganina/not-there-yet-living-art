# NOT THERE YET — LIVING ART

An experimental, browser-based generative artwork. Visitors can allow their device camera to detect body pose and influence the particle field in real time.

## Publish publicly with GitHub Pages

1. Create a **public** repository on GitHub, for example `not-there-yet-living-art`.
2. Upload the contents of this folder to the repository's **root**. Make sure `index.html` is at the root (not inside another folder).
3. In the repository, open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select branch **main** and folder **/(root)**, then click **Save**.
6. Wait for GitHub Pages to publish. Your public URL will look like:
   `https://YOUR-GITHUB-USERNAME.github.io/not-there-yet-living-art/`

## Use the camera

- Open the published `https://` address in Safari (iPhone) or Chrome/Edge (desktop).
- Tap **START CAMERA & BODY TRACKING** and grant camera permission.
- On iPhone, use Safari directly. If opened inside another app's mini-browser, choose **Open in Safari**.
- The first launch needs an internet connection to load MediaPipe and its pose model.
- Camera permission is granted separately by each visitor and device.

## Privacy

This site processes camera frames in the visitor's browser for pose detection. It does not send or store camera video. Do not publish a privacy statement that promises more than this code does if you later add analytics, hosting-side scripts, or other services.

## Current prototype limitations

This is an experimental visual-art prototype, not a production-hardened installation. Tracking quality depends on lighting, camera position, device performance, and browser support. The camera preview is not displayed. The artwork is generated locally in the browser. Body sensitivity is increased by default; use the Body sensitivity slider to adjust the reaction.
