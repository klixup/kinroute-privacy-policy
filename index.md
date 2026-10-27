---
title: Kinroute privacy policy
---

# Kinroute privacy policy

Last updated: 27 October 2026

Kinroute (`app.kinship.locator`) is a location-sharing app for people who have agreed to share with each other. This policy says what the app collects, why, and how long it is kept.


## Who the app is for

Kinroute is not for children under 13. In some countries the minimum age is higher, and the app blocks sign-up below that age. Kinroute stores a birth year and a country code, not a full date of birth.

Everyone who shares does so for themselves. An invite shows who is in the circle before anyone agrees. Sharing stays off until that person turns it on. They can pause or leave later, and the circle is told when sharing stops.

## Information the app uses

- **Account.** A Supabase account ID, display name, optional username, birth year, and country code, so we can provide your profile and apply the age rule. If you choose Google or an email sign-in link, Supabase Auth also processes your email address and Google may provide your name. Email is not shown to family members. Your display name and username are visible only to members of circles you join.
- **Location and movement, while you are sharing.** Latitude, longitude, accuracy, speed, and the time of the fix. With your activity-recognition permission, Kinroute also detects whether the phone is still, walking/on foot, bicycling, or in a vehicle. It uses this movement state to adjust background GPS update frequency and reduce unnecessary battery use. The current state is stored with location history and shared with members of the circle you chose while sharing is on. It is not used to select ads. You can pause sharing at any time.
- **Phone status used for sharing.** Battery level, charging state, whether background location is allowed, app version, OS version, and device model. These help the circle understand a stale location and help the app stay within its battery target.
- **Places and alerts.** Place names and areas you save, arrive and leave events, check-ins, low-battery and stopped-sharing notices, and SOS messages you choose to send.
- **Push token.** A Firebase Cloud Messaging token so alerts and a "refresh now" request can reach the phone. The token is removed when Firebase says it is no longer valid.
- **Purchases.** If you buy Kinroute Plus, Google Play gives us a purchase token, product id, and expiry. The phone does not grant Plus by itself. Google confirms the subscription first.
- **Advertising, free plan only.** Free accounts can see Google AdMob ads on the circle list, places, and device health screens. Ads are not shown on the sign-in, age, consent, or permission screens, on the live map, or on the SOS control. Kinroute does not use your location to choose ads and does not sell location data. Plus and Care accounts do not see ads.
- **Crash reports, only if Firebase is configured.** If the owner has added `google-services.json`, the app can send crash stack traces to Firebase Crashlytics. A build without that file does not send crash reports.
- **Who opened the map.** When you open a circle map, Kinroute can record that you viewed the members who are sharing, so they can see who looked. This is limited to people in the same circle.

## What Kinroute does not do

Kinroute does not sell location. Kinroute does not collect location before the disclosure and your choice to share. Kinroute does not show another member's location while their sharing is paused.

## Who processes the data

- **Supabase** stores account, circle, location, alert, and purchase records. If you choose Google sign-in, Supabase Auth verifies the Google ID token and stores your Google identity and email for sign-in and account recovery.
- **OpenStreetMap Foundation** serves map image tiles, rendered on the phone by MapLibre. The tile service receives your IP address and requested map tile areas. Member names, account tokens and exact location records are not sent to the tile service. See the [OSMF privacy policy](https://osmfoundation.org/wiki/Privacy_Policy).
- **Firebase Cloud Messaging** delivers alerts.
- **Google Play** processes Plus purchases.
- **Google AdMob** serves ads to free accounts, after the Google consent message where that message is required.
- **Firebase Crashlytics** receives crash reports only when the owner has configured Firebase.

## How long data is kept

The history screen shows 1 day on the free plan, 30 days on Plus, and 90 days on Care. The server rejects requests for anything older.

Raw location and movement records are kept at least 7 days so a delayed upload can still arrive, and longer when a circle's plan allows a longer history (30 or 90 days). A daily job deletes points after that, and deletes alerts older than 90 days. Until that job is enabled in the Supabase project, deletion is available but not yet on a clock. The owner turns the schedule on by enabling `pg_cron`.

You can export your data or delete your account in the app's Account screen. Deleting the account removes the profile, the circles you own, and your locations. Purchase rows can remain with personal fields cleared for accounting. Backups age out on the host's normal backup cycle.

## Your choices

- Pause or stop sharing, or leave a circle, inside the app.
- Turn off background location in Android settings. Sharing then becomes stale, and the app says why.
- Set quiet hours. Ordinary alerts wait. An SOS still comes through.
- Buy Plus to remove ads for the account.
- Ask a privacy question at the contact address below. Export and deletion are available in the app's Account screen.

## Contact

Privacy questions: klixupwork@gmail.com
