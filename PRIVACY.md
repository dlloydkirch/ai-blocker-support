# Privacy policy: AI Detector & Blocker

_Last updated: November 1, 2026_

AI Detector & Blocker checks images, videos and text on the pages you visit for signs that they were made with AI, then tags, blurs or hides them. This policy explains what the extension does with data. The short version: **the developer collects nothing**, checks run on your device, and content leaves your device only if you set up an optional "deep check" service yourself.

## What happens on your device

- **Page content.** The extension reads the images, videos and text on pages you visit so it can check them. On social and video sites (such as X, Instagram, YouTube and Reddit) that includes the text of the post around an image, the site's own AI labels and reader-added notes. This happens inside your browser and nothing is kept except the saved checks described below.
- **Image and video files.** To read an image's or video's metadata (for example Content Credentials or AI-generator tags), the extension downloads the start of the file again from the same address the page uses, much as your browser already does to display it. Like your browser, it sends that site's cookies with the request, so images that need you to be signed in can be checked; the request goes only to the site that serves the file. Images that carry Content Credentials are downloaded whole, so their signature can be checked.
- **Content Credentials verification.** When an image carries Content Credentials, the extension checks its digital signature on your device, using the official C2PA software and a copy of the C2PA trust list that ships with the extension. It does not look anything up online to do this.
- **Enhanced text detection (off by default).** If you choose to download the on-device text model (about 138 MB, after a confirmation that states the size), the extension downloads it from Hugging Face (huggingface.co and its download network, hf.co) and stores it in your browser. Hugging Face receives ordinary download requests, which include your IP address; nothing about the pages you read is sent. The model then runs only on your device. **Settings → Remove model** deletes it.
- **Saved checks.** Results for images and videos already checked are stored on your device for up to 7 days, at most about 2,000 items (around 8 MB), so repeat images don't need checking again. Each saved result contains the media's web address and the reasons for its verdict. You can delete them at any time with **Settings → Clear saved checks**, and they're removed when you uninstall the extension.
- **Settings and API keys.** Your settings and any API keys you enter are stored in your browser's local extension storage. They are not synced to other devices.

None of this is sent to the developer or anyone else.

## Optional deep checks (off by default)

If you choose to add an API key for a deep-check service in Settings, the extension sends content to that service **when you click "Deep check"**, or automatically if you turn on "Run deep checks automatically":

| Service | What is sent | Website |
|---|---|---|
| Hive | the image (or its web address), or a frame captured from a video | <https://thehive.ai> |
| Sightengine | the image (or its web address), or a video frame | <https://sightengine.com> |
| GPTZero | the text being checked | <https://gptzero.me> |
| Anthropic (Claude) | the image, video frame or text, plus the reasons the extension already found and the page address | <https://www.anthropic.com/legal/privacy> |

Content is sent directly from your browser to the service you chose, using your own account and API key. The developer never receives it. Those services handle it under their own privacy policies (linked from their websites) and your agreement with them. In Firefox, the extension asks for your permission before any content is shared this way.

## "Wrong? Report it"

The report button opens a pre-filled form on GitHub, in the public repository [dlloydkirch/ai-blocker-support](https://github.com/dlloydkirch/ai-blocker-support), so anyone can read reports once they're submitted. It contains the verdict, the reasons for it, the website's domain name and the extension's version. It does **not** include the page address, the image or video address, or the text. Nothing is sent until you choose to submit the form yourself, and what you submit is governed by GitHub's privacy policy.

## What the extension does not do

- It does not collect, sell or share your browsing history or personal information.
- It contains no analytics, tracking or advertising.
- It does not load or run code from anywhere other than the extension itself.

## Permissions

- **Access to all websites:** to check content on the pages you visit and read media metadata.
- **Storage:** to keep your settings and saved checks on your device.
- **Context menus:** for the right-click "Check … for AI" items.
- **Scripting:** to keep new images and videos invisible until they're checked, only while you have chosen "Hide".

## Contact

Questions about this policy: open an issue at <https://github.com/dlloydkirch/ai-blocker-support/issues>.

## Changes

If this policy changes, the new version will be published at the same address with a new "Last updated" date.
