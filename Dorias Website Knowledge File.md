# Doria Website — Project Status

Last updated: May 2026
**Who she is** My wife is a trained sexologist and therapist based in Querétaro, Mexico. Her practice in Mexico is called Doria Sexologa. For US clients she presents as a sex and intimacy coach — not a therapist — for legal reasons. She is bilingual but her US target market is Spanish-speaking clients residing in the US.

**Her style** Warm and nurturing when clients need safety, direct and clinical when they need clarity. She moves between the two naturally. Content tone: provocative yet educational. Think: a trusted expert who isn't afraid to say the thing nobody else will say.

**Client pain points she works with**

- Low sexual desire
    
- Disconnection from their own bodies — often rooted in Catholic guilt and shame around pleasure (she has female clients who cannot identify the clitoris on an anatomical model)
    
- Poor communication with partners
    
- Relationship conflict, emotional distance, infidelity, sexual incompatibility
    

**Her offer** One-hour video sessions via Zoom. She trained in long-form therapy, not brief therapy — she works with clients ongoing until the work feels complete. No fixed package yet for US coaching clients; this may need to be developed.

**Quiz funnel (approved questions on file in Spanish)** Goal: qualify and segment Spanish-speaking US leads who are ready to talk. Quiz title candidates: "Diagnóstico de tu Relación e Intimidad" / "¿Qué está bloqueando tu relación?" Questions cover: relationship status, main concern (desire, communication, conflict, trust, emotional distance, sexual differences), satisfaction level, urgency, and readiness to work. Funnel: quiz → auto-score → personalized email follow-up → booked call.

**Content system (phased)**

- Phase 1: Canva Pro — repurpose and draw inspiration from proven viral content in her niche, in Spanish
    
- Phase 2: Voice note → structured content → scheduled posts (automation system to be built by Brian)
    
- Phase 3: On-camera podcast-style content when she's comfortable
    

**Platforms**

- Instagram — uses daily, comfortable with Brian managing
    
- WhatsApp — uses daily, likely distribution and client contact channel
    
- TikTok — not comfortable on camera herself, comfortable with Brian managing
    
- LinkedIn — has account
    

**Future possibility** Curated adult toy recommendations or affiliate shop. She already incorporates product education (vibrators, pleasure toys) into her client sessions. Natural brand extension when the time is right.

**Brian's role** Building the quiz funnel, automation stack, and content system. This is also a real portfolio project for MindshiftOS LLC.
## What exists
- `public/index.html` — single page site (built via Claude Code). Deployable files live in `public/`; this knowledge doc stays at repo root and is NOT served.
- `public/gracias.html` — branded thank-you page the contact form redirects to
- GitHub repo ✅: https://github.com/bbrenz001/doria-website
- **Live at https://doriaalvarez.com** — hosted on Netlify (site `adorable-queijadas-09b79a`, MindshiftOS LLC team)
- **Continuous deploy ✅ (2026-08-29):** every `git push` to `main` auto-deploys. Netlify config: branch `main`, publish dir `public`, no build command (`netlify.toml`). Wired via Netlify deploy key + GitHub push webhook.
- doriasexologa.com to redirect to doriaalvarez.com — not done yet

## Framing (updated 2026-09-05)
- Public title: **"Sexóloga · Asesora en Relaciones e Intimidad"** (hero, `<title>`, meta description, footer, About-section body copy — all 5 occurrences updated).
- Never "Coach"/"Coaching" — Doria can lose her Mexico therapist license if seen advertising as a "Coach" here. **"Asesoría" is the replacement family of terms for "coach/coaching"**, per Brian 2026-09-05 — used "Asesora" (not "Consultora") as the actual on-page noun for grammatical parallelism with "Sexóloga" (both person-role nouns). Never "Psicóloga/terapeuta" toward US clients (US legal). "Sexóloga" is kept — it's her real Mexican credential and the @doriasexologa brand.
- Edited in the site's `public/index.html` 2026-09-05, **not yet pushed** — confirm the "Asesora" (vs. literal "Asesoría") word choice before this goes live, and this is still pending Doria's own final sign-off same as the "Consultora" wording was.

## Contact form (2026-08-29)
- Netlify Forms (`data-netlify="true"` + `bot-field` honeypot), form name `contact`, fields name/email/message. Redirects to `/gracias.html`.
- Submissions emailed to brenzelbrian@gmail.com (Netlify form notification hook). Also visible in Netlify dashboard → Forms.
- The Tally/Make.com quiz funnel is NOT wired to the site right now — Doria paused it. If it comes back it gets rebuilt in n8n.

## Tech stack
- Plain HTML/CSS, no framework
- Google Fonts: Cormorant Garamond + DM Sans
- No backend yet

## Decisions made
- Hero photo ✅ — Photo_Doria.JPG in both hero and About sections; responsive: stacked crop on mobile, side-by-side on tablet (iPad looks great), nav-offset positioning on laptop
- Photo filename: Photo_Doria.JPG (already in project folder)
- All "Agenda una llamada" buttons link to WhatsApp with pre-filled message:
  https://wa.me/5214421195049?text=Hola%20Doria%2C%20me%20gustar%C3%ADa%20saber%20m%C3%A1s%20sobre%20tu%20trabajo.

## El Proceso — approved copy ✅ implemented in index.html
1. Cuéntame cómo estás — quiz, no clinical language
2. Te escribo personalmente — Doria responds manually for now
3. Agendamos tu primera sesión — 30 min / $30 USD discovery call

## Booking flow
- "Agenda una llamada" buttons → Calendly (direct)
- Quiz CTA → quiz page → Doria sends Calendly link personally via WhatsApp

## Next session tasks
- [x] ~~Purchase doriaalvarez.com~~ — done, live on Netlify
- [x] ~~Contact form~~ — done (Netlify Forms → email), 2026-08-29
- [x] ~~Continuous deploy from GitHub~~ — done, 2026-08-29
- [ ] Doria's sign-off on the "Asesora en Relaciones e Intimidad" wording (updated 2026-09-05 from "Consultora")
- [ ] Set up Calendly for Doria + connect to Stripe ($30 USD / 30 min) — deferred, no booking link on site yet
- [ ] Add testimonials section once responses come in
- [ ] doriasexologa.com → doriaalvarez.com redirect
- [ ] (only if quiz is reactivated) rebuild quiz funnel in n8n

## Testimonial outreach
- WhatsApp message drafted in Mexican Spanish — ready to send
- Ask for first name or anonymous, keep it low pressure

## Business context
- US clients only (coaching framing, not therapy — legal requirement)
- Spanish-speaking Latinas in the US
- Full sessions: $150–200/hr target
- Discovery call: $30 / 30 min (filters leads, not a revenue line)
- Doria has capacity for 1–2 discovery calls per day