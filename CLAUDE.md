# CLAUDE.md — Fazil Rehman Personal Brand Site

## Goal
Build a fast, single-page personal brand site for **Fazil Rehman**, an SMB Account Executive targeting higher-paying, fully-remote SaaS sales roles. This is a job-hunt asset. In 5 seconds it should make a recruiter or sales leader think "this person closes, and they're sharp about how they show up." It backs his LinkedIn and resume.

## Audience
SaaS sales hiring managers, recruiters, and sales leaders at SMB-focused software companies. They skim. Land the pitch fast, let them dig if they want.

## Positioning (use this framing, don't invent metrics)
- **Title:** SMB Account Executive · SaaS & Technology Sales
- **One-liner:** Full-cycle SMB closer. 9+ years. Self-sourced pipeline, consultative selling, 107% of quota.
- **Proof points (use as the metric callouts):** 9+ years in sales · 107% of quota · $500 to $50K deal range · 4,000+ vendor portfolio · co-sell with Microsoft, Google, AWS, Cisco.
- **Tone:** confident, plain, no corporate fluff. Short punchy lines. No buzzword soup.

## Tech constraints (non-negotiable)
- **Single file.** Everything in one `index.html`: inline `<style>` and `<script>`. No build step, no framework, no npm, no bundler.
- Google Fonts via `<link>` is fine. Icons = inline SVG only, no icon library.
- Must deploy to **Netlify** by drag-and-drop of the folder, or `netlify deploy --prod`. Zero config.
- Fully responsive, mobile-first. Must look great at 375px and 1440px, no horizontal scroll.
- Fast and clean: no heavy images, no libraries, near-100 Lighthouse.
- Accessible: semantic HTML, strong contrast, alt text, keyboard navigable.

## Design direction (make it not look templated)
- Clean light theme, generous whitespace, one committed bold accent color (deep/electric blue, e.g. `#1A56DB` — pick one and use it consistently).
- Type: a strong modern sans for headings (Inter, Space Grotesk, or Sora) and a clean readable sans for body. Big confident headline.
- **Make the metrics the visual centerpiece.** Big numbers, short labels, in a callout strip.
- Subtle motion only: fade-in on scroll, clean hover states. Nothing gimmicky.
- Layout order: sticky minimal nav → bold hero → metric strip → about → track record → skills & tools → vendors/partners → contact footer.

## Sections & content

### Nav (sticky, minimal)
Wordmark "Fazil Rehman" on the left. Links: About, Track Record, Contact. A small **Download Resume** button on the right.

### Hero
- H1: Fazil Rehman
- Subhead: SMB Account Executive · SaaS & Technology Sales
- One-liner: Full-cycle SMB closer with 9+ years turning self-sourced pipeline into closed revenue.
- Two CTAs: **Get in touch** (mailto) and **Download resume** (links to the PDF).

### Metric strip (centerpiece)
Big-number callouts:
- **9+** — Years in sales
- **107%** — Of quota
- **$50K** — Top deal size
- **4,000+** — Vendor portfolio
(Optional 5th: **15%+** account expansion, or **Top 1%** rank.)

### About (2-3 short paragraphs, his voice, plain and direct)
Cover: who he is (SMB AE who self-sources and closes full-cycle), what he sells (cloud, security, software, co-sell across major vendors), how he sells (consultative, SPIN/Challenger), what he wants (a remote SaaS sales role where he runs the full cycle).

### Track record (skimmable cards or list — company, role, 1-2 metric lines each)
- **Softchoice** (Account Executive, SMB, current): 107% of quota · $500 to $50K deals · 4,000+ vendor co-sell · Google Champion.
- **Best Buy Canada** (Sales Project Specialist): $4M procurement portfolio · 23% cost reduction · $500K+ annual savings · 200+ store rollouts.
- **TTC** (Senior Client Relations Specialist): 75,000+ stakeholder book · led 50+ agents · 22% churn-risk reduction.
- **CIBC** (Digital Sales & Product): 60%+ upsell conversion · Simplii launch (44% engagement lift, 50K+ accounts).
- **GoodLife Fitness** (Membership Sales): 112% of quota · top 1% at club · 40% close rate.

### Skills & tools (two or three grouped lists)
- **Sales:** full-cycle SMB selling, self-sourced outbound, cold calling, SPIN, Challenger, consultative/solution selling, co-sell motions, new-logo acquisition, account expansion, forecasting.
- **Stack:** Salesforce, ZoomInfo, LinkedIn Sales Navigator, RingCentral, Power BI.
- **Certifications:** CSPO, CSM (Scrum Alliance).

### Vendors / partners
A simple styled row of vendor names he co-sells: Microsoft, Google, AWS, Cisco, Adobe, Sophos. Use text chips, **not** copyrighted logos.

### Contact / footer
- Email: fazilrehman@gmail.com (mailto link)
- LinkedIn: linkedin.com/in/fazilrehman
- Phone: (647) 469-6695 (optional)
- Location: Vancouver, BC · Open to Remote
- Download Resume button.

## Assets
- Resume PDF will be dropped next to `index.html` as `Fazil_Rehman_Resume.pdf`. Wire every "Download Resume" button to `./Fazil_Rehman_Resume.pdf`.
- No headshot required. Leave a clean spot for one if he later adds `headshot.jpg`.

## SEO / meta
- Title: `Fazil Rehman — SMB Account Executive | SaaS & Technology Sales`
- Meta description: `SMB Account Executive with 9+ years in SaaS and technology sales. Full-cycle closer, self-sourced pipeline, 107% of quota.`
- Add Open Graph tags for clean LinkedIn/Slack link previews. Favicon = simple "FR" monogram as inline SVG or data URI.

## Definition of done
- One `index.html`, opens directly in a browser with no server and no console errors.
- Responsive 375px to 1440px, no horizontal scroll.
- All links work: mailto, LinkedIn, resume download.
- Reads confident and clean, not like a default template.
- Folder is ready to drag straight into Netlify.

## Deployment
Netlify: drag the project folder into the Netlify dashboard, or run `netlify deploy --prod` from the folder. Custom domain optional later (e.g. fazilrehman.ca).
