# Nurikabe Islands Website

Static website for the Nurikabe Islands iOS app.

## Files

- `index.html` - Landing page
- `privacy.html` - Privacy Policy (required for App Store)
- `support.html` - Support page with FAQ
- `icon.png` - App icon

## Before Deploying

1. **Update the App Store link**: Replace `YOUR_APP_ID` in `index.html` with your actual App Store ID
2. **Update email**: Replace `support@nurikabeislands.com` with your actual support email
3. **Update domain**: If using a different domain, update all internal links

## Deployment Options

### Option 1: GitHub Pages (FREE - Recommended)

1. Create a new GitHub repository
2. Push these files to the repo
3. Go to Settings → Pages
4. Select "Deploy from a branch" → main → / (root)
5. Your site will be at `https://yourusername.github.io/repo-name`

To use a custom domain:
1. Add a `CNAME` file with your domain name
2. Configure your domain's DNS to point to GitHub

### Option 2: Netlify (FREE)

1. Go to [netlify.com](https://netlify.com)
2. Drag and drop this folder
3. Done! Get a free `.netlify.app` subdomain
4. Optional: Add custom domain in settings

### Option 3: AWS S3 + CloudFront (~$1/month)

1. Create S3 bucket with static website hosting
2. Upload files
3. Create CloudFront distribution
4. Point your domain to CloudFront

## Domain Suggestions

Cheap domain registrars:
- **Cloudflare** - At-cost pricing, great DNS
- **Porkbun** - Often cheapest
- **Namecheap** - Good first-year deals

Domain ideas:
- `nurikabeislands.com` (~$10/year)
- `nurikabe.app` (~$14/year)
- `nurikabe-game.com` (~$10/year)

## For App Store Connect

After deploying, use these URLs:

- **Support URL**: `https://yourdomain.com/support.html`
- **Privacy Policy URL**: `https://yourdomain.com/privacy.html`
- **Marketing URL**: `https://yourdomain.com` (optional)
