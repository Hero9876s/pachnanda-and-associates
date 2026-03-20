# Quick Start Guide

## Installation

1. **Install Dependencies**
   ```bash
   npm install
   ```

2. **Add Founder Image**
   - Place your founder's professional photograph at:
     `/public/images/ca-sandeep-pachnanda-founder.jpg`
   - Recommended: 800x1000px, JPG format, optimized for web

3. **Run Development Server**
   ```bash
   npm run dev
   ```
   - Open [http://localhost:3000](http://localhost:3000) in your browser

## Project Structure

```
├── app/                    # Next.js App Router pages
│   ├── about/             # About Us page
│   ├── blog/              # Blog structure
│   ├── contact/           # Contact page with form
│   ├── consultation/      # Consultation page
│   ├── our-story/         # Our Story page
│   ├── services/          # Services page
│   ├── why-trust-us/      # Why Trust Us page
│   ├── privacy-policy/    # Privacy Policy
│   ├── terms-conditions/  # Terms & Conditions
│   ├── disclaimer/        # Professional Disclaimer
│   ├── layout.tsx         # Root layout
│   ├── page.tsx           # Home page
│   └── globals.css        # Global styles
├── components/            # Reusable React components
│   ├── Header.tsx         # Navigation header
│   ├── Footer.tsx         # Footer component
│   ├── CTASection.tsx     # Call-to-action sections
│   ├── TrustMetrics.tsx   # Trust metrics display
│   ├── FounderImage.tsx   # Founder image component
│   ├── Testimonials.tsx   # Testimonials section
│   └── StickyContactButtons.tsx # Sticky contact buttons
└── public/               # Static assets
    └── images/           # Image files
```

## Key Features

✅ **Responsive Design** - Works on all devices  
✅ **SEO Optimized** - Meta tags, sitemap, robots.txt  
✅ **Professional UI** - Corporate, elegant design  
✅ **Fast Loading** - Optimized images and code  
✅ **Accessible** - Follows web accessibility standards  
✅ **ICAI Compliant** - Professional decorum maintained  

## Customization

### Update Contact Information
- Edit contact details in:
  - `components/Footer.tsx`
  - `components/StickyContactButtons.tsx`
  - `app/contact/page.tsx`

### Update Colors
- Edit `tailwind.config.js` to change the color scheme
- Primary color is defined as `corporate-blue`

### Add Blog Articles
- Create markdown files or pages in `app/blog/`
- Update blog structure as needed

### Connect Contact Form
- Update `app/contact/page.tsx` form submission handler
- Connect to your email service or backend API

## Build for Production

```bash
npm run build
npm start
```

## Need Help?

- Check `DEPLOYMENT.md` for deployment instructions
- Review `README.md` for general information
- Ensure all dependencies are installed correctly








