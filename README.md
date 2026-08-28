# Dezivia Atelier — Final Deploy Package

This package contains the multi-page Dezivia Atelier website, optimized hero images, all 10 featured project images, team images, pricing guides, Insights pages, contact forms and the Netlify email function.

## Deploy to Netlify
1. Upload this project to a GitHub repository.
2. Connect that repository to Netlify.
3. Deploy. No static build command is required.

## Contact and Join forms
The forms post to `/api/contact` and use Resend through the included Netlify Function.

In Netlify → Site configuration → Environment variables, add:
- `RESEND_API_KEY` — your Resend API key
- `CONTACT_TO` — `Contact@dezivia.in`
- `EMAIL_FROM` — a verified sender, for example `Dezivia Atelier <hello@dezivia.in>`

After those are added, Project enquiries and Join Dezivia submissions are delivered separately to the official contact mailbox, with the visitor's email set as Reply-To.

## One media file to place
The current workspace did not contain the actual showreel video file itself, so the showreel section is already wired and uses a poster fallback. Put the final video here before deployment:

`assets/showreel/dezivia-showreel.mp4`

## Noir Bold
If you own/use a webfont version of Noir Bold, place it here:

`assets/fonts/Noir-Bold.woff2`

The CSS is already wired for it. Until the font file is present, the hero uses the included heavy fallback.

## Social links
Instagram, Behance, email and WhatsApp are wired. Replace the temporary LinkedIn/YouTube URLs when those official profiles are ready.
