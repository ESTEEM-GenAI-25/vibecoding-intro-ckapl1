# Chris Kaplan's Personal Website

A clean, responsive personal website built with vanilla HTML, CSS, and JavaScript. Features dynamic content loading, light/dark theme toggle, and mobile-responsive design.

## 🚀 Live Site

This site is designed to work on GitHub Pages. Simply push to the main branch and enable GitHub Pages in your repository settings.

## 📁 File Structure

```
/
├── index.html          # Homepage
├── about.html          # About page
├── projects.html       # Projects page
├── 404.html           # Custom 404 page
├── assets/
│   ├── styles.css     # All styling and theme support
│   └── site-copy.json # All website content (edit this!)
├── PRD.md             # Product Requirements Document
└── README.md          # This file
```

## ✏️ How to Edit Content

**All website text is stored in one file for easy editing:**

### 1. Edit `assets/site-copy.json`

This is the **only file you need to edit** to update all website content:

```json
{
  "site": {
    "name": "Chris Kaplan",
    "title": "Master's Student in ESTEEM Program at University of Notre Dame",
    "email": "ckaplan@nd.edu",
    "linkedin": "https://www.linkedin.com/in/christopherkaplanr/",
    "resume": "resume.pdf"
  },
  "home": {
    "greeting": "Hello, I'm",
    "description": "A master's student in the ESTEEM program at the University of Notre Dame with a background in finance and entrepreneurship. I am passionate about startups, innovation, and helping others learn personal finance and investing.",
    "cta": "Get in touch to learn more about my work and academic journey."
  },
  "about": {
    "bio": "Chris Kaplan is a master's student in the ESTEEM program at the University of Notre Dame with a background in finance and entrepreneurship. He is passionate about startups, innovation, and helping others learn personal finance and investing.",
    "education": {
      "items": [
        {
          "degree": "Master's in ESTEEM Program",
          "institution": "University of Notre Dame",
          "status": "In Progress"
        }
      ]
    },
    "background": {
      "items": [
        "Finance",
        "Entrepreneurship",
        "Startups",
        "Innovation",
        "Personal Finance Education"
      ]
    }
  },
  "projects": {
    "items": [
      {
        "title": "ESTEEM Program Projects",
        "description": "Various projects and coursework as part of the ESTEEM program at Notre Dame, focusing on entrepreneurship and innovation.",
        "status": "In Progress",
        "technologies": ["Entrepreneurship", "Innovation", "Project Management"]
      }
    ]
  }
}
```

### 2. Add Your Resume

1. Add your resume PDF to the root directory
2. Update the `"resume"` field in `site-copy.json` to match your filename

### 3. Customize Colors (Optional)

Edit CSS variables in `assets/styles.css`:

```css
:root {
  --accent-color: #0d6efd;  /* Change this to your preferred color */
  --bg-primary: #ffffff;    /* Light theme background */
  --text-primary: #212529;  /* Light theme text */
}
```

## 🎨 Features

- ✅ **Responsive Design** - Works on all devices
- ✅ **Light/Dark Theme** - Toggle in top-right corner
- ✅ **Dynamic Content** - All text loads from JSON
- ✅ **Fast Loading** - No build process, pure static files
- ✅ **GitHub Pages Ready** - Works directly from main branch
- ✅ **Accessible** - Screen reader friendly, keyboard navigation
- ✅ **SEO Optimized** - Proper meta tags and structure

## 🛠️ Technical Details

- **No Build Process** - Pure HTML/CSS/JavaScript
- **No Dependencies** - Everything is self-contained
- **Modern CSS** - Uses CSS Grid, Flexbox, and custom properties
- **ES6 JavaScript** - Modern JavaScript with classes and async/await
- **Progressive Enhancement** - Works without JavaScript (content still loads)

## 📱 Mobile Support

The site is fully responsive with:
- Mobile-first CSS design
- Collapsible navigation menu
- Touch-friendly buttons and links
- Optimized typography for small screens

## 🌙 Theme System

The theme toggle:
- Remembers your preference in localStorage
- Smooth transitions between themes
- Accessible with keyboard navigation
- Works across all pages

## 🚀 Deployment

### GitHub Pages (Recommended)

1. Push all files to your repository's main branch
2. Go to Settings → Pages
3. Select "Deploy from a branch" → "main"
4. Your site will be live at `https://yourusername.github.io/repository-name`

### Other Hosting

This site works on any static hosting service:
- Netlify
- Vercel
- AWS S3
- Any web server

## 🔧 Customization

### Adding New Pages

1. Create new HTML file (e.g., `contact.html`)
2. Copy structure from existing pages
3. Add navigation link to all pages
4. Add content to `site-copy.json`

### Changing Layout

Edit `assets/styles.css`:
- Modify grid layouts in `.about-content` and `.projects-grid`
- Adjust spacing with margin/padding variables
- Change typography in the base styles

### Adding Features

The JavaScript is modular:
- `ThemeManager` - Handles theme switching
- `ContentManager` - Loads and renders content
- `MobileNav` - Mobile navigation functionality

## 📞 Support

If you need help customizing the site:

1. Check the `assets/site-copy.json` file first
2. Look at the CSS variables in `assets/styles.css`
3. The JavaScript is well-commented for easy modification

## 📄 License

This project is open source and available under the MIT License.

---

**Happy editing!** 🎉