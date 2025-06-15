# Deployment Instructions for Eco Stream Air Website

## Overview
This website has been converted from Microsoft Power Pages to a static HTML website ready for deployment on hosting.com.

## Files Structure
```
/
├── index.html          # Main website file
├── .htaccess          # Apache configuration for clean URLs and security
├── ESAS/              # Assets folder
│   ├── *.css          # Stylesheets
│   ├── *.png          # Images
│   ├── *.jpg          # Images
│   └── ...            # Other assets
└── DEPLOYMENT.md      # This file
```

## Deployment Steps

### 1. Upload Files via cPanel File Manager
1. Log into your hosting.com cPanel
2. Open File Manager
3. Navigate to your domain's public_html folder (usually `public_html/`)
4. Upload all files maintaining the folder structure:
   - Upload `index.html` to the root
   - Upload `.htaccess` to the root
   - Upload the entire `ESAS/` folder

### 2. Set Permissions (if needed)
- Files: 644
- Folders: 755
- The .htaccess file should be 644

### 3. Test the Website
- Visit www.ecostreamair.com
- Check that all images load properly
- Test the "Book a Consultation" buttons (should redirect to cal.com)
- Verify phone number displays correctly: (817)-470-0133

## Features Included
- ✅ Responsive design for mobile and desktop
- ✅ Clean URLs (no .html extension needed)
- ✅ Optimized images and CSS
- ✅ Security headers via .htaccess
- ✅ Browser caching for better performance
- ✅ Cal.com integration for appointments
- ✅ Professional HVAC company branding

## SSL Certificate
If you have an SSL certificate, uncomment these lines in .htaccess:
```apache
# RewriteCond %{HTTPS} off
# RewriteRule ^(.*)$ https://%{HTTP_HOST}%{REQUEST_URI} [L,R=301]
```

## Contact Information
- Phone: (817)-470-0133
- HVAC License: TACLA009556C
- Booking: https://cal.com/ecostream-air

## Troubleshooting
- If images don't load, check folder permissions and paths
- If .htaccess causes errors, temporarily rename it to debug
- Contact hosting.com support if you encounter server-specific issues