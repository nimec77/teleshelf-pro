# TeleShelf Privacy Policy

**Version 1 · Effective 18 October 2026.**

[Policy archive](https://github.com/nimec77/teleshelf-pro/tree/main/privacy).

This policy covers the single TeleShelf Pro app for Android TV and Google TV,
its account-access bot and support. The in-app user agreement is version 3,
dated 17 October 2026.

## Who is responsible

TeleShelf is developed and operated by an independent individual developer.
Contact the developer through [@TeleShelfSupportBot](https://t.me/TeleShelfSupportBot).
Questions, complaints and privacy requests are handled through this bot.

TeleShelf uses the Telegram API and is unofficial. It is not made, endorsed or
operated by Telegram. You sign in with your own Telegram account; there is no
separate TeleShelf login.

## What happens to your videos

Videos, thumbnails, posts and comments come directly from Telegram through your
own signed-in session. TeleShelf operates no server-side media store, proxy,
channel catalog or content index. Its automatic feed covers your joined channels,
including archived ones. Search can use Telegram's own public search.

This does not prevent you from deliberately sending a message or attachment to
support. Support messages are handled separately, as described below.

## What stays on your TV

- **Telegram session and local data:** your sign-in and TDLib's local database,
  including Telegram data loaded for browsing.
- **Media cache:** downloaded video parts, thumbnails and profile photos.
  Settings → Storage lets you choose a cache limit, initially 512 MB. A playing
  file and recently downloaded files can temporarily take storage above that
  limit; it is not a hard cap on all app storage.
- **Library:** the recent channel-video cache, watch progress, History, explicit
  Watch Later saves, hidden videos/channels and the last ten searches.
  Saved and unfinished videos retain local details needed to display them;
  the 500 newest unsaved finished-video snapshots are retained for History.
- **Account country:** a two-letter country code may be derived locally from
  your Telegram account's phone country to choose a search keyboard.
- **Access evidence:** signed trial, paid-license and revocation messages cached
  for the signed-in account. They include the Telegram user ID, access type and
  issue time; trial messages also include the fixed expiry.
- **Device settings:** language, playback/storage preferences, Hide watched,
  sync preference, your diagnostics answer and a random support ID.
- **Report-deletion record:** after current reporting consent, the latest available
  Analytics app-instance identifier and Firebase app context. It stays after Off,
  sign-out and media/history clears; Android backup excludes it. Uninstall or app-data
  removal loses it. Only the latest saved identifier is available.
- **TV home-screen cards:** up to ten unfinished videos can appear in the
  launcher's Continue watching row. Other apps on the TV can read the
  thumbnails provided for that row.

### Removing local data

*Remove from history* and *Clear history* reset the relevant playback history
and resume points. Explicit Watch Later saves remain saved. Removal writes a
state marker rather than deleting every record. Hide watched changes what Home
and channel pages show; it does not erase history.

*Clear cache* in Settings → Storage removes downloaded media and pictures.
It does not remove the Telegram login, library or bot-side access records.

A successful *Sign out* ends this TV's session, clears the local account library
and signed-access cache, and removes its home-screen cards. Device settings,
diagnostics answer and support ID remain. Use Clear cache first if you also want
to reclaim downloaded media. Uninstalling removes the app's local storage.
Neither action deletes Saved Messages, trial/purchase records or support chats.

## What goes to Telegram

Your session contacts Telegram to authenticate, load and search content, stream
videos, read access messages and, when enabled, synchronize watch state.
A two-step verification password is sent to Telegram for authentication and is
not saved by TeleShelf.

Reactions, joining/leaving channels and reporting content happen on your
explicit action. TeleShelf does not upload videos, post to channels or write
comments. A QR code for a post or support link is opened on your phone.

Telegram requires sponsored messages in clients that show channel content.
TeleShelf fetches them and reports a view when the entire ad text is on screen,
and a click when you open the sponsored card's link QR. TeleShelf has no ads of
its own and receives no revenue from these messages.

Telegram handles its services under [its privacy policy](https://telegram.org/privacy).

## Watch progress and Watch Later sync

Settings → Account → Sync watch progress is on by default. While enabled and
account access allows sync, the app reads tagged `#teleshelf_sync` text messages
from your own Saved Messages at startup and writes changes when you leave.

Records contain the video identifier, source channel/post numbers, playback
position/duration, watch status, edit time and, where applicable, save and
playback times. Video titles, captions, pictures and local snapshots are not
part of this sync record. The developer does not receive this backup.

Turning sync off stops both directions and leaves existing messages in place.
Sign-out and uninstall also leave them. To erase the remote backup, turn sync
off on your TVs and delete the `#teleshelf_sync` messages in Telegram.
Re-enabling sync can upload remaining local watch state again. Compaction
deletes only fully parsed, outgoing TeleShelf sync messages older than its new
snapshot, never unrelated Saved Messages.

## Trial, purchase and access records

The account's one-time trial starts only when you press **Start free trial** in
[@TeleShelfProBot](https://t.me/TeleShelfProBot?start=trial) on your phone.
Installing the app or opening the bot starts nothing. Previous users receive
the same trial. It lasts exactly 1,209,600 seconds (14 days); repeat starts,
another TV, reinstall and `/restore` retain the original deadline.

After expiry, browsing and playback require a one-time Telegram Stars purchase.
There is no subscription or continuing free mode. You may buy before starting
a trial. The standard purchase price is 500 Stars worldwide, displayed by the
bot before checkout.
Use the same Telegram account on the phone and TV. The TV reads signed access
messages and uses Telegram server time; it never sends to the Pro bot or pays.

The Pro bot runs on Cloudflare Workers and stores:

| Store | Information | Purpose and retention |
|---|---|---|
| D1 trial ledger | Telegram user ID, first trial start and fixed expiry | Restore the same trial across TVs/reinstalls. Kept while the service operates; the trial row is deleted on a verified account-erasure request. |
| KV user record | Telegram user ID, access type, payment identifier, Stars amount, purchase/issue time, bot language, license-message ID and delivery time, grant flag and refund time where applicable | Deliver/restore access, handle refunds and retry delivery. Kept while the service operates to restore permanent access and handle refunds. Verified erasure requests are handled manually after explaining the effect on restore. |
| KV charge record | Telegram payment identifier and payer's Telegram user ID | Recognize handled payment updates. Kept while the service operates and included in verified purchase-record erasure requests. |

These stores hold no media or channel-content catalog. Your bot conversation,
invoices and signed messages also exist in Telegram. Deleting a message or
clearing TV data does not erase the server-side ledger. Send `/restore` to the
Pro bot to resend paid access or the original trial deadline.

For a payment question use `/paysupport` in the Pro bot. Your message is
forwarded to the developer with a routing user ID; replies return through
Telegram. A successful refund withdraws paid access; any existing trial keeps
its original deadline. The bot's `/terms` describes purchase/refund terms.

Encrypted operator backups of trial/purchase records are retained for up to
30 days from creation. Verified erasures are reapplied before restored data
returns to service. Provider-managed recovery history is subject to Cloudflare's
documented recovery windows; erasure is also reapplied before using recovered data.

Cloudflare processes the Pro bot's requests and records. See
[Cloudflare's privacy policy](https://www.cloudflare.com/privacypolicy/).

## Optional crash reports and usage statistics

Reporting is off until you say Yes. Firebase is not initialized before consent
is in force. No thanks or BACK declines; Settings → Support can switch sharing
off or on. This choice concerns optional reports, not the Telegram processing
needed for sign-in, playback, trial or purchase.

Crash reports include technical traces, recent diagnostic breadcrumbs, device
and app versions and your random support ID. *Send diagnostics* works only
while sharing is enabled. It saves a technical snapshot for upload on the next
app start: build/authentication state, channel count, cache sizes/limit in MB,
language, keyboard, throttling and playback/sync preferences.

Usage events describe screens, playback health and progress, feature choices,
search-result ranges, sponsored impressions/clicks, card actions, sign-in/out,
cache clears and settings. Setup properties include app language, channel-count
and memory ranges, Telegram Premium status, install source and preferences.
App-defined events use fixed categories, counts and ranges; they do not carry
the content or account identifiers used by the Pro bot.

These reports go to Google Firebase Crashlytics and Google Analytics.
Their SDKs also use installation/app-instance identifiers; this is
pseudonymous reporting, not a promise of anonymity. Google may process
technical connection/device information. Advertising-ID collection and
ad-personalization signals are disabled in the app. See
[Firebase's privacy information](https://firebase.google.com/support/privacy)
and [Google's privacy policy](https://policies.google.com/privacy).

TeleShelf's optional report fields exclude chats, captions, channel names,
usernames, chat/message/video identifiers, search queries, phone numbers and
content-bearing file paths. Logs are filtered/scrubbed for these purposes.
This restriction does not describe messages you deliberately send to support
or the separately disclosed account/payment identifiers stored by the Pro bot.

Crashlytics retains crash data and associated identifiers for 90 days before
starting removal. Analytics user/event data has a 14-month retention setting;
new activity may renew user-identifier retention, and aggregate reports are
outside that setting. See [Google's retention explanation](https://support.google.com/analytics/answer/7667196?hl=en).
Switching reporting off stops new collection; it does not erase already sent
reports or guarantee that aggregate statistics disappear.

The support ID is a random eight-character TV code, not a Telegram user ID or
phone number. It accompanies crash reports while sharing is enabled and the
Support link when you press Start on your phone. It helps locate crash reports;
it is not an Analytics user ID and cannot locate all Analytics data.

After a Yes to agreement v3, TeleShelf retains the latest available Analytics
app-instance identifier and its Firebase app context on this TV for later deletion
requests. The local record is excluded from Android backup. Switching sharing off,
signing out or clearing media/history leaves it; uninstalling or removing app data
loses it. Only the latest saved identifier is available, so earlier or replaced
identifiers may be unrecoverable.

Settings → Support → Request report deletion reads already committed local data;
it does not enable reporting or retrieve an identifier from Google. Start Support
on your phone first. The request QR opens a Telegram draft containing the available
identifiers and requested report types. Opening that link discloses them to Telegram;
the developer receives them when you press Send. Closing the TV screen does not
remove the phone draft or a sent message. If Analytics information is unavailable,
the TV offers an explicit crash-only request rather than claiming both types are
covered. The developer verifies the scope of a shared TV and requests provider
deletion manually. A submitted request is not proof of completed deletion; reports
created after a provider's cutoff can remain while sharing is on.

A material change to collected report data, processors or retention increments
the in-app agreement version. A previous Yes then pauses sharing until renewed;
a previous No remains off without another prompt. We do not sell report data.

## Support and privacy requests

[@TeleShelfSupportBot](https://t.me/TeleShelfSupportBot) is for app support and
privacy requests. Payment support stays in the Pro bot. The TV's Support QR
includes build number and support ID; they reach the bot when you press Start
on your phone. Messages and attachments you choose to send, your Telegram user
ID and any visible profile information are handled through Telegram for the
conversation. The developer manually removes developer-held support copies
90 days after resolution, or earlier following a verified erasure request.
This covers the developer's accessible forwarded messages, routing context,
replies, attachments and downloaded copies. Telegram's deletion controls can
remove a message only from one participant's view. This is not a promise to
erase every bot-side copy, other participants' copies or Telegram's retained
history/backups. A privacy-request response will state the scope actually removed.

To request access to or deletion of information held by the developer, write
to the Support bot and identify the relevant Telegram account or support ID.
Do not send a login code, password or Telegram session file. Verification must
be limited to what is needed to identify the relevant records.
Deleting TeleShelf records does not delete your Telegram account or information
independently held by Telegram, Google or Cloudflare.

Trial- and purchase-record erasure is handled manually through Support.
Deleting a trial row does not invalidate a signed trial token before its original
expiry. Deleting purchase records prevents future bot restoration from those
records; it does not itself invalidate signed licenses already in Telegram or
cached on a TV. Operator backups follow the retention and erasure-replay rules
above.

## Children and policy changes

TeleShelf displays channel content without child-oriented filtering. You must
meet the minimum-age requirements applicable to you under
[Telegram's Terms of Service](https://telegram.org/tos). TeleShelf adds no
separate minimum-age restriction.

Later policy versions will be dated and retained in the policy archive.
Material changes to optional reporting also use the in-app consent mechanism
described above.
