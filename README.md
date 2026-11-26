# Nature With Riaz | RK Production

A responsive React and Vite portfolio for Nature With Riaz and RK Production. The site includes a cinematic landing page, creator introduction, filterable photo gallery with keyboard-accessible lightbox, YouTube video modal, production services, WhatsApp booking form, social links, and contact details.

## Run locally

```bash
npm install
npm run dev
```

Create a production build with `npm run build`, then preview it using `npm run preview`.

## Personalize the website

- **Contact details and social accounts:** edit `src/data/site.js`. Replace the WhatsApp number with digits only and include the country code (for example `923001234567`).
- **Gallery, videos, and services:** edit the arrays in `src/data/site.js`. Gallery items use Unsplash photo IDs; replace them with your own Unsplash IDs or update `imageUrl` to use your preferred image hosting. Video entries use YouTube video IDs.
- **Profile image:** replace `src/assets/images/riaz-portrait.png` with your own photo.
- **Brand logo and browser icon:** replace `public/rk-production-logo.png` with your preferred logo; it is used in the header, footer, 404 page, and browser tab.
- **Branding and page metadata:** edit `index.html` and the favicon at `public/favicon.svg`.

The booking form validates its required fields and opens WhatsApp with a prefilled message. It does not store or transmit form data to a server. The contact links and YouTube/social URLs are examples and should be updated with verified accounts before publishing.

## Deploy to Vercel

1. Push the project to a GitHub repository.
2. In Vercel, choose **Add New → Project** and import the repository.
3. Keep the detected Vite settings: build command `npm run build`, output directory `dist`.
4. Deploy. No environment variables are needed for the static site.

## GitHub setup

```bash
git init
git add .
git commit -m "Build Nature With Riaz portfolio"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git
git push -u origin main
```
