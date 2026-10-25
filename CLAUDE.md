# Website build rules (Next Digital Level)

These rules apply to every site in this repo. Follow them without being reminded.

## Stack and hosting
- Static site only: plain HTML, CSS and vanilla JavaScript. No frameworks, no build step, no npm.
- Hosted on GitHub Pages as a project site, served from `/<repo-name>/`.
- ALL paths must be relative: `css/style.css`, `images/hero.jpg`, `services.html`. Never start a path with `/`.
- Filenames are lowercase, no spaces, no accents (`a-propos.html`, not `À Propos.html`). GitHub Pages is case sensitive.
- `index.html` at the repo root. Include a `404.html` and a favicon.

## Mobile first
- Design for mobile first; most visitors open the link from WhatsApp on a phone.
- Must work perfectly at 375px, 768px and 1440px. No horizontal scroll at any width.
- Tap targets at least 44px. Readable text (16px minimum body size on mobile).
- Sticky or highly visible call button on mobile (`tel:` link). Add a WhatsApp button if a WhatsApp number is provided.

## Look and feel: professional, prestigious, NOT AI-generated
- Restrained palette built from the client's logo or trade. Max 2 brand colors plus neutrals.
- Real typography: one quality Google Font pairing, clear hierarchy, generous spacing.
- Avoid these AI tells:
  - purple/blue gradients, glassmorphism, glowing blobs
  - emoji used as icons (use simple inline SVG icons instead)
  - "Welcome to our website", "Your trusted partner", "Unlock", "Elevate", "Seamless"
  - em dashes in copy
  - three identical feature cards as the whole page
  - generic stock photos that don't match the trade
- Copy must sound like a real local business owner wrote it: concrete, short, specific to the trade and the city.

## Language and local conventions
- Site copy in French unless the brief says otherwise. Swiss French conventions: CHF, `+41` phone format, Swiss address format.
- Correct French spelling and accents everywhere.

## Local Google SEO (every page)
- Unique `<title>` and meta description containing the main service and the city.
- One `<h1>` per page that names the service and the city.
- `LocalBusiness` JSON-LD schema (name, address, phone, area served, opening hours) on the homepage.
- Embedded Google Map on the contact page if an address is provided.
- Descriptive `alt` text on every image. Clean headings (h1 > h2 > h3).
- Open Graph tags so the WhatsApp link preview shows a title, description and image.

## Performance
- Compress images (WebP where possible), set width and height, `loading="lazy"` below the fold.
- No heavy libraries. Minimal JavaScript.

## Honesty rules (strict)
- NEVER invent reviews, testimonials, ratings, client counts, years of experience, certifications or awards.
- NEVER invent an address, phone number, email or opening hours.
- If information is missing, use a clearly visible placeholder like `[TODO: numéro de téléphone]` and list every TODO at the end of your reply.

## Workflow
1. Read the client brief below. Before writing code, propose the page list and homepage sections in a few lines.
2. Build the site.
3. Check every page at 375px, 768px and 1440px and fix any layout issue.
4. Verify no path starts with `/` and every link and image resolves.
5. Commit with a clear message after each working version.
6. End with: what was built, the list of TODOs, and anything you assumed.

---

## Client brief (fill in for each project)
- Business name:
- Trade / services (only what they really sell):
- City and area served:
- Phone / WhatsApp:
- Email:
- Address:
- Opening hours:
- Logo and colors:
- Photos available:
- Pages wanted:
- Reference sites or style notes:
- Source info (Google Business link, Instagram, etc.):
