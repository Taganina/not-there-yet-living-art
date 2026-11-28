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


## The Watching Portrait

The project includes `portrait.jpg`, an artwork supplied for this installation. The portrait is rendered as the main artwork; the camera's pose landmarks estimate the visitor's position and gently shift the painted irises so the portrait appears to follow the viewer. The camera is processed locally in the browser.


## The Living Face update

The application now uses MediaPipe Face Landmarker in addition to Pose Landmarker. The visitor's face position, approximate size and head roll drive a smoothed transform of the complete original portrait. This replaces the earlier synthetic eye overlays. Face landmarks are processed in the browser; the camera stream is not uploaded by this app.


## Living Face 2.5D update

The portrait is rendered as a triangle mesh. Face-landmark head-turn estimates drive subtle deformation around the painted face, while visitor position shifts the whole artwork. This is a 2.5D illusion, not true 3D reconstruction: one flat image cannot reveal hidden side surfaces or unseen facial details. A more lifelike turn requires a manually prepared depth map with separated layers, or a 3D model based on the painting.
