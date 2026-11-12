---
name: location-pages
description: Use when the user wants to create, plan or improve location pages, city pages or service-area pages for a local business, or asks how to rank in nearby cities, how many city pages to build, or whether city pages are doorway pages. Plans which cities deserve a page and writes pages with unique local value instead of swapped city names.
---

# Location Pages

Location pages help a business rank in the cities it serves beyond its main address. Done badly (same text, city name swapped) they are doorway pages, which violate Google's spam policies. You build fewer, better pages with real local value.

## Before you start

1. Read `.agents/seo-context.md` for service areas, priorities and proof.
2. For each candidate city, collect: search demand for the main services, jobs done there, reviews from customers there, travel time, local specifics.

## Decide which cities get a page

A city gets its own page only if:
- The business really serves it regularly
- There is search demand (GSC impressions, tools, or clear SERP evidence)
- You can add unique local content (projects, reviews, local factors)

Otherwise list the city on a general "Service Areas" page. Five strong city pages beat fifty thin ones.

## Unique local content (each page needs several of these)

- Real projects done in that city (photos, neighborhood, problem, result)
- Reviews from customers in that city
- Local factors: climate and weather issues, building codes, permits, HOA rules, typical home age and styles, water hardness, soil
- Neighborhoods and nearby areas served, typical response time
- Team members based there, or a real office (only if it exists)
- Local partnerships, sponsorships, community work

If the client cannot provide any of this for a city, recommend not building that page yet.

## Page structure

1. H1: "{Main service} in {City}" (or "{Brand} in {City}" if the page covers all services)
2. Intro: services offered in this city and why customers there choose the business
3. Services available in {City} (short sections, each linking to its service page)
4. Local projects in {City}
5. Reviews from {City} customers
6. Local factors (what is different about this city for this service)
7. Areas / neighborhoods covered
8. FAQs specific to the city (permits, response time, pricing factors there)
9. CTA

## SEO details

- URL: `/service-areas/{city}/` or `/{city}/{service}/` for high-value combos
- Title: `{Service} in {City}, {State} | {Brand}`
- Internal links: from the Service Areas hub, from relevant service pages, to the service pages
- Schema: `Service` with `areaServed` set to the city, linked to the business `@id`. Do not add a fake LocalBusiness address for a city without a real office.

## Output

1. City priority table: City | Demand evidence | Jobs / proof available | Build now / later / no
2. Page template with required unique fields
3. Full draft for the requested cities, with `[CLIENT TO PROVIDE]` placeholders where local proof is needed

## Rules

- Never swap city names into identical text.
- Never invent projects, reviews or local facts.

## Related skills

`service-pages`, `site-architecture`, `local-seo-audit`, `seo-content-writing`, `schema-markup`
