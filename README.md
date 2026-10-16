![TeleShelf Pro — your Telegram videos on TV, with the blue shelf icon beside an illustrated television](assets/social-preview.jpg)

# TeleShelf Pro

**Your Telegram videos, at home on TV.**

Browse the channels you follow as video shelves. Resume where you stopped,
save something for later, and control everything with your TV remote.

[English](README.md) · [Русский](guides/ru.md) · [Português (Brasil)](guides/pt-BR.md) · [Español (Latinoamérica)](guides/es-419.md)

**The first public APK is being prepared. There is nothing to download yet.**

**[How to install on your TV](#install-and-sign-in)** · [Check APK availability](https://github.com/nimec77/teleshelf-pro/releases)

The cover is an illustration; the app screenshots below use synthetic data.

[Release availability](https://github.com/nimec77/teleshelf-pro/releases) ·
[Trial, buy or restore](https://t.me/TeleShelfProBot?start=trial) ·
[App support](https://t.me/TeleShelfSupportBot)

Install TeleShelf before starting the trial: the timer starts when you press
**Start free trial** in the Pro bot on your phone.

TeleShelf uses the Telegram API and is an independent, unofficial app. It is
not made or endorsed by Telegram. This repository distributes official APKs;
it does not contain the app's source code.

## A TV view of your channels

- **Home:** popular videos, latest posts and shelves for the channels you follow.
- **Keep your place:** playback resume, History and progress sync through your own Saved Messages.
- **Make a list:** Watch Later and a reversible Hide watched setting for Home and channel pages.
- **Find a video:** search your subscriptions or use Telegram's free public search quota.
- **Watch comfortably:** quality and speed controls, embedded audio tracks and subtitles when the file provides them.

The following are actual app UI captures rendered with synthetic test data.
Thumbnails and video pictures are absent in these previews. Select an image
to view it at full size.

| Home | Player |
| --- | --- |
| [![Home showing video shelves and a Resume action with synthetic titles](assets/screenshots/home.png)](assets/screenshots/home.png) | [![Player controls showing progress, play, seek and playback speed](assets/screenshots/player.png)](assets/screenshots/player.png) |
| **Search** | **Start trial** |
| [![Search with All Telegram, Subscriptions and Channels tabs and synthetic results](assets/screenshots/search.png)](assets/screenshots/search.png) | [![Trial screen with the Pro bot QR, trial instructions and Check access button](assets/screenshots/trial.png)](assets/screenshots/trial.png) |

## What you need

An Android TV or Google TV device running **Android 8.0 or later**, with a
32-bit or 64-bit ARM processor, a remote, an internet connection and Telegram
on your phone. Android-based Fire TV devices may run the sideload APK;
device compatibility still needs launch verification. Vega OS, Apple TV
and x86 devices are unsupported by this APK.

The interface is available in English, Russian, Brazilian Portuguese and
Latin American Spanish. TeleShelf plays videos from your own Telegram
account; it does not supply subscriptions or a content catalog.

## Install and sign in

The first public APK has not been released. The steps below explain how to
install the official file once it appears in [GitHub Releases](https://github.com/nimec77/teleshelf-pro/releases).
If a release has no `.apk` under **Assets**, there is no installable file yet.
Install the app before starting the trial.

### Download directly on the TV

1. Install **Downloader by AFTVnews** from your TV's supported app store.
   See the [official Downloader page](https://www.aftvnews.com/downloader/) to
   identify the app. Open Downloader on the TV.
2. Enter this address in Downloader's browser:

   ```text
   https://github.com/nimec77/teleshelf-pro/releases
   ```

3. Open the newest official release, expand **Assets** and select the file
   ending in **`.apk`** (`teleshelf-pro.apk`). **Source code (zip)** and
   **Source code (tar.gz)** are not Android installers.
4. When Android asks, allow **Downloader** to install apps. The setting may be
   called **Install unknown apps** or **Unknown sources**; names and locations
   vary by TV. Return to Downloader and open the downloaded APK again if needed.
5. Choose **Install**, then **Open**. For an update, install over the existing
   TeleShelf app to keep your Telegram login, history and settings. Keep its data.

If a verified numeric Downloader code becomes available, it will be shown
here and in [@teleshelf_pro](https://t.me/teleshelf_pro). Use the full Releases
address above until then. These are general APK-installation steps; a
device-by-device TeleShelf compatibility list has not been published.

### Transfer from an Android phone

Use this alternative only if [LocalSend](https://localsend.org/download) is
available and usable with the remote on your TV:

1. On the phone, open the official Releases page and download the `.apk`
   from **Assets**. After a Telegram mirror is published, you can also save
   the APK document from [@teleshelf_pro](https://t.me/teleshelf_pro).
2. Open LocalSend on the Android phone and TV, connected to the same local
   Wi-Fi/network. On the phone, select the APK and send it to the TV; accept
   the transfer on the TV.
3. Open the received APK using LocalSend or the TV's file manager. If prompted,
   allow that app to install APKs, then choose **Install** and **Open**.

LocalSend availability, remote control and opening APKs depend on the TV;
this alternative has not yet been verified on physical TeleShelf hardware.
iPhone users should use the direct TV method above.

### Sign in, then start the trial

1. Open TeleShelf on the TV. Use Telegram's device-link QR scanner on your
   phone to scan the TV's login code and confirm the connection. Enter your
   Telegram two-step verification password on the TV if requested.
2. On the phone, open [@TeleShelfProBot](https://t.me/TeleShelfProBot?start=trial)
   with **the same Telegram account**. Press **Start free trial** when you
   are ready to begin the account's 14 days. Installing or opening the bot
   starts nothing.
3. Return to TeleShelf. Choose **Check access** if the access screen remains.
   Existing trial/purchase: send `/restore` to the Pro bot; it preserves the
   original trial deadline.

### Updating and common problems

- **Update:** download the new official APK and install it over TeleShelf.
  There is no automatic updater. Uninstalling removes local app data.
- **Downloaded a ZIP?** Return to **Releases → Assets** and select the APK.
- **Installation is blocked?** Allow the app opening the APK to install apps
  in your TV settings. Check your model supports Android APK installation.
- **App not installed / incompatible?** Check Android 8.0+, an ARM processor
  and the official signing certificate below. Contact support with the TV
  model, Android version and exact error.
- **Access does not appear?** Use the same Telegram account on phone and TV,
  send `/restore` to the Pro bot and choose **Check access** on the TV.

App/install help: [@TeleShelfSupportBot](https://t.me/TeleShelfSupportBot).

## Fourteen days, then a one-time purchase

Every account gets **one 14-day trial**, including previous TeleShelf users.
It starts only when you press **Start free trial** in
[@TeleShelfProBot](https://t.me/TeleShelfProBot?start=trial) on your phone.
Installing the APK or opening the bot starts nothing. Another TV, a reinstall
or `/restore` keeps the original deadline.

After the trial ends, browsing and playback require a **one-time Telegram
Stars purchase**. There is no subscription or continuing free mode. The bot
shows your regional price, **250 or 500 Stars**, before you confirm checkout.
You can buy before starting a trial. A purchase belongs to your Telegram
account and unlocks the app until a signed revocation, such as after a refund.
Read `/terms` in the Pro bot before buying; use `/paysupport` there for payment help.

For a new TV or a missing access message, send `/restore` to the Pro bot on
your phone and choose **Check access** on the TV if needed. Restore does not
restart the trial. Support, the user agreement and sign-out remain available
while content access is locked. The TV never sends bot messages or spends Stars.

## Updates and authenticity

Official release files will appear in
[GitHub Releases](https://github.com/nimec77/teleshelf-pro/releases) and as APK
documents in [@teleshelf_pro](https://t.me/teleshelf_pro). News is in
[@teleshelf_tv](https://t.me/teleshelf_tv). Each release will identify its
version and the APK's SHA-256. Both mirrors must contain identical bytes.

Compare the downloaded file's SHA-256 with that release's published hash.
The APK hash changes for every build; the signing certificate identifies
official updates. Its SHA-256 is:

```text
4e5bc630c2a119d9ce22abe9f77a1191be749eac50af3ec4a306214a53fe768c
```

On a computer with Android SDK Build Tools, inspect the certificate with
`apksigner verify --print-certs teleshelf-pro.apk`. Check the
`Signer #1 certificate SHA-256 digest` against the fingerprint above. Use
`shasum -a 256 teleshelf-pro.apk` on macOS, `sha256sum teleshelf-pro.apk` on
Linux or `Get-FileHash .\teleshelf-pro.apk -Algorithm SHA256` in PowerShell
to inspect the file hash. A copy signed with a different certificate is
not an official update and can expose your Telegram session.

## Privacy and help

Videos are fetched directly by your own Telegram session. TeleShelf operates
no server-side media cache or content catalog. The Pro bot retains your
Telegram account id, the original trial dates and purchase records for access
and restore. Optional crash and usage reports are off until you consent.
The public privacy policy is being finalized before launch; the in-app user
agreement is available from Support and About.

- App problems and feedback: [@TeleShelfSupportBot](https://t.me/TeleShelfSupportBot).
- Trial, purchase, restore and `/paysupport`: [@TeleShelfProBot](https://t.me/TeleShelfProBot).
- Official files: [@teleshelf_pro](https://t.me/teleshelf_pro).
- News and discussion: [@teleshelf_tv](https://t.me/teleshelf_tv); use its linked Discussion button for “TeleShelf — comments”.
