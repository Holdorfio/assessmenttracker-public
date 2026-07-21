# Publication Procedure -- Legal Documentation

Governed by ADR-008. Two parts: one-time setup (creating the Publication Repository) and the recurring per-publish procedure. Both assume the Publication Repository's existence has already been separately approved per ADR-006 Principle 9.

## Public-facing content

`README.md` in this folder is the exact content for the Publication Repository's own `README.md` -- copy it verbatim. It contains no reference to the AssessmentTracker Repository's internal structure, and must stay that way on every future edit.

## One-time setup

1. Create the Publication Repository (public, empty).
2. Add `README.md` (from this folder) as its `README.md`.
3. Follow "Per-publish procedure" below for `EULA.md` and `PRIVACY_POLICY.md` (and `THIRD_PARTY_SERVICES.md`, if included).
4. Choose a Publication Platform and point it at the Publication Repository, following that platform's own setup instructions (see ADR-008 for platform neutrality -- no platform is prescribed here).
5. Verify each document is reachable over HTTPS before submitting URLs to Intuit.

## Per-publish procedure

Used whenever `legal/EULA.md`, `legal/PRIVACY_POLICY.md`, or `legal/THIRD_PARTY_SERVICES.md` changes in the AssessmentTracker Repository.

1. Confirm the change already went through its own review in the AssessmentTracker Repository -- this procedure publishes an approved document, it does not review legal content.
2. Copy the changed file's substantive text into the Publication Repository, unchanged.
3. Apply only whatever minimal formatting the chosen Publication Platform requires (e.g. front matter, if the platform is a static-site generator), plus a one-line provenance note stating the source Effective Date, e.g.:
   > Published from the AssessmentTracker Repository, Effective Date July 20, 2026.
4. Diff the copy against `legal/`: confirm the only differences are the platform formatting and provenance note from step 3 -- no substantive wording changed in transit.
5. Confirm the Publication Repository's README and pages still contain no reference to the AssessmentTracker Repository's internal structure, ADR numbers, or client engagement details.
6. Commit (message referencing the source Effective Date) and push.
7. Verify the live URL.

No separate publish-history log is kept -- the Publication Repository's own commit history is that record.
