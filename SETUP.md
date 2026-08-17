# Store setup

## Do this in order

1. **Pick a checkout provider** from the table below and create your products there. This is the only step that involves anyone else.
2. **Paste each checkout URL back in:** `bryson-studio products link <product-id> --url <checkout-url>`
3. **Rebuild:** `bryson-studio store build` — the buy buttons go live.
4. **Host this folder** on GitHub Pages, Netlify or Cloudflare Pages. All three are free and none of them need a build step.
5. **Record the public URL:** `bryson-studio store url <https://...>` so the catalogue feeds point at real pages.
6. **Link it everywhere** — every video description, every bio, the pinned comment, the channel banner.

## Checkout providers

| Provider | Best for | Fee | Payouts | Notes |
|---|---|---|---|---|
| Gumroad | digital products, fastest setup | 10% flat | worldwide via PayPal/bank | Lowest-friction way to take your first payment. No store build required. |
| Lemon Squeezy | digital products, handles sales tax/VAT as merchant of record | 5% + 50c | wide | Merchant of record means they handle VAT/tax compliance for you, which is worth the fee once you sell internationally. |
| Stripe Payment Links | anything, lowest fee | ~2.9% + 30c | supported countries only | Cheapest, but you own tax compliance and Stripe is not available in every country. |
| Paystack | Nigeria, Ghana, South Africa, Kenya | ~1.5-3.9% | local bank | Local cards and mobile money. Far higher conversion than a foreign processor for African audiences. |
| Flutterwave | pan-African, multi-currency | ~1.4-3.8% | local bank, mobile money | Broad African coverage including mobile money, which matters more than card support in several markets. |
| Ko-fi | small digital items, tips, memberships | 0% on the free tier | PayPal/Stripe | No platform cut on the free plan. Good for a first cheap product. |
| Shopify | physical goods, and required for YouTube Shopping | monthly plan + card fees | wide | The heavyweight option. Only worth it once you sell physical products or specifically need YouTube Shopping. |
| Fourthwall | creator merch, POD built in | product cost, no monthly | wide | Print on demand, storefront and YouTube Shopping connection in one, with no monthly fee. Strongest starting point for merch. |

## Platform shops — what each one actually requires

This is the section worth reading twice. Most attempts to open a store on a channel fail here, and almost always for a reason that is not obvious from the platform's own marketing.

### YouTube Shopping (the Store tab)

**Requirements**

- Channel must be in the YouTube Partner Programme
- 1,000+ subscribers (higher for some regions and for the affiliate programme)
- Connect an APPROVED merchant partner - Shopify, Fourthwall, Spring, Spreadshop and a handful of others
- Channel not set as made for kids, no strikes, monetization enabled
- Available only in supported countries

**Where it usually goes wrong.** You cannot simply add a store to a YouTube channel. The Store tab appears only after you are in the Partner Programme AND you have connected one of YouTube's approved merchant partners. A Gumroad link or your own website will not connect - those platforms are not on the approved list. This is the reason almost every attempt to 'start a store on my channel' stalls.

**What to do instead.** Until you are eligible, put the storefront link in the video description, the pinned comment and the channel banner link. That works from your very first video, costs nothing, and converts better than most people expect.

### TikTok Shop

**Requirements**

- Available only in supported countries - check before you build anything
- Business verification with real documents
- 1,000+ followers for most creator selling features
- Product catalogue meeting TikTok's category rules

**Where it usually goes wrong.** Country availability is the wall. TikTok Shop is not open everywhere, and no amount of setup works from an unsupported market.

**What to do instead.** Link in bio to your own storefront, and mention the product verbally in the video rather than relying on a shop tag.

### Instagram / Facebook Shops

**Requirements**

- A Meta Commerce Manager account and a product catalogue
- A connected Facebook Page and business account
- Compliance with Meta's commerce policies - digital-only goods are restricted in several regions
- Supported country

**Where it usually goes wrong.** Meta commerce policy restricts purely digital products in many markets. Physical merch clears review far more easily than an ebook does.

**What to do instead.** Use the catalogue for physical products and a link in bio for digital ones. This system writes a Meta-compatible catalogue CSV either way.

### X

**Requirements**

- No general creator shop; link only

**Where it usually goes wrong.** There is no storefront to build here.

**What to do instead.** Pinned post plus profile link.

### Your own storefront

**Requirements**

- A hosted page and a checkout link

**Where it usually goes wrong.** None. This is the one nobody can switch off.

**What to do instead.** This system generates a complete static store you can host free on GitHub Pages, Netlify or Cloudflare Pages, then link from every platform. Start here, always - platform shops are a distribution channel added later, never the foundation.

## Catalogue feeds

- `catalog-meta.csv` — upload in Meta Commerce Manager to create a catalogue for Facebook and Instagram Shops.
- `catalog-google.csv` — upload to Google Merchant Center.

Both files use a placeholder domain until you run `bryson-studio store url <your-url>`. Upload them with the wrong domain and every product fails review on an unreachable link.

## Legal housekeeping nobody enjoys and everybody needs

- A refund policy on the store page, before the first sale.
- Disclose affiliate links and sponsorships every time, in the video and in the description. It is a legal requirement in most markets, not a courtesy.
- Sales tax and VAT on digital goods depend on the *buyer's* country, not yours. A merchant of record like Lemon Squeezy handles this for you; Stripe and Gumroad largely do not.
- Never state or imply an income or outcome guarantee on a course or a guide. That is consumer protection law, and it is enforced.