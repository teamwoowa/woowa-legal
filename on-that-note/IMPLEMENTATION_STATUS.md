# On That Note implementation status

Review update: 2026-10-23. **Not a production privacy policy or release approval.**

## Implemented and executed locally
- Installation-authenticated data access/export and explicit record deletion in an isolated Cloudflare Worker/D1 candidate. No login account is added.
- Bounded deletion, immediate public exclusion while deletion is pending, revocation-aware write guards, and bounded cursor-based cleanup.
- Revision2 server:51 baseline checks,27 targeted review-fix checks and TypeScript check passed.
- Diagnostic English Godot UI: two-step confirmation/cancel, manual continuation/retry and explicit new-file export selection. Latest39 targeted checks passed; earlier74 baseline and5 configure-fence checks remain earlier-revision evidence, not a combined final suite.
- Actual Godot controller to local HTTP/Miniflare/D1:125 score records and130 validation records exported over independent pages, followed by two bounded deletion calls.18 Godot conditions and12 Node postconditions passed, including other-installation isolation and revoked-identity rejection. The gameplay profile adapter in this roundtrip is a fixture, not the main game writer.
- Actual installed-build v95 APK catalog:4 families,12 tracks,36 same-engine bindings,40 JSON resources and296 packed code/data items compared. The current development source differs from this installed build; it is not overwritten or silently relabeled as the same release.

## Still required before publication/activation
- Safe main-game cache ownership/restart integration, real Settings wiring and Android/production HTTPS validation.
- Bounded public-query work under expired/revoked backlog and an independently held deletion ledger/restore gate.
- Controller identity/contact details, audience/consent-age handling and final SDK/provider/transfer review.
- Final retention choices and verification.365-day public ranking /30-day unlinked evidence /expiry+24h incomplete tickets are candidate defaults, not owner-approved effective policy.
- The candidate retains a minimal revoked credential hash/timestamp and cleanup flag indefinitely. This is an unresolved security-retention exception, not full erasure or irreversible anonymity. Do not copy these defaults into an effective policy without reviewing necessity and limits.
- Final policy, binary, UMP options and Play Data safety must match before owner review/publication.

No production Worker, public policy URL, UMP message, store submission or device installation is activated by this review. Existing JustBalance policy files and URLs are unchanged.
