# Deployment Guide

## Pre-Deployment Checklist

1. **Add Founder Image**
   - Place the founder's professional photograph at: `/public/images/ca-sandeep-pachnanda-founder.jpg`
   - Recommended dimensions: 800x1000px (portrait orientation)
   - Format: JPG or PNG
   - Ensure the image is optimized for web (compressed but high quality)

2. **Update Domain Information**
   - Update `app/sitemap.ts` with your actual domain name
   - Update `public/robots.txt` with your actual domain
   - Update metadata in `app/layout.tsx` if needed

3. **Configure Contact Form**
   - Connect the contact form in `app/contact/page.tsx` to your email service or backend
   - Consider using services like:
     - EmailJS
     - Formspree
     - SendGrid
     - Your own backend API

4. **Google Maps Integration** (Optional)
   - Add Google Maps API key to `next.config.js` if you want to embed a map
   - Update the map placeholder in `app/contact/page.tsx`

5. **Environment Variables** (if needed)
   - Create a `.env.local` file for any API keys or sensitive information
   - Add `.env.local` to `.gitignore` (already included)

## Deployment Options

### Vercel (Recommended)

1. Push your code to GitHub
2. Import your repository to Vercel
3. Vercel will automatically detect Next.js and configure build settings
4. Add environment variables if needed
5. Deploy!

### Other Platforms

- **Netlify**: Similar to Vercel, supports Next.js out of the box
- **AWS Amplify**: Good for AWS ecosystem integration
- **Self-hosted**: Requires Node.js server setup

## Post-Deployment

1. **Test All Pages**
   - Verify all links work correctly
   - Test contact form submission
   - Check mobile responsiveness
   - Verify images load correctly

2. **SEO Setup**
   - Submit sitemap to Google Search Console
   - Verify robots.txt is accessible
   - Check meta tags with SEO tools

3. **Analytics** (Optional)
   - Add Google Analytics or similar
   - Track form submissions and key interactions

4. **Performance**
   - Run Lighthouse audit
   - Optimize images if needed
   - Enable Next.js Image Optimization

## Maintenance

- Regularly update blog content
- Keep dependencies updated
- Monitor form submissions
- Review and update legal pages as needed








