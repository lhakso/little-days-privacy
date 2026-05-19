---
layout: default
title: LittleDays Privacy Policy
---

# LittleDays Privacy Policy

**Effective date:** 2026-05-18

## Who we are

LittleDays is a family memory journal app for iOS. It is built and maintained by a single independent developer, Luke Hakso. If anything in this policy is unclear, or you want your data deleted, email me directly at **luke.c.hakso@gmail.com**.

This is the whole policy. No fine print elsewhere.

## What the app does

LittleDays helps parents capture short voice or text "memories" of moments with their kids — a funny thing they said, a milestone, a small everyday scene worth remembering. You can optionally attach one photo per memory and tag which child it's about. The app then generates monthly recap summaries and printable photobook PDFs from those memories.

That is the entire product surface. Everything described below exists to support that.

## What we collect

- **Apple Sign-In identity.** When you sign in, Apple gives us a stable user identifier and an email address. The email may be Apple's "Hide My Email" private relay address — that's fine, it works the same.
- **Memories you write.** Text content, an optional photo, optional tags for which child the memory is about, and optional milestone tags.
- **Child profiles.** A name, an optional birthday, and an optional accent color. You create these; they describe your own kids.
- **Audio recordings.** When you record a voice memory, the audio is uploaded to our backend for transcription, then discarded server-side. A local copy stays on your device only so the app can retry the upload if it fails; once upload succeeds, the audio's job is done.
- **Settings preferences.** Things like reminder frequency and how much editorializing you want the app to do when it rewrites memories.

We do **not** collect:

- Analytics or usage telemetry
- Advertising identifiers (no IDFA, no ad networks)
- Location data
- Contacts
- Anything from other apps on your device

## Where your data lives

- **On your device.** This is the primary copy.
- **Supabase.** We use Supabase for the cloud database and private file storage. This gives you cloud backup and enables future cross-device sync.
- **OpenAI API.** Audio recordings and memory text are sent to OpenAI for transcription and for the optional rewriting/editorialization feature. Per OpenAI's API terms, data sent through the API is not used to train their models and is deleted from their systems within 30 days.
- **Sentry.** Used only for crash reports, so I can fix bugs that take down the app. Personal identifiers are stripped before the report is transmitted.

That's the full list of places your data goes.

## Children's data

LittleDays is designed around a clear principle: **the parent is the user; the child is the subject of the memories.**

- We do not knowingly accept account signups from anyone under 13.
- We do not knowingly collect personal information directly from children.
- Memories about children are created, edited, and controlled by the parent who holds the account.

If you believe a child has somehow created an account, email me and I will delete it.

## Sharing

We do not sell your data. We do not share it for marketing. We do not share it with anyone outside the service providers listed above (Supabase, OpenAI, Sentry), each of which is bound by its own privacy terms and uses the data only to provide its piece of the service.

## Your controls

- **Edit or delete any memory** at any time, from inside the app.
- **Delete your entire account** from Settings → Delete Account. This permanently removes all of your memories, photos, child profiles, and your account itself from our servers. It is not a soft delete.
- **Apple's "Hide My Email"** is fully supported — sign in with the relay address and the app works normally.

## Retention

Your data persists for as long as you keep your account. When you delete your account, we wipe your Supabase database rows, your storage objects (photos), and your Supabase auth user. There is no backup we hold onto afterward for "recovery" purposes — once it's gone, it's gone.

## Security

Supabase row-level security policies enforce per-account isolation at the database layer: your account can only read and write its own rows. Storage objects (your photos) are stored in private buckets and are only retrievable via authenticated requests scoped to your account.

## Changes to this policy

If this policy changes, the version on this page will be updated and the effective date at the top will be bumped. If a change materially affects how your data is handled, the app will surface a notice so you actually see it rather than relying on you checking this page.

## Contact

For privacy questions, deletion requests, or anything else related to your data in LittleDays:

**luke.c.hakso@gmail.com**
