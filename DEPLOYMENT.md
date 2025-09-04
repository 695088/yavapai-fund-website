# Yavapai Fund Website - Deployment Guide

## Overview
This guide explains how to deploy the Yavapai Fund website to various hosting platforms. The website has been restructured from a single-page scrolling design to a multi-page structure with the following pages:
- `index.html` - Homepage
- `about.html` - About page
- `services.html` - Services page
- `portfolio.html` - Portfolio page
- `contact.html` - Contact page

## File Structure
```
yavapai-fund-website/
├── index.html          # Homepage
├── about.html          # About page
├── services.html       # Services page
├── portfolio.html      # Portfolio page
├── contact.html        # Contact page
├── styles.css          # Main stylesheet
├── script.js           # JavaScript functionality
├── favicon.ico         # Website icon
├── package.json        # Dependencies (if using Node.js)
└── README.md           # Project documentation
```

## Color Palette
The website uses the following color scheme:
- Primary Blue: #0047AB
- Light Blue: #BFD1E5
- Bright Blue: #0066FF
- Dark Blue: #002F6C
- White: #FFFFFF
- Light Gray: #F8F9FA

## Hosting Options

### 1. GitHub Pages (Free)
**Best for:** Simple static hosting, portfolios, small businesses

**Steps:**
1. Create a GitHub repository named `yavapai-fund-website`
2. Upload all website files to the repository
3. Go to Settings > Pages
4. Select source branch (usually `main` or `master`)
5. Your site will be available at `https://username.github.io/yavapai-fund-website`

**Pros:** Free, easy to set up, automatic updates
**Cons:** Limited features, GitHub branding

### 2. Netlify (Free Tier)
**Best for:** Professional websites, custom domains, forms

**Steps:**
1. Sign up at [netlify.com](https://netlify.com)
2. Drag and drop your website folder to deploy
3. Or connect your GitHub repository for automatic deployments
4. Customize your domain or use the provided Netlify subdomain

**Pros:** Free tier, custom domains, form handling, CDN
**Cons:** Limited bandwidth on free tier

### 3. Vercel (Free Tier)
**Best for:** Modern web apps, fast performance

**Steps:**
1. Sign up at [vercel.com](https://vercel.com)
2. Import your GitHub repository
3. Deploy automatically on every push
4. Get a custom Vercel domain

**Pros:** Excellent performance, automatic deployments, edge network
**Cons:** Free tier limitations

### 4. Traditional Web Hosting
**Best for:** Full control, databases, server-side features

**Popular providers:**
- Bluehost
- HostGator
- SiteGround
- DreamHost

**Steps:**
1. Purchase hosting plan
2. Upload files via FTP/SFTP
3. Configure domain DNS
4. Set up SSL certificate

## Domain Configuration

### Custom Domain Setup
1. Purchase domain from registrar (GoDaddy, Namecheap, etc.)
2. Point DNS to your hosting provider
3. Configure SSL certificate (usually automatic with modern hosts)

### DNS Records
```
Type    Name    Value
A       @       [Your hosting IP]
CNAME   www     [Your domain]
```

## SSL/HTTPS Setup
- Most modern hosting providers offer free SSL certificates
- Let's Encrypt provides free SSL certificates
- Ensure all internal links use HTTPS

## Performance Optimization

### Before Deployment
1. **Minify CSS and JavaScript** (optional)
2. **Optimize images** (compress, use WebP format)
3. **Enable GZIP compression** on server
4. **Set up browser caching**

### CDN Setup
- Cloudflare (free tier available)
- AWS CloudFront
- Google Cloud CDN

## Maintenance

### Regular Updates
1. **Content updates** - Edit HTML files directly
2. **Style changes** - Modify `styles.css`
3. **Functionality** - Update `script.js`

### Backup Strategy
1. **Version control** - Use Git for code changes
2. **File backups** - Regular backups of all files
3. **Database backups** - If using databases

## Troubleshooting

### Common Issues
1. **404 errors** - Check file paths and navigation links
2. **Styling issues** - Verify CSS file paths
3. **JavaScript errors** - Check browser console
4. **Mobile responsiveness** - Test on various devices

### Debug Tools
- Browser Developer Tools
- W3C Validator
- Google PageSpeed Insights
- GTmetrix

## Security Considerations

### Basic Security
1. **HTTPS only** - Redirect HTTP to HTTPS
2. **Security headers** - Implement CSP, HSTS
3. **Form validation** - Client and server-side validation
4. **Regular updates** - Keep dependencies updated

### Advanced Security
1. **WAF (Web Application Firewall)**
2. **DDoS protection**
3. **Malware scanning**
4. **Security monitoring**

## Analytics and Monitoring

### Google Analytics
1. Create Google Analytics account
2. Add tracking code to all pages
3. Set up goals and conversions

### Other Tools
- Google Search Console
- Bing Webmaster Tools
- Uptime monitoring services

## Support and Resources

### Documentation
- [MDN Web Docs](https://developer.mozilla.org/)
- [W3Schools](https://www.w3schools.com/)
- [CSS-Tricks](https://css-tricks.com/)

### Community
- Stack Overflow
- Reddit webdev community
- Web development forums

## Contact Information
For technical support or questions about the website:
- Email: [Your email]
- Phone: [Your phone]
- Website: [Your website]

---

**Last Updated:** December 2024
**Version:** 2.0 (Multi-page structure)
