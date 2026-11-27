---
layout: default
title: SpeakPro Privacy Policy
description: Privacy Policy for the SpeakPro Android app published by Value Pattern Labs.
permalink: /apps/android-app-speakpro/privacy-policy/
---

# Privacy Policy for SpeakPro

**Effective date:** November 26, 2026  
**Publisher:** Value Pattern Labs  
**App package:** `com.valuepattern.speakpro`  
**Contact:** [support@valuepattern.com](mailto:support@valuepattern.com)

SpeakPro helps you practice public speaking and negotiation. You record yourself, and the app gives you feedback
on how you spoke and what you said. Some of that feedback comes from AI, which means your speech leaves your phone.
This policy explains exactly what is sent, who handles it, how long it is kept and how to delete it.

## The short version

- To review a speech, SpeakPro sends its recording to our server, which has it transcribed and assessed by OpenAI.
- Our server never stores the recording. It keeps the transcript and the feedback for 90 days, then deletes them.
- Your recordings and practice history stay on your phone, and are not included in Android backups.
- Unless you turn it off in Settings, the app sends Google Firebase usage statistics and crash reports. They never
  include your speeches, transcripts or recordings.
- If you subscribe to Pro, Google Play handles the payment. We never see your card or payment details; we receive
  the subscription's status from Google so we can turn Pro on and off.
- There are no ads, and we don't sell or share your data for advertising.
- You can delete what our server holds, or your whole account, from the app at any time.

## Your account

You need an account to use SpeakPro. You can create one in either of two ways:

- **With Google.** We receive your Google account's ID, email address, name, and whether Google has verified the
  email address. We never see your Google password.
- **With a username and password.** We store the username and a one-way hash of the password (argon2id). We can't
  read your password.

Each phone you sign in on gets its own sign-in session. We store a hash of the session token, the phone's model
name (for example "Pixel 9"), whether the session was opened on a physical device, an emulator or one of Google's
test devices, and when the session was last used. On your phone, the session token is encrypted with
a key kept in Android's secure key store.

We also keep how many seconds of your recordings have been analyzed, so we can apply the free limit. This count
stays with the account even if you delete your speeches. Whether you have Pro is worked out from your Google Play
subscription (see below), or from Pro given to your account by Value Pattern staff, which we record with who gave it,
when, and until when.

For our costs and spending limits, we keep a daily usage total for each account: how many AI requests of each kind
were made, how many seconds of audio and how many tokens they used, and what they cost us. It holds no words from
your speeches. It stays when you delete your data; when you delete your account, it is no longer linked to you.

**Prevention of abuse.** To enforce the limits of the free tier and the daily usage limits, and to prevent misuse
of the service, we maintain a pseudonymous identifier derived from your Google account identifier or username, which
cannot be used to recover either. We may suspend any account that we reasonably believe has been used in breach of our
[Terms of Use](/apps/android-app-speakpro/terms/), and we record the fact of the suspension, its date and the reason
for it. Upon deletion of your account, we retain the identifier, together with the amount of free analysis time
used and the suspension status of the account, if any, for a period of one year, and we retain its association with
the deleted account's daily usage totals for a period of two days. This information is used solely for the purposes
described in this paragraph.

**Device and app integrity.** When you create an account and each time a recording is submitted for analysis, the
app requests an integrity verdict from Google Play, and our servers submit that verdict to Google for verification.
The verdict indicates whether the request originates from an unmodified copy of SpeakPro installed through Google Play
on a device that passes Android's integrity checks. We record only whether the verification succeeded and, if it did
not, the category of the failure, in our service logs, which are retained for a few days. We may decline requests
that fail verification.

## What happens when you practice

**On your phone.** SpeakPro records your speech and measures your pace, pauses and timing on the phone itself. The
live word count during a speech uses Android's on-device speech recognition, so that audio is not sent anywhere.
Recordings, transcripts, scores and history are stored in the app's private storage. They are excluded from Android
cloud backup and from transfers to a new phone. You can have recordings deleted automatically after analysis in
Settings.

**Sent for review.** When a speech is analyzed, the app sends our server:

- the recording, as an audio file;
- the transcript, with the time each word was spoken;
- what the app measured, such as pace and pauses;
- the exercise, topic or title, the speech's language and its length.

For a negotiation it sends each spoken turn, the scenario you chose and its difficulty.

**What our server does with it.** It sends the audio to OpenAI to be transcribed, and the transcript and
measurements to OpenAI to write the feedback: ratings, what worked, what to fix and suggested rewrites. In a
negotiation, OpenAI also plays the other side. The recording is held in memory only for as long as transcription
takes, and is never written to our database or disks.

**What our server keeps.** For each speech or negotiation it keeps:

- the transcript, with word timings;
- the topic, exercise and language;
- the feedback;
- a record of each AI request: what was sent to the model and what it answered, how long it took and what it
  cost.

We use these to run the service, to fix problems and to improve the feedback. Value Pattern staff can read them in
a private admin panel, which only allowlisted staff accounts can open, and every time staff open an account or a
speech it is logged.

## Pro subscription and payments

Pro is a subscription sold through Google Play. Google Play takes the payment and handles billing, renewals, refunds
and cancellation under the [Google Play terms](https://play.google.com/about/play-terms/) and
[Google's privacy policy](https://policies.google.com/privacy). We never receive your card number, billing address or
other payment details.

- **What the app sends Google Play:** when you buy, a random code that stands for your SpeakPro account (not your name
  or email), so the purchase can be matched to your account.
- **What the app sends our server:** the purchase token Google Play gives the app, after you buy, each time the app
  starts, and when you tap Restore purchase.
- **What we receive from Google Play:** for each subscription, its plan (yearly or monthly), any offer such as a free
  trial, its status (for example active, canceled, in a grace period or expired), when it started and when it
  renews or ends, whether it renews automatically, the price and currency, the order number, and whether it is a
  test purchase. Google also notifies our server when a subscription changes, through Google Cloud Pub/Sub.
- **What we keep:** that information with your account, for as long as you have the account, so we know whether you
  have Pro. It is deleted with your account.

Deleting your SpeakPro account doesn't cancel the subscription. Cancel it first in Google Play under **Payments &
subscriptions › Subscriptions**, or with **Manage subscription** in SpeakPro's Settings.

## Usage statistics and crash reports

To see how SpeakPro is used and to fix crashes, the app uses Google Analytics for Firebase and Firebase
Crashlytics. You can turn both off under **Settings › Privacy and analysis › Share usage statistics and crash reports**; turning
it off also deletes crash reports not yet sent.

- **Usage statistics:** that you signed up or signed in (and whether with Google or a password), that a speech was
  started, finished and reviewed, its exercise and its length in broad ranges (such as "1 to 3 minutes"), that the
  free minutes or the day's AI review ran out, that the Pro screen was shown and from where in the app, and that Pro
  was bought, with the plan and whether it began with a free trial. Firebase also records Google Play purchases on
  its own: the product, price and currency. Firebase adds an identifier for this installation of the app, the phone's model, Android
  version, language and country, the app's version, and which Google Play listing led to the install.
- **Crash reports:** what the app was doing when it crashed, the phone's model and state (such as free memory), and
  an identifier for this installation.

They never include your speeches, transcripts, recordings, titles, topics, name or email. SpeakPro doesn't collect
the advertising ID and sends no advertising signals. Google keeps usage statistics linked to the installation for
2 months and crash reports for 90 days.

## Who else handles your data

We use these service providers to run SpeakPro, and only for that purpose:

- **OpenAI.** It transcribes speeches and writes the feedback. Under OpenAI's API terms, the data we send is not
  used to train OpenAI's models. OpenAI may keep it for up to 30 days to detect abuse, then deletes it. We ask
  OpenAI not to store our requests beyond that. With each request we send a code derived from your account, which
  is not your name or email, so OpenAI can tell accounts apart if it finds abuse.
- **Cloudflare.** It runs our server. Like any web host, it handles your phone's IP address and request details
  to deliver requests and protect against attacks. Its request logs are kept for a few days.
- **Render.** It hosts our database, which holds your account, transcripts and feedback, in Ohio, United States.
- **Google.** It provides Sign in with Google, if you choose it; Google Play, which sells and bills the Pro
  subscription and tells our server its status; Google Play Integrity, which verifies that requests come from SpeakPro
  as installed through Google Play; and Firebase's usage statistics and crash reports, unless you turn
  them off.

We don't sell your data, share it for advertising, or give it to anyone else, unless the law requires it.

## Security

Every connection between the app and our server is encrypted (HTTPS). Transcripts, topics and feedback are
encrypted before they are stored, with a key that only our admin panel holds, so the part of our server that
receives your speeches can't read them back. Passwords and session tokens are stored only
as hashes. The database accepts only encrypted connections, and the server's own access is limited to reading and
writing rows. The admin panel sits behind a separate sign-in that only Value Pattern staff can pass. To stop abuse,
our server counts requests by IP address and username, and deletes those counts within a day.

## How long we keep data

- **Transcripts, feedback and AI request records:** 90 days from the speech, then deleted automatically.
- **Recordings:** never stored on our server. On your phone until you delete them.
- **Your account:** until you delete it. A sign-in session ends after 180 days without use.
- **Rate-limit counts:** up to one day.
- **Daily usage totals:** linked to your account until you delete it, then kept without it.
- **Pro subscription records:** while you have your account; deleted with it. Google Play keeps its own records of
  your purchases under Google's policies.
- **After deleting your account:** the pseudonymous identifier, with the free analysis time used and any
  suspension status, for one year.
- **Firebase usage statistics:** 2 months at Google. **Crash reports:** 90 days at Google.

## Your choices and rights

In the app, under **Settings › Your data**:

- **Delete my data on the server** deletes every transcript, all feedback and every AI request record for your
  account right away. Your account stays.
- **Delete account** deletes your account and everything our server holds for it right away, and signs you out on
  every phone. It doesn't cancel a Pro subscription; cancel that in Google Play first.
- **Delete everything on this phone** removes your sessions, recordings and settings from the phone.

You can also delete your account without the app; see
[Delete your SpeakPro account](/apps/android-app-speakpro/delete-account/).

Depending on where you live, you may have the right to access, correct, delete or export your data, or to object
to how it is used. Email [support@valuepattern.com](mailto:support@valuepattern.com) and we will answer within 30
days. If you are in the EU or the UK, you can also complain to your data protection authority.

We process your data to provide the service you asked for: transcribing and assessing your speeches. Our service
providers may process it outside your country, including in the United States, under their standard data
protection terms.

## What SpeakPro doesn't do

- No ads, and no advertising ID.
- No tracking across other apps or websites.
- No location, contacts, camera or files outside the app.

## Permissions the app uses

- **Microphone:** to record your speeches. It is used only while you practice.
- **Google Play billing:** to buy Pro and restore a purchase.
- **Internet and network state:** to send speeches for review, and to wait for a connection when you are offline.
- **Keep the phone awake, and start after a restart:** so a review started just before you left the app, or
  before the phone restarted, can still finish.
- **Vibration:** for the timing cues during a speech.
- **Install referrer:** added by Firebase, to tell which Google Play listing or campaign led to the install.
- **Biometrics:** listed by Google's sign-in library, which Android uses for saved passwords and passkeys. SpeakPro
  itself never reads fingerprint or face data.

## Children

SpeakPro is not meant for children under 13, and we don't knowingly collect their data. If you believe a child has
created an account, email us and we will delete it.

## Changes

If we change how SpeakPro handles your data, we will update this page and its effective date before the change
takes effect.

## Contact

Value Pattern Labs, [support@valuepattern.com](mailto:support@valuepattern.com)
