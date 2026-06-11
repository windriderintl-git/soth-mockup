# SOTH Website Redesign — Board Brief

**Prepared:** June 10, 2026 · **Status:** Mockup for board feedback
**What this is:** A complete, clickable redesign mockup of sothchurch.com (12 pages, open `index.html` in any browser), plus the research and rationale behind it.

---

## 1. Why redesign

The current Squarespace site (built ~2020) has good content but works against us in four measurable ways:

| Problem | Evidence from the current site |
|---|---|
| **Invisible to search engines** | Every page has an *empty* meta description; the homepage has no H1 heading; the structured-data block Google reads has no name, address, phone, or hours; a dead pre-2020 URL (`/newsletters.html`) still shows up in Google and 404s. We rank #1 only for our own name. |
| **Hard on first-time visitors** | "First Time Visitors" is buried in a dropdown; no map, no parking info, no office hours anywhere; Zoom/YouTube/recordings links are scattered; Pastor Yolanda — our strongest differentiator — is 3 clicks deep. |
| **Welcome statement under-leveraged** | Our best asset for the progressive-church seeker sits below the fold on the homepage and never appears in search snippets. The site never says "ELCA" prominently or names what inclusion means in practice. |
| **Members underserved** | No events calendar (Campfire/Dinner Church dates live in prose), newsletter is a wall of PDFs, no contact form, portal links exist but no member hub. |

## 2. What we studied

Deep structural/design/SEO analysis of 10 churches you suggested: **CPC Edina, Church of the Resurrection (Leawood), Cathedral of Hope (Dallas), Lutheran Church of Hope (W. Des Moines), Mt. Olivet (Mpls), Trinity UCC (Chicago), Windsor Village/Kingdom Builders (Houston), Hosanna (Lakeville), Concordia (San Antonio), Grace Church (Eden Prairie)** — plus a full audit of our own live site.

**The patterns the best sites converge on (all adopted in this mockup):**

1. **"I'm New" is the first nav item and the hero's primary button.** One obvious front door. (CPC, Resurrection, Cathedral of Hope)
2. **Service time + address at zero clicks** — visible on the homepage *and* in the footer of every page. The #1 and #2 visitor questions, answered before any clicking. (Every strong site)
3. **What-to-expect logistics beat welcome prose.** Dress code, parking, kids, communion, "how long is it really" — concrete promises reduce first-visit anxiety more than any paragraph about hospitality. (Mt. Olivet's promise list, Grace's door-by-door guide, Windsor's "what to wear")
4. **One multi-purpose contact form** with an "I'd like to…" dropdown (talk to pastor / plan visit / get connected / request care), instead of five scattered forms. (CPC — the single highest-leverage low-budget pattern we found)
5. **Named humans, not departments.** Every next step ends at a real name with a real inbox — a small church's unfair advantage over megachurches. (Mt. Olivet, Hosanna, Concordia)
6. **One welcome sentence repeated everywhere**, plus structural proof. Cathedral of Hope repeats "No matter who you are or where you are on life's journey, you're welcome here" on every page — and backs it with resources and programming. Resurrection's board-adopted "Statement of Belonging" leads their sitewide search description.
7. **Per-service personality descriptions** ("come-as-you-are," "about an hour," "kids welcome") so people can self-select comfortably. (Lutheran Church of Hope)
8. **SEO basics are an open lane.** Almost every big church we studied has weak titles, missing descriptions, and no Church schema. A small church doing this correctly can outrank bigger ones for local searches like *"inclusive church Edina"* or *"LGBTQ affirming church Minneapolis."*

**What we deliberately did NOT copy** (doesn't scale to our budget): autoplay video heroes, member-portal platforms, multi-campus apparatus, daily content machines, mega-menus, native apps.

## 3. The new site

### Structure (12 pages)

| Page | Job |
|---|---|
| `index.html` Home | Orient in 5 seconds: who we are, when/where, three pathways (visit / belong / worship), welcome statement, Pastor Yolanda, this week, kids, members strip |
| `new-here.html` **Plan Your Visit** | The conversion page: 4-step first visit, honest logistics, visit-note form, map, 8-question FAQ |
| `worship.html` Worship | Weekly schedule, what worship feels like, sermon series, **one consolidated "watch online" section** (Zoom + YouTube + bulletin) |
| `belong.html` **Our Welcome & Beliefs** | Full welcome statement verbatim, "welcome as practice" (6 concrete proofs), the four belief statements, ELCA affiliation |
| `about.html` Staff & Leadership | Pastor Yolanda feature, all staff with photos + emails, council, building/AV |
| `kids-youth.html` | PrayGround → milestones → confirmation/youth → parent supports → safety + named contact (Aym) |
| `connect.html` Groups & Care | All adult groups; care ministries incl. Mental Health Connect; "need care today" phone CTA |
| `serve.html` Serve & Partners | Sunday roles, quilters, Onward feature, 22 partner organizations |
| `events.html` | This week + recurring rhythms + seasonal traditions (replaces "no calendar at all") |
| `give.html` | Theology-first giving page (new — currently we dump people straight to Vanco), ways to give, transparency note, "visitors: don't feel obligated" |
| `members.html` | One hub: portal, directory, newsletter, giving, volunteering, council business |
| `contact.html` | Real-person framing, who-to-ask-for-what, intent-dropdown form, embedded map |

**Navigation (7 items max + Give button):** I'm New · Worship · Kids & Youth · Connect ▾ · About ▾ · Events · Members · **Give**
**Utility bar on every page:** service time · address · phone · Watch Online.

### Design language

- **Warm paper background, deep plum + teal + honey gold** — evolved from the current purple identity, dignified but warm; reads "rooted *and* progressive" rather than corporate.
- **Source Serif (display) + Inter (body)** — free Google fonts, serif warmth + clean readability.
- Fully responsive (phone-first), accessible (skip links, focus states, ARIA labels, semantic headings), zero JavaScript dependencies — works on any platform including current Squarespace as a rebuild reference, or a cheap static/WordPress build.

### Inclusivity treatment (per your goal)

- Welcome statement quoted **verbatim** as the homepage centerpiece and a full page (`belong.html`), with each named group given visual weight.
- New **"What that welcome looks like on an actual Sunday"** section converts the statement into six concrete practices (LGBTQ+ affirmation incl. marriage/leadership, doubt honored, accessibility, kids, economic, neighbors) — this is the section seekers screenshot and share.
- The first-visit FAQ answers the real question directly: *"I'm LGBTQ+. Am I actually welcome, or just tolerated?"*
- Pride flag photo used purposefully (homepage pathway card + belong page hero), pronouns shown for staff, ELCA badge in hero.

### SEO build (all implemented in the mockup)

- Unique, keyword-bearing `<title>` on every page (pattern: *Page — keywords | Shepherd of the Hills Lutheran Church | Edina, MN*).
- Unique meta description on every page — the homepage one leads with the welcome, so our search snippet *is* our welcome.
- Proper H1 on every page; semantic heading hierarchy.
- **Church/PlaceOfWorship JSON-LD** with full name/address/phone/email, Sunday service Event schedule, ELCA membership, social profiles — on the homepage.
- **FAQPage schema** on Plan Your Visit (eligible for FAQ rich results on queries like "what to wear to a Lutheran church").
- **Person schema** for Pastor Yolanda; OpenGraph tags sitewide; canonical URLs; embedded Google Map (a local-SEO signal); `noindex` on the members page.

## 4. Imagery — shot list for our photographer

All grey-gradient images labeled **"MOCK PHOTO"** are placeholders. Carrie can replace them with one Sunday-plus-one-Wednesday shoot:

1. Hero: wide, warm shot of congregation + building exterior (replaces current hero.png if desired)
2. Pastor Yolanda — portrait + preaching/greeting candid
3. Each staff member — square portrait
4. PrayGround with kids in it (faces with photo releases, or shot from behind)
5. Coffee hour conversation · 6. Communion at the rail · 7. Greeter at the door · 8. Quilters in Ranum Hall · 9. Dinner Church tables · 10. Youth group · 11. Sunday School · 12. Music leaders · 13. Building/grounds exterior
- Already usable: `hero.png`, `campfire.png`, `pride_flag.png`

## 5. Needs board/office confirmation before launch

- **Parking & arrival specifics** (mockup says "free lot, accessible spaces near entrance" — verify wording and which doors).
- **Office hours** (none published anywhere today — decide and publish; also needed for Google Business Profile).
- **Phone number discrepancy:** main listing is 952-935-3457, but the live volunteer page shows 952-234-4721 — confirm and fix.
- **Pastor Yolanda's homepage quote** is a placeholder — she should write her own two sentences.
- **Reconciling in Christ:** our welcome statement is RIC-style but we never claim the designation. If we *are* RIC, say so (it's a search term seekers use); if not, consider pursuing it.
- Safety/safe-church language on kids page — confirm it matches actual policy.
- Event dates shown (June 2026) are samples; the real site needs a maintainable events source (even a simple Google Calendar embed).
- Geo coordinates in any future schema should be verified against Google Maps.

## 6. Launch checklist (when approved — beyond the mockup)

1. **301 redirects** from all current Squarespace URLs (`/what-to-expect`, `/recordings`, `/leadership`, etc.) to new paths — and finally redirect the long-dead `/newsletters.html`.
2. **Google Business Profile**: claim/refresh with hours, photos, service times; this drives more local discovery than the website itself.
3. Submit XML sitemap in Google Search Console; verify the FAQ/Church schema with Google's Rich Results test.
4. Newsletter form → connect to a real email tool (even free Mailchimp tier) instead of "email the office."
5. Contact/visit forms → any free form service (or Squarespace native forms if staying on the platform).
6. Add Instagram (families discover churches there; we currently only have Facebook).
7. Retire the unused Squarespace commerce cart and duplicate folder URLs if remaining on Squarespace.

**Cost posture:** Everything in this design uses free fonts, free icons, our own photos, and existing services (Vanco, Servant Keeper, Zoom, YouTube). No video production required. The only ongoing costs are the website platform we already pay for and ~1–2 hrs/week of content upkeep (events + weekly email), which fits Carrie's existing role.
