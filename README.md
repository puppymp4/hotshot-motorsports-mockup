# Hotshot Motorsports - Spec Build

Spec website for **Hotshot Motorsports** in Fresno, CA.

- **Business:** Custom truck shop. Lift kits, forged wheels, custom lighting, vinyl wraps, color match, audio, full SEMA-grade builds.
- **Address:** 3770 N Marty Ave, Fresno, CA 93722
- **Phone:** (559) 396-9670
- **Email:** Hotshotmotorsport@yahoo.com
- **Instagram:** [@hotshotmotorsports](https://www.instagram.com/hotshotmotorsports/) (21K followers, 700+ posts)
- **Current site:** [builtbyhotshot.com](https://builtbyhotshot.com) (GoDaddy template, mostly placeholder content)

## Built by Rift Media

Single-file HTML/CSS/JS spec build. No framework, no build step, deploys static to Vercel.

### Stack
- Vanilla HTML / CSS / JS in a single `index.html`
- Google Fonts: Archivo (display) + Inter (body) - "Performance Shop" pairing from Rift Media font library
- LocalBusiness JSON-LD schema for SEO
- Sitemap.xml + robots.txt
- Real build photos sourced from his public IG (@hotshotmotorsports)

### Local preview
Open `index.html` directly in a browser, or:
```
npx serve .
```

### Pages / Sections
1. Sticky nav with mobile drawer
2. Full-bleed hero with chrome+ember gradient H1
3. Marquee strip of services
4. Six-card service grid (lift, wheels, lighting, wrap, audio, full builds)
5. 12-tile builds gallery (real customer trucks)
6. Four-step process
7. Stats + brand partners row
8. Multi-step contact form (5 steps, inline validation, success state)
9. Contact info + Google Maps embed
10. Footer with sitemap

### SEO
- Title + meta description tuned for "Fresno custom truck shop" intent
- LocalBusiness + AutomotiveBusiness schema with hours, address, geo, services
- Open Graph + Twitter card meta with hero build photo
- Sitemap with image entries
- Image alt text on every photo

### Deploy notes
- Public repo: github.com/puppymp4/hotshot-motorsports-mockup
- Vercel project: hotshot-motorsports-mockup
- Production URL: hotshot.riftmedia.cc (Porkbun CNAME -> cname.vercel-dns.com)
- vercel.app fallback: hotshot-motorsports-mockup.vercel.app

### Replacement notes for production handoff
- Form submit currently shows success state only. Wire to Formspree, Resend, or a /api endpoint before production launch.
- Replace placeholder map with custom-styled embed (Google Maps API key) if needed.
- Service area cities (Clovis, Madera, Visalia) listed in schema for local SEO. Add city-specific landing pages if SEO budget exists.
- IG photos are sourced from his public business account. For production, swap with high-res originals from his camera roll.
