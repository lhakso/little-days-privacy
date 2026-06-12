# LittleDays Privacy Policy

**Effective date:** 2026-06-12

## Who we are

LittleDays is a family memory journal app for iOS, operated by **Little Days LLC**, a small independent company. If anything in this policy is unclear, or you want your data deleted, email us directly at **littledaysllc@gmail.com**.

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
- **Photobook order details (only if you order a book).** When you buy a printed photobook, you provide a shipping name, address, phone number, and the email for delivery updates. We also generate a print-ready PDF of the memories and photos you chose to include. Payment card details are entered into Stripe's payment sheet and go directly to Stripe — we never see or store your card number.
- **Subscription status (only if you subscribe to Little Days Plus).** If you subscribe to our optional cloud-storage upgrade, the purchase is processed by Apple through your Apple ID — we never see your payment details. Apple sends us a signed receipt and renewal notifications so we know your subscription is active and can raise your storage limit accordingly. We store only your subscription's status and the identifiers needed to keep it in sync; we do not store any card or Apple ID payment information.

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
- **Stripe** *(only if you order a photobook).* Payments for printed books are processed by Stripe. Your card details are entered directly into Stripe and are handled by Stripe, not by us — we only receive a confirmation that a payment succeeded and a reference to it, never the card number. Stripe acts as the payment processor for the transaction; Little Days LLC is the merchant of record.
- **Lulu** *(only if you order a photobook).* Printed books are manufactured and shipped by Lulu, a print-on-demand provider. To fulfill your order we send Lulu the print-ready PDF of your book and your shipping details (name, address, phone, and an email for delivery updates). Lulu uses this only to print and deliver your book.
- **Apple** *(only if you subscribe to Little Days Plus).* The Little Days Plus storage subscription is sold and billed by Apple through your Apple ID. Apple handles the payment and sends us a signed receipt and renewal notices so we can keep your storage limit in sync. We never receive your card or Apple ID payment details.

That's the full list of places your data goes. Stripe and Lulu only ever receive anything if you order a printed photobook; Apple's subscription data only exists if you subscribe to Little Days Plus. If you do neither, your data never touches them.

## Children's data

LittleDays is designed around a clear principle: **the parent is the user; the child is the subject of the memories.**

- We do not knowingly accept account signups from anyone under 13.
- We do not knowingly collect personal information directly from children.
- Memories about children are created, edited, and controlled by the parent who holds the account.

If you believe a child has somehow created an account, email us and we will delete it.

## When you order a photobook

Ordering a printed book is the only part of LittleDays that involves money or physical shipping, so it's worth spelling out separately:

- The memories and photos you select are rendered into a print-ready PDF.
- That PDF, plus your shipping name, address, phone, and email, is sent to **Lulu** to print and ship the book.
- Your payment is handled by **Stripe**. Card details go straight to Stripe; we don't see them. We keep a record of the order (what was ordered, the price, the order status, and a reference to the Stripe payment) so we can support you and handle refunds.
- The financial and order details of a purchase are kept as long as needed for tax, accounting, and dispute-resolution purposes, even if you later delete other data — this is a legal requirement that overrides ordinary deletion.

See the separate [Terms of Sale](terms.html) for how orders, pricing, and refunds work.

## Sharing

We do not sell your data. We do not share it for marketing. We do not share it with anyone outside the service providers listed above (Supabase, OpenAI, Sentry, and — only for photobook orders — Stripe and Lulu), each of which is bound by its own privacy terms and uses the data only to provide its piece of the service.

## Your controls

- **Edit or delete any memory** at any time, from inside the app.
- **Delete your entire account** from Settings → Delete Account. This permanently removes all of your memories, photos, child profiles, and your account itself from our servers. It is not a soft delete.
- **Apple's "Hide My Email"** is fully supported — sign in with the relay address and the app works normally.

## Retention

Your data persists for as long as you keep your account. When you delete your account, we wipe your Supabase database rows, your storage objects (photos), and your Supabase auth user. There is no backup we hold onto afterward for "recovery" purposes — once it's gone, it's gone.

The one exception is photobook purchase records. If you've ordered a book, the order and payment record (not your memories or photos — just the transaction details) is retained as required for tax and accounting law, even after account deletion.

## Security

Supabase row-level security policies enforce per-account isolation at the database layer: your account can only read and write its own rows. Storage objects (your photos) are stored in private buckets and are only retrievable via authenticated requests scoped to your account.

## Changes to this policy

If this policy changes, the version on this page will be updated and the effective date at the top will be bumped. If a change materially affects how your data is handled, the app will surface a notice so you actually see it rather than relying on you checking this page.

## Contact

For privacy questions, deletion requests, or anything else related to your data in LittleDays:

**littledaysllc@gmail.com**
