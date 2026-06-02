# Fmsarp LLC — Business Website

Professional services site for Fmsarp LLC. Plain HTML/CSS/JS, hosted free on GitHub Pages.

## Pages
- `index.html` — Home (hero, services overview, process, why us, CTA)
- `services.html` — Detailed services + engagement models
- `about.html` — Company story, values, team
- `contact.html` — Contact form + details
- `css/style.css` — Shared styles (light corporate theme)
- `js/main.js` — Mobile menu + scroll animations

## IMPORTANT — Before going live

### 1. Make the contact form work
The form uses [Formspree](https://formspree.io) (free tier works on GitHub Pages):
1. Sign up at formspree.io with hello@fmsarp.com
2. Create a new form — it gives you an endpoint like `https://formspree.io/f/abcd1234`
3. In `contact.html`, find `action="https://formspree.io/f/YOUR_FORM_ID"` and replace `YOUR_FORM_ID` with your real ID

### 2. Update contact details
Search and replace across all files if these change:
- `hello@fmsarp.com` — your real email
- `github.com/fmsarp` — your real GitHub (or remove)

### 3. Replace the "Partner" placeholder
In `about.html`, the second team card is a placeholder for your business partner — add their real name, role, and bio.

## Deploy
This replaces your existing blog. To deploy over your current repo:
```bash
# in your repo folder, after copying these files in
git add .
git commit -m "Launch Fmsarp LLC business site"
git push
```
Live at fmsarp.com within ~60 seconds.

## Notes on winning contracts
To strengthen contract/RFP applications later, consider adding:
- A **portfolio / case studies** page once you have client work to show
- **Client testimonials** as you collect them
- A **capabilities statement** PDF (especially for government contracts — SAM.gov registration is required for US federal work)
- Specific **certifications** (Microsoft Partner, AWS pricing tier, etc.) as you earn them
