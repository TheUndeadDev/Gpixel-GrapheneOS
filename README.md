# Pixel 8 + GrapheneOS Welcome Guide

A small, phone-first static website for gifting a Pixel 8 with GrapheneOS. It has no build step, backend, analytics, or paid dependency. Google Fonts and the optional YouTube video embeds are third-party resources; YouTube content connects to YouTube when a video is loaded. The page remains readable if those resources are blocked.

## Personalize it

The welcome already addresses the recipient as **Crazy Cat Lady**. Open `index.html` and replace `[Your name]` with your sign-off. Read the guide once as the recipient would, especially the handoff note above the videos.

For the cleanest handoff, make sure your personal accounts and data are removed and the device is waiting at its initial setup screen. If the phone has already been used, back up anything you need before erasing it from Settings. A factory reset erases user data; it does not reinstall the operating system. Do not give the recipient your passcode or account credentials.

During setup, do not proceed if the phone reports that its bootloader is unlocked. GrapheneOS treats that as an incomplete installation; resolve it using the official installation guidance before the recipient adds personal data.

## Preview locally

Open `index.html` in a browser. No package install or server is required.

## Free hosting

### GitHub Pages

The site is already published at [the welcome guide](https://theundeaddev.github.io/Gpixel-GrapheneOS/) from [its GitHub repository](https://github.com/TheUndeadDev/Gpixel-GrapheneOS).

To publish updates without Git, open `index.html` in the repository, select the pencil **Edit this file** button, replace its contents with the local `index.html`, and commit. Repeat for `styles.css`. GitHub Pages is already enabled, so it will redeploy automatically; keep the same site URL and QR code. Allow a few minutes, then reload the live page.

For a new site, create a public repository, upload `index.html`, `styles.css`, and `README.md`, then open **Settings → Pages**. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and `/ (root)`, and save. The published address will look like `https://YOUR-USERNAME.github.io/REPOSITORY/`.

GitHub's setup instructions: [Creating a GitHub Pages site](https://docs.github.com/en/pages/quickstart).

### Cloudflare Pages

1. Create a GitHub repository containing the site files and connect it to Cloudflare Pages.
2. Choose **Create a project → Connect to Git** and select that repository.
3. Use no framework, leave the build command empty, and set the build output directory to `.` (the repository root).
4. Deploy. Cloudflare will provide a `*.pages.dev` URL.

Cloudflare's setup instructions: [Git integration](https://developers.cloudflare.com/pages/get-started/git-integration/) and [build configuration](https://developers.cloudflare.com/pages/configuration/build-configuration/).

Both providers can change their dashboards and free-plan terms, so check their current instructions if a label differs. Do not publish private information: anyone with the public URL can open the guide.

## Make the QR card

Wait until the hosted page works on a phone, then copy its final HTTPS URL (including the repository path for GitHub Pages). In Chrome or Edge, open that URL and use the browser's **Share → Create QR code** command. Download or print the QR and test it with a second phone before attaching it to the gift. The QR only contains the website address; it does not grant access to the phone or its data.

If the browser does not offer QR creation, use a reputable QR generator with the public URL, download a high-resolution PNG or SVG, and test it before printing. Avoid putting passwords or personal details in the QR code.

## Sources

The on-page technical and support links point to GrapheneOS and Google Pixel's official pages. GrapheneOS changes over time; follow its current documentation for details. This guide is an informal welcome, not a substitute for the project's documentation.