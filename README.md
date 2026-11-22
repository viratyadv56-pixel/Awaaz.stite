# Awaaz AI — Render-ready static website

This project is a static HTML website. It does not require a Node.js server, build framework, or backend.

## Deploy with Render Blueprint (recommended)
1. Upload the contents of this folder to a GitHub repository (the `render.yaml` file must be at the repository root).
2. In Render, select **New + → Blueprint**.
3. Connect the GitHub repository and select **Apply**.
4. Render reads `render.yaml` and publishes the `public/` folder.

## Deploy as a Static Site (manual)
- **New:** Static Site
- **Repository:** your GitHub repository
- **Branch:** `main` (or the branch you use)
- **Root Directory:** leave blank
- **Build Command:** `echo "No build needed"` (or leave blank if Render permits)
- **Publish Directory:** `public`

## Before publishing
- The WhatsApp contact number is currently set in `public/index.html` as `WHATSAPP_NUMBER='918384059345'`.
- Replace it with your own WhatsApp Business number using country code and digits only, with no `+`, spaces, or hyphens.
- The contact form opens WhatsApp with a prefilled message. It does not store enquiries in a database or send them to an email inbox.
- Test the site on mobile and desktop, and submit a test enquiry to confirm the WhatsApp number is correct.

## Changes in this revision
- Fixed the missing scroll-progress element that caused a JavaScript error and prevented later animations from running.
- Added a scroll-progress indicator, safer animation initialization, mobile Indian-number validation, and reduced-motion accessibility handling.
- Added security response headers in the Render Blueprint configuration.
