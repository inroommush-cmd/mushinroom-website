# MushInRoom Website

Premium Next.js 15 website for MushInRoom — India's premier Cordyceps militaris cultivation startup.

## Tech Stack

- **Framework:** Next.js 15 (App Router)
- **Language:** TypeScript
- **Styling:** Tailwind CSS
- **Animations:** Framer Motion
- **UI Components:** Radix UI primitives + custom components
- **Icons:** Lucide React
- **Theme:** next-themes (dark/light mode)
- **Notifications:** Sonner
- **Fonts:** Space Grotesk (display) + Inter (body) + JetBrains Mono

## Getting Started

```bash
# Install dependencies
npm install

# Run development server
npm run dev

# Build for production
npm run build

# Start production server
npm start
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

## Project Structure

```
mushinroom/
├── app/
│   ├── about/page.tsx          # About page
│   ├── contact/page.tsx        # Contact page
│   ├── products/page.tsx       # Products page
│   ├── research/page.tsx       # Research & Lab page
│   ├── training/page.tsx       # Training page
│   ├── privacy/page.tsx        # Privacy policy
│   ├── terms/page.tsx          # Terms of service
│   ├── refund/page.tsx         # Refund policy
│   ├── shipping/page.tsx       # Shipping policy
│   ├── globals.css             # Global styles
│   ├── layout.tsx              # Root layout
│   ├── loading.tsx             # Loading animation
│   ├── not-found.tsx           # 404 page
│   ├── robots.ts               # robots.txt
│   └── sitemap.ts              # sitemap.xml
├── components/
│   ├── layout/
│   │   ├── Navbar.tsx          # Sticky navigation
│   │   └── Footer.tsx          # Animated footer
│   ├── providers/
│   │   └── ThemeProvider.tsx   # Dark/light mode provider
│   ├── sections/               # Page sections
│   │   ├── HeroSection.tsx     # Homepage hero with particle canvas
│   │   ├── StatsSection.tsx    # Animated counters
│   │   ├── FeaturedProducts.tsx
│   │   ├── WhyMushInRoom.tsx
│   │   ├── Testimonials.tsx
│   │   ├── FAQ.tsx
│   │   ├── ContactCTA.tsx
│   │   ├── AboutHero.tsx
│   │   ├── CompanyStory.tsx
│   │   ├── VisionMission.tsx
│   │   ├── TeamSection.tsx
│   │   ├── ProductsHero.tsx
│   │   ├── ProductsGrid.tsx
│   │   ├── ProductScience.tsx
│   │   ├── TrainingHero.tsx
│   │   ├── TrainingPrograms.tsx
│   │   ├── TrainingIncludes.tsx
│   │   ├── ResearchHero.tsx
│   │   ├── LabCapabilities.tsx
│   │   ├── ResearchFocus.tsx
│   │   ├── ContactHero.tsx
│   │   └── ContactSection.tsx
│   └── shared/
│       ├── ScrollToTop.tsx     # Scroll-to-top button
│       ├── SectionWrapper.tsx  # Reusable section components
│       └── LegalPage.tsx       # Legal page template
├── lib/
│   └── utils.ts                # cn() utility
├── public/
│   ├── favicon.svg
│   └── site.webmanifest
├── tailwind.config.ts
├── next.config.mjs
└── tsconfig.json
```

## Pages

| Page | URL | Description |
|------|-----|-------------|
| Home | `/` | Hero, stats, products, why us, testimonials, FAQ, CTA |
| About | `/about` | Story, vision/mission, team |
| Products | `/products` | All products with detailed specs |
| Training | `/training` | 2-day program packages and curriculum |
| Research | `/research` | Lab capabilities and research focus |
| Contact | `/contact` | Contact form, WhatsApp, location |

## Customisation

### Brand Colours
Edit `tailwind.config.ts` to update brand colours:
- **Orange (Primary):** `#F97316`
- **Emerald (Accent):** `#10B981`

### Contact Details
Search for `inroommush@gmail.com` and `919999999999` across the codebase and replace with actual values.

### Google Maps
In `ContactSection.tsx`, replace the map placeholder with an actual Google Maps embed.

### WhatsApp Number
Replace `919999999999` with the actual WhatsApp business number in:
- `components/layout/Footer.tsx`
- `components/sections/ContactCTA.tsx`
- `components/sections/ContactSection.tsx`
- `components/sections/ProductsGrid.tsx`

## Deployment (Vercel)

1. Push to GitHub
2. Connect repository to Vercel
3. No environment variables required for basic deployment
4. Vercel will auto-detect Next.js and configure the build

```bash
# Or deploy via Vercel CLI
npx vercel --prod
```

## SEO

- Metadata configured in each `page.tsx` file
- `robots.ts` generates `/robots.txt`
- `sitemap.ts` generates `/sitemap.xml`
- Open Graph metadata set in `app/layout.tsx`
- **Replace** `https://mushinroom.com` with actual domain before deployment

## Adding Real Images

Replace placeholder elements with real images:
1. Add images to `/public/images/`
2. Use Next.js `<Image>` component
3. Update `next.config.mjs` if using external image sources

## License

Proprietary — MushInRoom / Tithika Agritek Pvt. Ltd.
