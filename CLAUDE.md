# Solana Health website: rules for Claude

This repository is the public website for Solana Health, an allied health clinic at Shop 1, 448 Bunnerong Road, Matraville NSW 2036, operated by ANJM Pty Ltd. Every change saved to the `main` branch publishes to solanahealth.com.au through Netlify.

Ange (Angelo Marketos, principal chiropractor) owns the business and approves every change.

## How to make a change

1. Never commit to `main` directly. Always work on a new branch.
2. Make the smallest change that does the job. Don't restyle, reorganise or rewrite pages that weren't part of the request.
3. Open a pull request with a plain-English summary: what changed, on which pages, and why.
4. Netlify builds a deploy preview for every pull request. Give Ange the preview link and ask him to check it on his phone.
5. Only merge after Ange has explicitly approved. If he asks for changes, update the same branch.
6. If something goes wrong after publishing, tell Ange straight away. Netlify can roll back to the previous version.

## Facts

- Never invent or guess fees, hours, services, practitioners, qualifications or statistics. If a fact isn't in the request or already on the site, ask.
- Keep name, address, phone and email identical everywhere. When any of these or the hours change, update every page, the footer, the JSON-LD structured data and `llms.txt` in the same pull request, then remind Ange to update the Google Business Profile and Cliniko the same day.
- Patient enquiries go to reception@solanahealth.com.au. Don't publish practitioners' own email addresses unless Ange asks.

## AHPRA advertising rules (non-negotiable)

Check every change against these before opening the pull request, and say in the pull request that you have.

- No testimonials, and no quoting or reposting reviews about treatment.
- No claims to cure or fix a condition, no guaranteed outcomes, and nothing that creates an unreasonable expectation of benefit.
- No before-and-after images that could mislead, and no AI-generated results imagery.
- No fear-based or scare messaging.
- Any offer or discount states its terms and conditions clearly.
- If "Dr" is used for a chiropractor, "Chiropractor" appears alongside it.
- No patient can be identified, directly or by inference.

Flag anything with a clinical claim so Ange can review that wording specifically. It is his AHPRA registration on the page.

## Privacy

- No patient information anywhere in this repository.
- No API keys, passwords or secrets in this repository. Ever.
- Don't add analytics, advertising pixels or other third-party scripts without Ange's approval, and never on booking or contact form pages.

## Brand

- Colours: Forest Green #224433 (headings, lettering, tagline), Terracotta #B27060 (logo mark and wordmark only), Warm Cream #FDFAF6 (background), Light Oak #EEDDBB (accent), Charcoal #555555 (secondary text).
- Fonts: Lora for headings, Poppins for body text.
- Tagline: "move well · recover faster", always lowercase with the interpunct, in Poppins and Forest Green. Never in the same lockup as "ALLIED HEALTH AND RECOVERY CLINIC".
- Use the shared stylesheet. Don't add one-off inline styles.

## Site structure

- Pages: home, `/chiropractor-matraville/`, `/dry-needling/`, `/physiotherapy-matraville/`, `/team/`, `/contact/`, `/faq/`, `/privacy-policy/`.
- `sitemap.xml`: update the `lastmod` date for any page you change. Add new pages to it.
- `_redirects`: don't change it unless asked. Old URLs depend on it.
- JSON-LD structured data: keep it valid and in step with the visible page content.
- Every image needs meaningful alt text.

## Writing style

- Australian English, plain and warm, written for local patients.
- No em dashes. Never use the word "ensure". Write "and", not "&".
- Short sentences. Explain what to expect rather than making promises.
