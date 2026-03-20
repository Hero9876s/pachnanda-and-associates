# Pachnanda and Associates - Professional CA Firm Website

A professional, trust-driven, production-ready website for Pachnanda and Associates, a Chartered Accountant firm based in Jammu, Jammu & Kashmir.

## 🎯 Features

- ✅ Professional corporate design following ICAI decorum
- ✅ Fully responsive and mobile-optimized
- ✅ SEO-friendly structure with sitemap and robots.txt
- ✅ Fast loading and production-ready
- ✅ Multiple service pages and consultation forms
- ✅ Trust metrics and testimonials
- ✅ Sticky contact buttons (Call & WhatsApp)
- ✅ Comprehensive legal pages (Privacy, Terms, Disclaimer)
- ✅ Blog structure ready for content
- ✅ Accessible and well-commented code

## 🛠 Tech Stack

- **Next.js 14** (App Router) - React framework
- **TypeScript** - Type-safe development
- **Tailwind CSS** - Utility-first CSS framework
- **React Icons** - Icon library

## 📁 Project Structure

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
│   └── ...
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

## 🚀 Getting Started

### Prerequisites

- Node.js 18+ installed
- npm or yarn package manager

### Installation

1. **Install dependencies:**
   ```bash
   npm install
   ```

2. **Add Founder Image:**
   - Place the founder's professional photograph at:
     `/public/images/ca-sandeep-pachnanda-founder.jpg`
   - Recommended: 800x1000px, JPG format, optimized for web

3. **Run the development server:**
   ```bash
   npm run dev
   ```

4. **Open your browser:**
   - Navigate to [http://localhost:3000](http://localhost:3000)

## 📄 Pages Included

1. **Home** - Hero section, trust metrics, services preview, testimonials
2. **About Us** - Founder introduction and qualifications
3. **Our Story** - Firm history and journey
4. **Services** - Comprehensive service offerings
5. **Why Trust Us** - Trust-building content and metrics
6. **Consultation** - Free consultation information
7. **Contact** - Contact form and office details
8. **Blog** - Blog structure (ready for content)
9. **Legal Pages** - Privacy Policy, Terms & Conditions, Disclaimer

## 🎨 Customization

### Update Contact Information
Edit contact details in:
- `components/Footer.tsx`
- `components/StickyContactButtons.tsx`
- `app/contact/page.tsx`

### Update Colors
Edit `tailwind.config.js` to change the color scheme. The primary corporate blue is defined as `corporate-blue`.

### Connect Contact Form
Update the form submission handler in `app/contact/page.tsx` to connect to your email service or backend API.

## 🏗 Build for Production

```bash
npm run build
npm start
```

## 📦 Deployment

See `DEPLOYMENT.md` for detailed deployment instructions.

### Quick Deploy to Vercel

1. Push code to GitHub
2. Import repository to [Vercel](https://vercel.com)
3. Deploy automatically

## 📝 Important Notes

- **Founder Image**: Must be placed at `/public/images/ca-sandeep-pachnanda-founder.jpg`
- **Contact Form**: Connect to your email service or backend (see `app/contact/page.tsx`)
- **Domain**: Update sitemap and robots.txt with your actual domain
- **Google Maps**: Optional - add API key if you want embedded maps

## 📚 Documentation

- `QUICK_START.md` - Quick setup guide
- `DEPLOYMENT.md` - Detailed deployment instructions
- Code is well-commented for easy maintenance

## 🔒 Compliance

- Follows ICAI professional decorum
- Includes professional disclaimer
- Privacy policy and terms included
- Accessible design standards

## 📞 Support

For questions or issues, refer to the documentation files or contact the development team.

---

**Built with ❤️ for Pachnanda and Associates**

