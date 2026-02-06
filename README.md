# EmptyMiles Landing Page

A beautiful, responsive landing page for **emptymiles.in** with early access registration forms.

## Features

- ✅ Hero section with CTAs
- ✅ Problem explanation (why cabs are expensive)
- ✅ EmptyMiles vs Ola/Uber comparison
- ✅ How it works (Customer & Driver flows)
- ✅ Pricing transparency section
- ✅ Early access signup forms (Customer & Driver)
- ✅ FAQ accordion
- ✅ Responsive footer
- ✅ Success modal on signup
- ✅ Dark theme with green/yellow accents
- ✅ Mobile responsive
- ✅ Smooth scroll navigation

## How to View

Simply open `index.html` in any web browser:

```bash
# Windows
start index.html

# Mac
open index.html

# Linux
xdg-open index.html
```

## How to Deploy

### Option 1: Netlify (Free)

1. Go to [netlify.com](https://netlify.com)
2. Drag and drop the `website` folder
3. Done! Your site is live.

### Option 2: Vercel (Free)

1. Install Vercel CLI: `npm i -g vercel`
2. Run: `vercel --prod`
3. Follow prompts

### Option 3: GitHub Pages (Free)

1. Create a GitHub repo
2. Upload `index.html`
3. Go to Settings → Pages → Enable

### Option 4: Any Static Hosting

Upload `index.html` to any web hosting service.

## Connecting to Google Sheets (for signups)

To collect real signups, you can connect the forms to Google Sheets:

1. Create a Google Sheet
2. Use [Google Apps Script](https://script.google.com) to create a web app
3. Update the form submit handlers in `index.html`

Or use services like:
- [Formspree](https://formspree.io)
- [Netlify Forms](https://www.netlify.com/products/forms/)
- [Google Forms embed](https://forms.google.com)

## Customization

### Change Colors

Edit the Tailwind config in `<script>` tag:

```javascript
colors: {
    primary: { ... },    // Green tones
    secondary: { ... },  // Yellow tones
    dark: { ... },       // Background tones
}
```

### Change Content

All content is in the HTML file. Search for the text you want to change.

### Add Google Analytics

Add before `</head>`:

```html
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_MEASUREMENT_ID');
</script>
```

## Current Data Storage

Signups are currently stored in browser localStorage for demo purposes:
- `emptymiles_customers` - Customer waitlist
- `emptymiles_drivers` - Driver registrations

For production, connect to a real backend or Google Sheets.

## Files

```
website/
├── index.html      # Complete landing page
└── README.md       # This file
```

## Tech Used

- HTML5
- Tailwind CSS (via CDN)
- Vanilla JavaScript
- Google Fonts (Outfit)

---

Built for EmptyMiles.in 🚗
