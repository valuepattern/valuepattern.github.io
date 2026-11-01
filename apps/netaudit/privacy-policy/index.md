---
layout: default
title: NetAudit Privacy Policy
description: Privacy Policy for the NetAudit Android app published by Value Pattern.
permalink: /apps/netaudit/privacy-policy/
---

# Privacy Policy for NetAudit

**Effective date:** November 1, 2026  
**Publisher:** Value Pattern  
**App package:** `com.valuepattern.netaudit`

This Privacy Policy explains how the NetAudit Android app (the **“App”**) accesses, uses, stores, and shares information. If you have questions, contact us at [support@valuepattern.com](mailto:support@valuepattern.com).

## Summary

NetAudit inspects the Wi‑Fi networks around you and the devices on your local network. It does not require an account, and Value Pattern does not run a server for it: scan results, device lists, network names, addresses, passwords and settings stay on your device. A few tests you start yourself contact public internet services, as described below. The App also uses Google AdMob to show ads, Google’s User Messaging Platform (UMP) to manage privacy choices, and Google Firebase for usage analytics and crash reports. Those Google services collect certain device, usage and diagnostic data as described below.

## Information used by App features

### Wi‑Fi scans

The App reads the list of nearby Wi‑Fi networks reported by Android (network name, access point hardware address, signal strength, channel, security type and similar details) and the details of the network you are connected to. Android requires location permission for Wi‑Fi scans because network data can reveal where you are. The App uses this permission only to scan Wi‑Fi. It does not read your GPS position, does not request background location, and does not send scan results anywhere.

On Android 13 and later, the App also asks for the Nearby Wi‑Fi devices permission to list Wi‑Fi Direct devices. It only listens: it never connects to or invites them.

### Local network scans

When you scan your network, the App sends standard discovery and probe traffic to devices on your local network, such as ping, Bonjour (mDNS), UPnP/SSDP, NetBIOS, reverse DNS, and connection checks on common ports. It reads names, manufacturers, open ports and service descriptions that devices announce, and asks your router for its UPnP port-forwarding list (read-only; the App never adds or removes forwards). This traffic stays on your local network.

The App remembers devices it has seen on each network so it can tell you what is new. This device inventory, coverage measurements, and your settings are stored in the App’s private storage on your device.

### New device alerts

If you turn on new device alerts, the App scans the network you chose in the background at the interval you pick and shows a notification when an unknown device appears. You can turn this off in Settings at any time. Background scans stay on your local network and never read your location.

### Device controls

For some devices (for example robot vacuums, smart TVs, printers, streaming players), the App can show status or send commands you choose, such as starting a clean, changing the volume, or sending a Wake‑on‑LAN packet. These commands go directly from your phone to the device over your local network. Passwords or pairing keys the device gives the App are encrypted with a key held in the Android Keystore and stored only on your device.

### Sharing Wi‑Fi by QR code

The App can draw a QR code that lets another phone join your network. Android does not let apps read saved Wi‑Fi passwords, so you type the password. If you choose to remember it, it is encrypted with a key held in the Android Keystore and stored only on your device. The QR code is drawn on your screen and is not uploaded.

### Tests that contact the internet

Some tests need to reach the public internet. They run only when you start them:

- **Public IP lookup.** When you tap to look up your public IP address, the App sends a request to [ipwho.is](https://ipwho.is/), falling back to [ipify](https://www.ipify.org/), which return your public IP address, internet provider and approximate location (city, region, country). The App shows the result and does not save it. These services receive your IP address as part of the request.
- **Connection diagnostics.** When you run diagnostics, the App pings your router, your DNS server and `1.1.1.1` (Cloudflare), and looks up a made-up name under `example.com` through your DNS server to time it.
- **Public Wi‑Fi check.** When you run this check, the App makes two DNS lookups and one HTTPS request to `one.one.one.one` (Cloudflare) to detect DNS tampering and HTTPS interception.

These requests do not include your network names, device lists or other scan results. The services involved process requests under their own privacy policies.

Android backup is turned off for the App, so its stored data is not copied to your Google backup.

## Usage analytics and crash reports (Google Firebase)

The App uses Google Analytics for Firebase to understand which features are used, and Firebase Crashlytics to receive crash reports so we can fix bugs.

Analytics records:

- **App interactions we define:** screens viewed; finishing a network scan, with the number of devices as a range (0, 1–5, 6–15, 16–30, 31+); the security grade of an audit; turning on new device alerts and the chosen interval; the verdict of a public Wi‑Fi check; the rating of a coverage measurement; and the type of device action used (for example “Wake‑on‑LAN”).
- **Information Firebase collects automatically,** according to Google: first opens, app opens, sessions and engagement time, the app version, the device model, the operating system version, language, and a general location (country or region) derived from the IP address. These are linked to a random app instance identifier created by Firebase, not to your name or any account.

Analytics and crash reports **never** include network names (SSIDs), access point or device hardware addresses, IP addresses of your devices, device names or host names, or passwords. The App turns off Firebase Analytics’ collection of the Android Advertising ID.

When the App crashes, Crashlytics sends a crash report containing the technical details of the error, the app version, the device model, the operating system version, and a random installation identifier.

Google processes this data under its own terms and policies, including the [Google Privacy Policy](https://policies.google.com/privacy) and Firebase’s [privacy information](https://firebase.google.com/support/privacy), and decides how long it keeps it within the retention settings Firebase offers.

## Advertising and consent services

The App uses the Google Mobile Ads SDK (AdMob) to show a banner ad on its main screens. According to Google, the SDK may automatically collect and share:

- IP address, which may be used to estimate general location;
- user product interactions, including app launches, taps, and video views where applicable;
- diagnostic information related to App and SDK performance, including app launch time, hang rate, and energy usage; and
- device and account identifiers, such as the Android Advertising ID, App Set ID, and other applicable identifiers.

Google states that this information is used for advertising, analytics, and fraud-prevention purposes and is encrypted in transit using TLS. The ads shown may be personalized, non-personalized, or limited depending on your region, consent choices, device settings, and Google’s ad-serving rules. Wi‑Fi scan results, device lists and other network information from the App are not shared with AdMob.

Where supported, the Google Mobile Ads SDK may also use Android advertising services for ad identification, attribution reporting, and Topics. The Topics API provides coarse-grained interest categories inferred on the device from recent app usage; attribution reporting helps measure when an ad leads to an action. These advertising-service permissions are included by the Google Mobile Ads SDK. You can manage supported advertising privacy features in Android system settings. See [Google’s Privacy Sandbox disclosure for AdMob](https://developers.google.com/admob/android/privacy/sandbox) for more information.

The App also uses Google UMP. On launch, UMP contacts Google to determine whether a privacy message or consent form is required and, where applicable, records your choices. Google and participating ad partners process advertising information under their own terms and policies. For more information, see:

- [Google Mobile Ads SDK data disclosure](https://developers.google.com/admob/android/privacy/play-data-disclosure)
- [How Google uses information from sites or apps that use its services](https://policies.google.com/technologies/partner-sites)
- [Google AdMob privacy](https://support.google.com/admob/answer/6128543)

## Privacy choices

Where required, Google UMP asks for your advertising privacy choices before the App requests ads. Where the consent form applies to you, you can change your choices later in the App under Settings › Privacy options.

You can also:

- reset or delete your Android Advertising ID and control ad privacy settings in Android system settings;
- manage personalized advertising through [Google’s My Ad Center](https://myadcenter.google.com/);
- turn off new device alerts in the App’s Settings;
- revoke the location, nearby devices or notification permissions in Android settings (Wi‑Fi scanning, Wi‑Fi Direct, or alerts will then stop working);
- clear the App’s storage in Android settings to remove its device inventory, saved passwords and pairing keys, measurements, settings, and locally stored consent state; or
- uninstall the App to remove all of its on-device data.

Value Pattern does not sell personal information for money. Google’s use of information for personalized or cross-context behavioral advertising may be considered “sharing,” “targeted advertising,” or a “sale” under some privacy laws. Use the choices presented by UMP, your Android advertising controls, or Google’s advertising controls to limit that processing where available.

## Permissions

The App may request or use these Android permissions:

- **Location (precise and approximate):** required by Android to scan for Wi‑Fi networks and read the connected network’s name. Not used to find your position, and never in the background.
- **Nearby Wi‑Fi devices (Android 13+):** lists Wi‑Fi Direct devices. Declared as not used for location.
- **Wi‑Fi and network state, change Wi‑Fi state, multicast:** read connection details, start Wi‑Fi scans, and receive local discovery replies (Bonjour, UPnP).
- **Internet:** local network scans and device controls, the internet tests above, ads, consent, analytics and crash reports.
- **Notifications:** new device alerts, only if you turn them on.
- **Advertising ID and advertising services:** added by the Google Mobile Ads SDK for ads, as described above.

The App does not request background location, contacts, camera, microphone, or storage permissions.

## Retention and deletion

Value Pattern does not operate an account or backend for the App and therefore holds no scan results, device lists, passwords or settings to retain or delete. Clear the App’s storage or uninstall it to remove this information from your device.

Google determines how long it retains information collected through AdMob, UMP and Firebase. Requests concerning that information should be made using the controls and request methods described in [Google’s privacy policy](https://policies.google.com/privacy).

## International data transfers

Value Pattern does not receive the App’s network data. Google, Cloudflare and the IP lookup services may process the information described above in countries other than the one where you live, subject to the safeguards described in their policies.

## Children’s privacy

The App is not directed to children under 13, and Value Pattern does not knowingly collect personal information from children through the App. The App’s advertising configuration does not identify users as children or as under the applicable age of consent. If you believe a child has provided personal information through a third-party service, contact us and the applicable service provider.

## Your privacy rights

Depending on where you live, you may have rights regarding personal information, including rights to access, correct, delete, restrict, or object to processing, and to withdraw consent. Because Value Pattern does not receive the App’s network data or maintain App accounts, most requests relating to advertising or analytics data must be directed to Google or exercised through Google’s and Android’s privacy controls. You may contact us if you need help identifying the appropriate route for a request.

## Changes to this policy

We may update this policy if the App, its third-party services, or legal requirements change. We will post the revised policy at this URL and update the effective date above. Material changes may also be communicated in the App or its store listing when appropriate.

## Contact

For privacy questions or concerns, email [support@valuepattern.com](mailto:support@valuepattern.com).
