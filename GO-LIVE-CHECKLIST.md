# Store — go-live checklist (Uganda)

**It already takes orders — no payment account needed.** All 14 sellable products
now have a **"Buy" button that opens a WhatsApp order** to **+256 753 717508**
with the product name pre-filled. A customer taps Buy → chats you → you confirm
**Mobile Money** and send the file. Zero signup, zero fees. (The 3 "Coming soon"
items are locked membership/ebook tiers the pipeline has not unlocked yet.)

**To change the order number:** edit `PHONE` in the wiring step and rebuild, or
ask me. **To upgrade to automatic checkout** (card + auto-delivery) later, follow
the provider steps below — WhatsApp orders keep working until you do.

See `SETUP.md` for the full provider comparison. This is the short version.

## 1. Pick a checkout provider (the only gated step)

For a **Ugandan / East African audience**, take **mobile money**, not just cards —
it converts far better:

| Best pick | Why |
|---|---|
| **Flutterwave** (recommended) | MTN + Airtel mobile money, cards, multi-currency, pan-African payouts. |
| **Paystack** | Also strong in the region; clean digital-product flow. |
| **Gumroad** | Fastest to a first sale (10% flat), pays out via PayPal/bank — good to start today. |
| **Lemon Squeezy** | If you sell internationally: it handles VAT as merchant of record. |

Create a free account, add each product there, and copy its checkout link.

## 2. Wire the links in (I can do this for you)

For each product, paste its checkout URL:
```
bryson-studio products link <product-id> --url <checkout-url>
```
Then rebuild so the buttons go live:
```
bryson-studio store build
```
Product ids are the file names in `store\p\` (e.g. `education-print-set`).
**Send me the provider links and I'll run these for you.**

## 3. Put it online free

Drag the **`data\store`** folder (or `store-site.zip`) onto **https://app.netlify.com/drop**
— live in ~60 seconds. Or use GitHub Pages. Then record the public URL so the
catalog feeds point at real pages:
```
bryson-studio store url https://your-store-url
```

## 4. Point everything at it
Put the store URL in every video description, the pinned comment, and every bio.
Per `SETUP.md`, your own storefront is the foundation — platform shops
(YouTube/TikTok/Meta) are added later and each has eligibility walls.

---
Status: built ✓ · packaged ✓ · **waiting on: your checkout links** · then host.
© 2026 Grass To Grace Media.
