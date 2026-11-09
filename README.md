# One Pace · Universal Wano Viewing Hub

This repository now serves the **Universal Hub v4** at `index.html`. It contains 62 links in order and an HTML5 browser player for laptop Firefox/Chrome and TV browsers, plus the existing iPhone Infuse and VLC options.

## Episode order
- Wano 01–04: One Pace English dub.
- Wano 05–30: Muhn Pace English dub.
- Wano 31–62: One Pace English dub.
- Wano continues beyond episode 62. Later video sources have not been verified for this directory.

## Browser playback and captions
- Click **Watch in Browser** to open the built-in HTML5 player.
- Captions are fetched as SRT files from GitHub and synchronized in a screen overlay. A WebVTT track is also generated for native subtitle display where supported.
- The video is streamed from existing Pixeldrain direct-file links. **We have not confirmed that Pixeldrain permits browser playback from this GitHub-hosted page.** If the remote host blocks it, try the alternate host, direct file, or Infuse.
- Wano 01 uses `One_Pace_Wano_01_English_Dub_Captions_Corrected_v1.srt` (partially corrected, not fully proofread).
- Wano 02–04 and 31–62 except 53/55 use unreviewed AI-generated DubTitlerr transcriptions.
- Wano 05–30 use **Muhn Pace videos** with SRT timings made for a **different One Pace edit**. The caption timing has not been verified; simple shifting cannot necessarily fix edit differences.
- Wano 53 and 55 have **no matching SRT** in the catalog. Do not promise captions for them.

## Laptop, Chromecast and Fire TV
- **Laptop:** open the published hub in Firefox or Chrome; choose Watch in Browser. The local downloadable HTML may also work in desktop browsers if remote subtitle fetch is allowed.
- **Chromecast:** use Chrome on a laptop to **Cast screen** so the browser-rendered caption overlay is included. This is desktop/screen mirroring, *not* a native Chromecast receiver app. The laptop must remain on and audio sharing may need enabling.
- **Fire TV:** open the published URL in Amazon Silk; use the browser player. Silk can play HTML5 MP4, but success depends on Pixeldrain policies and TV codec support.
- **iPhone:** browser player may work, or use the previously tested **Infuse + SRT** fallback. The **VLC iPhone** button uses an iOS-specific URI and is not intended for desktop VLC.

## Publish the hub as a website

A repository file is not automatically a website. GitHub Pages must be enabled once:

1. Open this repository's **Settings** tab.
2. Select **Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**.
4. Set **main** and **/(root)**, then **Save**.
5. Wait for GitHub's confirmed published site address shown in Pages settings.

For this repository, the usual site address is `https://h94p57c6tg-design.github.io/one-piece-subtitles/` **only if GitHub Pages has successfully published it**.

## Notes

This repository is a player interface and link index only; no video files are hosted here. The third-party video sources and subtitle libraries may change, and the One Pace / Muhn Pace edits are unofficial.

**Local validation performed:** JavaScript syntax check and a Chromium test with mocked video/subtitle responses verified navigation, 62 episode buttons, SRT parsing, caption overlay, caption controls, and filters. **Actual Pixeldrain playback on laptops, Chromecast, Fire TV, or iPhone has not been verified through this test.**

## Desktop VLC support (v5)

Open the universal hub and click **VLC Desktop + SRT** on an episode. Your desktop browser downloads a small `.m3u` playlist with the original streaming video URL and an `#EXTVLCOPT:sub-file=...` reference to its external captions. Open that playlist with **VLC Media Player on Mac, Windows, or Linux**. It does **not** download the video.

**Caption caveat:** VLC desktop's support for SRT files hosted at remote HTTPS URLs is inconsistent. If video starts without captions, use that episode's **Matching SRT** link to save its subtitle file, then choose **VLC → Subtitle → Add Subtitle File**. The missing SRT for Wano 53 and 55 and synchronization caveats for Muhn Pace 05–30 remain unchanged. This is a best-effort desktop playback workflow, not a guaranteed automatic-captions button. The existing in-browser, iPhone VLC, and Infuse buttons are retained.
