# Deployment Guide

This document provides detailed instructions for deploying the BCG Schedule Generator.

## Quick Deploy with Vercel (Recommended)

### 1. Prerequisites
- GitHub account
- Vercel account (sign up at vercel.com)

### 2. One-Click Deploy
1. Visit the repository: https://github.com/matt32l/bcg-scheduler
2. Click the "Deploy with Vercel" button
3. Follow the Vercel setup wizard

### 3. Custom Domain Setup
1. In Vercel dashboard → Project settings → Domains
2. Add your domain
3. Configure DNS:
   ```
   A Record:
   Name: @
   Value: 76.76.21.21

   CNAME Record:
   Name: www
   Value: cname.vercel-dns.com
   ```

## Manual Deployment

### Local Development
```bash
# Install dependencies
npm install

# Run development server
npm run dev

# Build for production
npm run build

# Start production server
npm start
```

### Environment Setup
Create `.env.local` file:
```
NEXT_PUBLIC_SITE_URL=https://your-domain.com
```

### Production Deployment Steps

1. Build the application:
```bash
npm run build
```

2. Test the production build:
```bash
npm start
```

3. Deploy to your hosting provider:
```bash
# Example for Vercel
vercel --prod
```

## Security Considerations

1. Enable HTTPS
2. Configure security headers:
   - CSP
   - HSTS
   - X-Frame-Options
   - X-Content-Type-Options

## Monitoring

1. Setup Vercel Analytics:
   - Enable in Vercel dashboard
   - Add analytics script to layout.tsx

2. Error tracking:
   - Configure Sentry or similar service
   - Monitor build logs

## Backup and Recovery

1. Database backups (if added later):
   - Schedule regular backups
   - Test restore procedures

2. Code backups:
   - GitHub repository
   - Local backups

## Troubleshooting

Common issues and solutions:

1. Build failures:
```bash
# Clear cache
rm -rf .next
npm run build
```

2. Deployment issues:
```bash
# Check logs
vercel logs
```

3. Performance issues:
   - Check Vercel Analytics
   - Run Lighthouse audits

## Maintenance

1. Regular updates:
```bash
# Check for updates
npm outdated

# Update packages
npm update
```

2. Security patches:
```bash
# Check for vulnerabilities
npm audit

# Fix vulnerabilities
npm audit fix
```

## Contact

For deployment support:
1. Open an issue on GitHub
2. Contact repository maintainers