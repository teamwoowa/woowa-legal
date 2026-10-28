# On That Note: Privacy Policy

> UNPUBLISHED RELEASE DRAFT. Proposed effective date: upon the production release of On That Note, not the date this file was written. Publication is blocked until INTERNAL_GATES.md is resolved and the final binary, deployed services and store disclosures are reconciled. The body below describes the intended shipping feature set, not verified present behavior.

## 1. Controller and contact
Geumbich Hwang, trading as Woowa, is the controller for the app processing described here. Establishment: Berlin, Germany, sole trader.

Postal address: Weserstr 35, 10247, Berlin, Germany

Privacy and support: team.woowa@gmail.com

## 2. Local play, age and choices
You can play without creating a login account or supplying an email address. The app stores settings, calibration, progress, local scores, initials/nickname, local gameplay diagnostics, pending service requests and access-right information on your device. Random guest/installation credentials support requested online services. They do not prove a unique person or the first download across reinstalls or devices. Pseudonymous identifiers and hashed credentials are not necessarily anonymous.

The intended audience is ages 13 and older. We use a local coarse age band, not a date of birth. Optional analytics, advertising and push notifications are blocked for under-16 or unknown-age users unless any required guardian consent has been verified; under-13 users are not eligible for these optional services. The age band is not sent to Analytics or FCM. Ordinary gameplay remains available without those optional services. A privacy notice acknowledgement is not consent to all processing. Analytics, advertising choices and push are separate.

## 3. Leaderboards
Online ranking is optional. Public Expert leaderboard entries show your chosen initials/name, score and position in the relevant game/chart. Avoid real names and contact details. The service processes chart/ruleset/control identifiers, score, submission identifiers and request connection information. Depending on the ranking route, score validation also processes session/ticket identifiers, calibrated input timing/type/hand data and calculated accuracy/combo. Input replay is used for validation, not retained as raw replay in the reviewed ranking database; validation digests/results may be retained. IP addresses are processed by network infrastructure and request-limiting controls.

For newly authenticated submissions, a private credential-derived ownership binding supports control, export and deletion of the record independently of optional analytics or push consent. It remains only while the corresponding ranking record exists and is removed on eviction or full ranking privacy revocation. Historical public submission IDs cannot establish ownership.

Publishing a score is a separate choice from local play. Verification on routes using run tickets may transmit information before a publication decision. The legacy credential-owned ranking service and the newer Expert Top10 service have different data and retention models, described below; a Top10 display alone does not mean every service stores only ten records.

## 4. Access rights, purchases and rewarded ads
The welcome offer is manually activated once per new installation/guest and lasts 600 seconds. It is not proof of a first-ever human user. A rewarded-ad time pass lasts 305 seconds and is granted only after the required verified reward and closure handling, not merely after closing an ad. There are five permanent purchase packs: four individual game packs and one current twelve-song bundle. These are access products, not a promise of every future release.

For purchases, Google Play handles payment details. Our app/backend processes product and purchase-option information, purchase tokens and their hashes, an obfuscated guest-account binding, purchase/acknowledgement/refund status, verification timestamps, entitlement records, restore challenges and recovery state as needed to verify, deliver and maintain rights. Purchase tokens go only through the purchase-verification/recovery path, never Analytics. Required encrypted token recovery storage is separate from analytics event references. The app does not receive your full payment-card details through this integration.

Last verified permanent rights are intended to be securely cached for offline use and revalidated online for refunds and restoration changes. Short-lived welcome/ad passes are not permanent offline rights. Losing installation credentials can affect automatic recovery; cross-installation restoration requires supported ownership verification and is not guaranteed by possession of a nickname or a pasted token.

A valid Google Play purchase is intended to be restorable on multiple installations without automatically taking rights away from earlier installations. Restoration requires the supported native purchase query and server verification, not a pasted token or nickname. Consent choices, advertising/analytics identifiers and ranking data are not copied between installations by purchase restoration.

Google AdMob and its consent service may process IP addresses, approximate location inferred from IP, device/advertising or app identifiers, ad interactions and diagnostics according to the SDK, privacy choices and settings. This SDK processing is distinct from our eight app analytics events. We do not treat ad consent as analytics consent or join leaderboard credentials into an advertising profile. Declining ads does not prevent ordinary gameplay.

## 5. Optional analytics
Analytics is off by default and starts only after a separate eligible opt-in. We use Google Analytics for Firebase to understand gameplay, result-screen visibility and access-right flows. The eight app-owned event names are level_start, level_end, otn_result_view, otn_welcome_granted, otn_welcome_activated, otn_ad_access_granted, otn_purchase_verified and otn_access_state.

Allowlisted fields include game/song/difficulty/content version, access source, completion/exit classification, limited performance and duration information, product/access state and timestamps, and random analytics-only event/attempt/grant/transaction references. These references must not reuse guest credentials, rank proofs, purchase tokens or FCM tokens. We do not send raw input replay, initials/names, support correspondence or date of birth through these events. The SDK may also process app-instance/session identifiers, device/app information and automatic events such as first_open and session_start; those are not additional app-owned events. A first SDK observation after late consent does not prove a first installation or first human download.

The approved analytics user/event retention setting is two months, without resetting it on new activity. That setting is not a promise that every aggregate report or provider backup disappears after two months. Turning analytics off stops future app collection and requests a local SDK reset; this does not by itself delete data already received by Google. Contact us about applicable deletion rights. Google Signals, Google ad personalization and Google Ads campaign use are not purposes adopted by this notice.

## 6. Optional rank notifications
Push is independently off by default. Eligible users may opt in to rank-change alerts for their own accepted Expert Top10 record and grant the device notification permission. We process an FCM registration token, private credential-derived ownership proof, watched board and score/baseline, language, IANA timezone, token generation, subscription timestamps and bounded sending history. A public submission UUID alone is not ownership proof. Tokens and ownership proofs are never analytics parameters or public leaderboard fields.

The approved limit is at most one sending attempt per owner per local calendar day, with quiet hours from 21:00 to 09:00. Unknown/invalid timezone means hold, not send. Delivery may be delayed or fail; a provider acceptance is not proof of device delivery. An alert opens the appropriate Expert preparation/ranking view, not autoplay, an ad or a purchase. Unsubscribing removes the backend token/subscription, watches, optional receipts and outbox through the authenticated deletion flow, and attempts SDK token deletion; those are separate operations. Essential ranking ownership metadata remains with the ranking record. A separate minimal owner-hash, last sending-reservation time and generation record remains for up to 30 days after its latest subscription/reservation update to prevent unsubscribe/re-enrolment from bypassing the daily limit. It contains no token, watched board or profile. Full ranking privacy revocation removes that history and owned ranking records as well. A send already in flight cannot always be recalled.

Authenticated subscription/resume activity renews the 90-day inactivity expiry for the subscription and its watches. Outbox/sending history expires 30 days after creation, not 30 days after proven device delivery. Expired data awaits bounded cleanup, not guaranteed instantaneous physical deletion. Invalid tokens stop sending. See the retention section for other records.

## 7. Purposes and legal bases
We process objectively necessary local/service data to provide the game and online features you request and to verify and deliver purchases (Article 6(1)(b) GDPR where applicable). Optional analytics, optional push and advertising/device access requiring consent use consent (Article 6(1)(a), with applicable device-access consent rules). Optional public score publication is based on your choice/consent. You can withdraw consent for future processing without making prior lawful processing unlawful.

Proportionate fraud prevention, request limiting and protection against replay/recreation of deleted records may rely on legitimate interests (Article 6(1)(f)), subject to necessity and balancing. A legally required record is processed under the applicable legal obligation (Article 6(1)(c)), not an invented blanket retention period. Support information is used to answer your request, under the requested service or a legitimate interest in handling enquiries as appropriate. We do not use gameplay analytics to make decisions producing legal or similarly significant effects about you.

## 8. Recipients and international processing
Woowa operates the requested services. Cloudflare Workers/D1 provides backend hosting/database and network/security processing. Google Analytics for Firebase, Firebase Cloud Messaging and Google AdMob/consent services provide the respective optional features; Google Play provides purchase/payment services and verification. Support email is handled through Gmail. Public leaderboard entries are visible to others.

AdMob is linked to Firebase/Google Analytics for revenue and engagement measurement. Exported data is subject to the receiving product terms. Linking accounts does not replace the separate eligible app-side consent requirements, and the two-month Analytics setting is not a universal retention limit for every receiving product.

These notices are hosted on GitHub Pages. GitHub processes website request/connection information under its applicable terms and privacy information; this website hosting is distinct from optional in-app Analytics.

Google Ireland Limited is a relevant Google contracting/service entity for EEA services, subject to the particular product terms; other Google entities may handle processing. Hosting/analytics/messaging service-provider roles and Google's own payment/advertising responsibilities depend on the service and applicable terms. We do not describe every provider operation as solely processing on our behalf.

Google and Cloudflare services can process data outside Germany and the EEA. We do not promise EU-only storage or processing. Where required, transfers must rely on applicable adequacy decisions or contractual safeguards, including Standard Contractual Clauses and supplementary safeguards as appropriate. Contact us for information about applicable safeguards and how to obtain a copy.

## 9. Retention, deletion and local storage
Local settings/progress/access caches remain until changed, removed by the app or cleared with device storage, subject to platform backup/restore behavior. Local collection diagnostics use capacity limits of 20 owned files/20 MiB in total and 4 MiB per session, removing older matching files when space is reserved for a new session, rather than an invented number of days. Older diagnostic paths outside that policy need separate handling.

The reviewed legacy ranking lifecycle excludes public entries after 365 days. Unlinked run evidence is eligible for cleanup 30 days after issue, and unfinished runs after expiry plus 24 hours; evidence referenced by a surviving entry is retained while needed by that entry. Bounded cleanup may leave a physical backlog. In the newer Expert Top10 implementation, only current qualifying rows remain in that table: rejected/evicted rows have no history there, but optional notification receipts/history are separate.

Deletion of credential-owned ranking data revokes the credential and removes linked records in bounded batches. A minimal credential hash, revocation time and cleanup state remain to prevent old requests recreating deleted records; the reviewed implementation has no automatic expiry for that revocation record. A display removal is not necessarily deletion from every service. Purchase rights/claims and purchase recovery records have separate purposes from rankings and analytics. The owner-approved purchase policy is to retain encrypted recovery tokens while the corresponding purchase remains valid and the token is needed for verification, refund monitoring or restoration. For permanent purchases this can mean years. Tokens are scheduled for cleanup when their active-rights/recovery purpose ends, subject to verified revocation, authorized erasure and any other active association that still needs the shared record. Acknowledgement alone is not purpose closure. Minimal rights/claim proof must also be limited to its documented continuing purpose.

On That Note support correspondence is scheduled for cleanup 90 days after the enquiry is resolved. This does not apply to other apps or unrelated mail. Any actual mandatory transaction-record obligations must be verified separately for the relevant records; no universal financial period is invented here.

Minimal credential-revocation hashes, times and cleanup state remain while old credentials or backup replay could recreate deleted data, potentially for years. Woowa reviews necessity every 90 days and must clean up records when that risk is demonstrably closed. This criterion is not a promise of immediate physical erasure from provider backups or operator copies. Actual deletion, backup safeguards and the review/cleanup procedure must be implemented and verified before release.

Private service requests use HTTPS. Source candidates use encrypted purchase-token recovery and Android encrypted credential/state storage, but no system is guaranteed completely secure. Clearing local app storage does not delete server records, Google Play's independent records or provider backups. Restoration procedures must preserve deletion decisions.

## 10. Your rights and help
Contact team.woowa@gmail.com to request access, correction, erasure, restriction, portability where applicable, objection to legitimate-interest processing, or help withdrawing consent. We may need proportionate proof of ownership; do not email credentials, purchase tokens, FCM tokens, passwords or authentication codes. No login registration is required to contact us. Losing an installation may limit the records we can safely link to you.

You may complain to a competent supervisory authority, including the authority where you live or work or where an alleged infringement occurred. For our Berlin establishment, the Berlin Commissioner for Data Protection and Freedom of Information is a relevant authority: https://www.datenschutz-berlin.de/ .

We will show the effective date in the published policy and explain material changes before affected processing begins where required.
