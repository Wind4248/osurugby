# OSU Rugby — Team & Alumni Website

Website for Ohio State University Men's Rugby Football Club and the Men's Rugby Alumni Society.

## Project Status: Planning Phase

## Site Purpose

Consolidate the fragmented OSU Rugby web presence (osurugby.com, u.osu.edu/osurugby, alumni society page) into a single, modern website that serves current players, recruits, alumni, and fans.

## Hosting

- GitHub Pages via `Wind4248/osurugby` repo
- Custom domain: TBD (possibly osurugby.com if obtainable, or osurugbyalumni.com)
- Push to `main` to deploy

## Tech Stack

- **Static site** hosted on GitHub Pages
- **Decap CMS** (formerly Netlify CMS) for content management — allows non-technical users to update roster, schedule, blog, and photos through a web UI, backed by GitHub
- **Cloudinary** (free tier) for image hosting and optimization — handles photo uploads and serves optimized images
- **HTML/CSS/JS** — no heavy frameworks, fast loading
- All pages are individual HTML files (like josephalotozo.com pattern)

## Design System

- **Colors:** Scarlet `#BB0000`, Gray `#666666`, White `#FFFFFF`, Black `#1A1A1A`, Light Gray `#F5F5F5`
- **Fonts:** Oswald or similar bold sans-serif (headings), Open Sans or similar (body)
- **Style:** Clean, athletic, modern — inspired by Penn State Rugby's polished Squarespace look
- **Responsive:** Mobile-first design

## Site Structure

```
/osurugby/
  index.html              ← homepage (hero, news highlights, next match, quick links)
  roster.html             ← current season roster with player cards
  schedule.html           ← upcoming matches + past results
  history.html            ← program history (founded 1966), achievements, records
  alumni/
    index.html            ← Alumni Society hub (mission, membership, events, donate)
    hall-of-fame.html     ← Hall of Fame inductees
    directory.html        ← Alumni directory / network (future phase)
  blog/
    index.html            ← news/blog listing
    [posts].html          ← individual posts (match recaps, spotlights, announcements)
  gallery/
    index.html            ← photo gallery grid (pulls from Cloudinary)
  recruit.html            ← prospective players info + contact form
  donate.html             ← donation page (link to OSU giving + Gavin Gill fund)
  store.html              ← merchandise (external link or embedded store)
  contact.html            ← contact form + social links
  assets/
    images/               ← local images (logo, favicon, etc.)
    css/                  ← stylesheets (if we move away from inline)
    js/                   ← scripts
  admin/
    index.html            ← Decap CMS admin panel
    config.yml            ← CMS configuration
  CNAME                   ← custom domain
  sitemap.xml
```

## Content Sources

- **Team info:** OSU Rugby leadership, Coach Tom Rooney
- **Alumni info:** Men's Rugby Alumni Society (osurfcalumni@gmail.com, Russ Howland)
- **History:** u.osu.edu/osurugby/sample-page/ has founding story
- **Photos:** @buckeyerugby Instagram, alumni Facebook (OSURFCALUMNI), program archives
- **Schedule/Results:** Big Ten Rugby Conference, Goff Rugby Report, CRAA

## Key Program Facts

- Founded: 1966 by two physicians at University Hospitals
- Level: D1A (highest men's college rugby)
- Conference: Big Ten Rugby → Midwest D1A (Fall 2026)
- Head Coach: Tom Rooney (2024 Big Ten Coach of the Year)
- Facilities: Two full-sized lit fields on campus
- Recent: 2024 Big Ten Champions
- Alumni Society email: osurfcalumni@gmail.com / mensrugbysociety@osu.edu
- Gavin Gill Memorial Scholarship Fund

## Audience Segments (Penn State model)

1. **Current Players** — roster, schedule, team news
2. **Prospective Players / Recruits** — program info, how to join, contact
3. **Alumni** — society info, Hall of Fame, events, donate, directory
4. **Parents & Fans** — schedule, results, photos, blog

## Phase Plan

### Phase 1: Foundation (Current)
- Homepage with hero, program overview, next match, news highlights
- Roster page
- Schedule page
- History page
- Contact page
- Basic responsive design

### Phase 2: Alumni & Community
- Alumni Society section (mission, membership, events)
- Hall of Fame
- Donation integration
- Blog with match recaps

### Phase 3: Media & Engagement
- Photo gallery with Cloudinary
- Decap CMS setup for content management
- Recruit page with contact form
- Merchandise store link

### Phase 4: Advanced
- Alumni directory
- Live match streaming links
- Email newsletter signup
- Audience-segmented landing pages
