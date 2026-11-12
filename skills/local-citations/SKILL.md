---
name: local-citations
description: Use when the user wants to build, audit or clean up local citations and business listings, fix NAP (name, address, phone) inconsistencies, remove duplicate listings, or asks which directories a local business should be listed on. Produces a NAP standard, a citation audit and a prioritized listing tracker.
---

# Local Citations

Citations are mentions of a business's name, address and phone number on other sites. Today they matter less for rankings than they used to, but consistent, accurate listings on the important platforms still build trust and send real customers. Quality beats quantity.

## Before you start

1. Read `.agents/seo-context.md` for the exact NAP and GBP details.
2. Ask for any old names, old addresses, old phone numbers, or previous agencies that built listings.
3. Note the country. Important directories and data aggregators differ by country.

## Step 1: NAP standard

Write the one official format and use it everywhere:
- Name: exactly as on GBP
- Address: same abbreviations every time (e.g. "St" or "Street", not both); SABs that hide their address on GBP should keep it hidden where platforms allow
- Phone: one main local number. If call tracking is needed, use the tracking number as primary only where the platform allows and keep the main number as an additional number.
- Website URL: same version (https, www or not)

## Step 2: Audit existing listings

- Search: business name, phone number, old phone numbers, old addresses
- Record each listing: platform, URL, NAP as shown, status (correct / wrong / duplicate / closed)

## Step 3: Priority listings

1. **Core**: Google Business Profile, Bing Places, Apple Business Connect, Facebook, Yelp
2. **Country basics**: main data aggregators and national directories for the client's country, BBB (US/Canada)
3. **Industry**: e.g. Angi, HomeAdvisor, Thumbtack, Houzz, Porch, Nextdoor for home services; Zillow, Realtor.com for real estate
4. **Local**: chamber of commerce, city or county directories, local business associations
5. **Avoid**: low-quality bulk directories and spammy link-farm lists

## Step 4: Fix and build

- Fix wrong listings first, then remove duplicates, then build missing core and industry listings
- Use the same description, categories, hours, logo and photos everywhere
- Save logins in the client's name (not the agency's)

## Output format

```markdown
## NAP standard
## Citation tracker
| Platform | Priority | Status | Listing URL | NAP correct? | Action | Owner | Done |
|---|---|---|---|---|---|---|---|
## Duplicates to remove
## Next steps
```

## Rules

- Never create listings with fake addresses or for locations the business does not have.
- Do not promise ranking jumps from citations alone.

## Related skills

`local-seo-audit`, `google-business-profile`, `review-management`, `link-building`
