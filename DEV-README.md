# 🚀 Local Development Setup

## Quick Start

1. **Start Development Server:**
   ```bash
   npm run dev
   ```
   This will:
   - Launch the website at `http://localhost:3000`
   - Automatically open your browser
   - Auto-reload when you save changes to HTML/CSS files

2. **Alternative Start Command:**
   ```bash
   npm start
   ```

## Development Workflow

### Making Changes
1. Edit `index.html` for content changes
2. Edit CSS files in `ESAS/` folder for styling
3. Save your changes - the browser will automatically refresh!

### File Structure for Development
```
/
├── index.html              # 🎯 Main file - edit this for content
├── ESAS/
│   ├── theme.css          # 🎨 Main custom styles
│   ├── portalbasictheme.css # 🎨 Color theme variables
│   ├── bootstrap.min.css   # 📦 Bootstrap framework
│   └── *.png/*.jpg        # 🖼️ Images
├── package.json           # 📦 Development dependencies
└── DEV-README.md         # 📋 This file
```

## Common Development Tasks

### 🎨 Styling Changes
- **Colors:** Edit CSS custom properties in `ESAS/portalbasictheme.css`
- **Layout:** Edit inline styles in `index.html` or add new CSS to `ESAS/theme.css`
- **Typography:** Font changes in `index.html` or `ESAS/theme.css`

### 📝 Content Changes
- **Text:** Edit directly in `index.html`
- **Images:** Replace files in `ESAS/` folder (keep same filenames)
- **Links:** Update href attributes and onclick handlers

### 🔧 Advanced Customization
- **Add new sections:** Copy existing section structure in `index.html`
- **Responsive breakpoints:** Use Bootstrap classes or custom CSS media queries
- **Interactive elements:** Add JavaScript at the bottom of `index.html`

## Browser Testing

The development server works great with:
- Chrome (recommended for dev tools)
- Firefox
- Safari
- Edge

## Tips for UI Refinement

1. **Use Browser Dev Tools:**
   - Right-click → "Inspect Element"
   - Edit styles in real-time
   - Copy successful changes back to your files

2. **Test Mobile Views:**
   - Use browser dev tools device simulator
   - Try different screen sizes

3. **Color Palette Reference:**
   - Primary Green: `#219653`
   - Accent Yellow: `#FFCA4B`
   - Dark Text: `#32322C`
   - Light Background: `#F5F7FA`

## Deployment
When ready to deploy, upload these files to hosting.com:
- `index.html`
- `.htaccess`
- `ESAS/` folder (entire folder)

## Need Help?
Tell Claude what you want to change and I'll help you implement it step by step!