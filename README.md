# Michael Saber Portfolio

A clean, modern, and professional single-page CV website showcasing aviation and data analysis expertise.

## 🌟 Features

- **Responsive Design**: Mobile-first approach that looks great on all devices (phones, tablets, desktops)
- **Modern UI**: Professional color scheme with smooth animations and transitions
- **Easy Navigation**: Smooth scrolling between sections with fixed navigation bar
- **Sections Included**:
  - Hero/Header with professional title
  - About section with introduction
  - Work Experience with timeline layout
  - Skills showcase with categorized tags
  - Education and certifications
  - Contact information and social links
- **Interactive Elements**:
  - Hamburger menu for mobile devices
  - Scroll-to-top button
  - Hover effects and animations
  - Active navigation highlighting
- **SEO-Friendly**: Proper HTML structure with meta tags
- **Print-Friendly**: Optimized styling for printing/PDF generation
- **No Dependencies**: Pure HTML, CSS, and JavaScript (no frameworks required)

## 🚀 Quick Start

### View the Website Locally

1. Clone this repository:
   ```bash
   git clone https://github.com/teddybear787888-code/michaelsaber-portfolio.git
   cd michaelsaber-portfolio
   ```

2. Open `index.html` in your web browser:
   - **Option 1**: Double-click the `index.html` file
   - **Option 2**: Right-click and select "Open with" → your preferred browser
   - **Option 3**: Use a local server:
     ```bash
     # Python 3
     python -m http.server 8000
     
     # Python 2
     python -m SimpleHTTPServer 8000
     
     # Node.js (if you have http-server installed)
     npx http-server
     ```
   - Then visit `http://localhost:8000` in your browser

### Deploy to GitHub Pages

1. Go to your repository on GitHub
2. Click on **Settings** → **Pages** (in the left sidebar)
3. Under "Source", select **Deploy from a branch**
4. Select the branch (usually `main` or `master`) and folder (`/ (root)`)
5. Click **Save**
6. Your site will be published at: `https://teddybear787888-code.github.io/michaelsaber-portfolio/`

**Note**: It may take a few minutes for your site to be published.

## ✏️ Customization Guide

### 1. Personal Information

**File: `index.html`**

Update the following sections with your information:

#### Hero Section (Lines ~30-41)
```html
<h1 class="hero-title">Your Name</h1>
<p class="hero-subtitle">Your Professional Title</p>
<p class="hero-description">Your tagline or description</p>
```

#### About Section (Lines ~46-64)
Replace the placeholder text with your own introduction and professional summary.

#### Work Experience (Lines ~69-145)
- Modify existing timeline items or add/remove as needed
- Update job titles, company names, durations, and responsibilities
- Each experience is wrapped in a `<div class="timeline-item">` element

#### Skills Section (Lines ~150-199)
- Update skill categories and tags to match your expertise
- Add or remove skill categories as needed
- Edit individual skill tags within each category

#### Education Section (Lines ~204-250)
- Update degrees, institutions, years, and details
- Modify certifications to match your qualifications

#### Contact Information (Lines ~258-275)
```html
<a href="mailto:your.email@example.com">your.email@example.com</a>
<a href="https://linkedin.com/in/yourprofile">LinkedIn</a>
<a href="https://github.com/yourusername">GitHub</a>
```

### 2. Color Scheme

**File: `styles.css`** (Lines 1-20)

Customize the color scheme by modifying CSS variables:

```css
:root {
    --primary-color: #2563eb;      /* Main brand color */
    --primary-dark: #1e40af;       /* Darker shade */
    --primary-light: #3b82f6;      /* Lighter shade */
    --secondary-color: #64748b;    /* Secondary color */
    --accent-color: #0ea5e9;       /* Accent color */
    /* ... more variables ... */
}
```

### 3. Typography

**File: `styles.css`** (Lines 15-18)

Change fonts and sizes:

```css
:root {
    --font-primary: -apple-system, BlinkMacSystemFont, 'Segoe UI', ...;
    --font-size-base: 16px;
    --line-height-base: 1.6;
}
```

To use a custom font from Google Fonts:
1. Add this to the `<head>` section of `index.html`:
   ```html
   <link rel="preconnect" href="https://fonts.googleapis.com">
   <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&display=swap" rel="stylesheet">
   ```
2. Update the CSS variable:
   ```css
   --font-primary: 'Inter', sans-serif;
   ```

### 4. Sections

To add, remove, or reorder sections:

1. **HTML**: Add/remove section blocks in `index.html`
2. **Navigation**: Update the navigation menu to match your sections
3. **CSS**: Use existing section styles or create new ones

### 5. Social Media Icons

Replace emoji icons with actual icon libraries (optional):

1. Add Font Awesome to `index.html`:
   ```html
   <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
   ```

2. Replace emoji icons with Font Awesome classes:
   ```html
   <i class="fas fa-envelope"></i>  <!-- Email -->
   <i class="fab fa-linkedin"></i>  <!-- LinkedIn -->
   <i class="fab fa-github"></i>    <!-- GitHub -->
   ```

## 📁 File Structure

```
michaelsaber-portfolio/
│
├── index.html          # Main HTML file with content structure
├── styles.css          # All styling and responsive design
├── script.js           # Interactive features and smooth scrolling
└── README.md           # This file
```

## 🎨 Customization Tips

1. **Images**: To add a profile photo, add an `<img>` tag in the hero or about section
2. **Animations**: Adjust animation speeds in `styles.css` by changing `--transition-speed`
3. **Spacing**: Modify spacing variables in CSS for tighter/looser layouts
4. **Mobile Menu**: The hamburger menu automatically appears on screens < 768px wide

## 🔧 Technical Details

- **No Build Process**: Pure HTML/CSS/JS - no compilation or bundling needed
- **Browser Support**: Modern browsers (Chrome, Firefox, Safari, Edge)
- **Responsive Breakpoints**:
  - Desktop: > 768px
  - Tablet: 481px - 768px
  - Mobile: ≤ 480px
- **Accessibility**: Semantic HTML, ARIA labels, keyboard navigation support

## 📱 Testing Responsive Design

1. **Chrome DevTools**: Press F12 → Click device toolbar icon (or Ctrl+Shift+M)
2. **Firefox**: Press F12 → Click responsive design mode icon (or Ctrl+Shift+M)
3. **Safari**: Develop → Enter Responsive Design Mode

Test on various device sizes:
- iPhone SE (375px)
- iPhone 12 Pro (390px)
- iPad (768px)
- Desktop (1920px)

## 🖨️ Print/PDF Generation

The website includes print-friendly styles. To generate a PDF:

1. Open the website in a browser
2. Press Ctrl+P (Windows) or Cmd+P (Mac)
3. Select "Save as PDF" as the destination
4. Recommended settings:
   - Layout: Portrait
   - Margins: Default
   - Background graphics: Enabled (optional)

## 🐛 Troubleshooting

**Issue**: Smooth scrolling not working
- **Solution**: Ensure JavaScript is enabled in your browser

**Issue**: Mobile menu not appearing
- **Solution**: Check browser console for errors; verify `script.js` is loaded

**Issue**: Styles not loading
- **Solution**: Verify `styles.css` is in the same directory as `index.html`

**Issue**: GitHub Pages site not updating
- **Solution**: Wait 5-10 minutes; clear browser cache; check GitHub Actions tab for build status

## 🤝 Contributing

Feel free to fork this repository and customize it for your own use. If you find bugs or have suggestions, please open an issue.

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 👤 Contact

Michael Saber
- Email: michael.saber@email.com
- LinkedIn: [linkedin.com/in/michaelsaber](https://linkedin.com/in/michaelsaber)
- GitHub: [github.com/michaelsaber](https://github.com/michaelsaber)

---

**Built with ❤️ using pure HTML, CSS, and JavaScript**