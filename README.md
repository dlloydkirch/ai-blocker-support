# AI Detector & Blocker

A browser extension for Chrome, Edge and Firefox that spots AI-generated images, videos and text as you browse, and tags, blurs or hides them. Checks run on your device; the developer collects nothing.

- **Download:** the latest version is on the [Releases](https://github.com/dlloydkirch/ai-blocker-support/releases) page. Chrome Web Store and Firefox Add-ons listings are coming.
- **Privacy policy:** [PRIVACY.md](PRIVACY.md)
- **Wrong verdict, bug or question:** [open an issue](https://github.com/dlloydkirch/ai-blocker-support/issues/new/choose). The extension's "Wrong? Report it" button fills one in for you. Issues are public, so leave out anything you don't want others to see.

## Installing a release by hand

1. Download `ai-detector-blocker-<version>.zip` from [Releases](https://github.com/dlloydkirch/ai-blocker-support/releases) and unzip it.
2. **Chrome or Edge:** open `chrome://extensions` (or `edge://extensions`), turn on **Developer mode**, click **Load unpacked** and pick the unzipped folder.
3. **Firefox:** open `about:debugging#/runtime/this-firefox`, click **Load Temporary Add-on** and pick `manifest.json` in the folder. Temporary add-ons are removed when Firefox restarts; the Add-ons listing installs it permanently.

`test-page.html`, attached to each release, is a page of sample content to see the extension working.

This repository holds the public pages and releases. The source code is kept elsewhere.
