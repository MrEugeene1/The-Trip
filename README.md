# The Trip ✈️

A personal travel journal website showcasing journeys through France with friends—exploring Paris, Lille, and Marseille through immersive storytelling, photography, and cultural experiences.

## 🌍 Overview

"The Trip" is a static website that documents unforgettable travel experiences across three iconic French cities. Built with vanilla HTML, CSS, and JavaScript, the site features an interactive image slideshow, responsive design, and rich multimedia content that brings travel memories to life.

## ✨ Features

- **🎞️ Interactive Slideshow**: Auto-advancing image carousel with manual controls and dot navigation showcasing 15 travel photos
- **📱 Responsive Design**: Mobile-first approach ensuring optimal viewing across all devices
- **🗺️ City Pages**: Dedicated pages for Paris, Lille, and Marseille with detailed travel stories
- **📸 Photo Gallery**: Curated collection of travel photography with descriptive captions
- **📬 Newsletter Subscription**: Custom-styled subscription form for travel updates
- **✉️ Contact Form**: Get-in-touch page for visitor engagement
- **🎨 Custom Styling**: Cohesive design with gradient backgrounds, smooth transitions, and modern UI elements

## 📂 Project Structure

```
The Trip/
├── index.html              # Main landing page with slideshow
├── Paris.html              # Paris travel journal
├── Lille.html              # Lille travel journal
├── Marseille.html          # Marseille travel journal
├── contact.html            # Contact form page
├── Subscribe_Pages.html    # Newsletter subscription page
├── style.css               # Global stylesheet
├── script.js               # Slideshow functionality
├── Assets/
│   ├── Sliding_images/     # Slideshow images (Paris, Lille, Marseille)
│   ├── Pages_images/       # City-specific gallery images
│   ├── Main_Page_Favicon/  # Main page icons
│   ├── Paris_Favicon/      # Paris page icons
│   ├── Lille_Favicon/      # Lille page icons
│   └── Marseille_Favicon/  # Marseille page icons
└── README.md
```

## 🚀 Getting Started

### Prerequisites

- Modern web browser (Chrome, Firefox, Safari, Edge)
- Local web server (optional but recommended)

### Installation & Running

1. **Clone or download the repository**
   ```bash
   git clone https://github.com/yourusername/The-Trip.git
   cd "The Trip"
   ```

2. **Open with Live Server (VS Code)**
   - Install the "Live Server" extension (`ritwickdey.LiveServer`)
   - Right-click `index.html` → "Open with Live Server"
   - Website opens at `http://127.0.0.1:5500`

3. **Or open directly in browser**
   - Navigate to the project folder
   - Double-click `index.html`
   - ⚠️ Some features may require a local server

## 🎨 Design Features

### Slideshow Component
- **Auto-advance**: Images change every 4 seconds
- **Manual controls**: Previous/Next arrow buttons
- **Dot navigation**: Click specific dots to jump to images
- **Fade transitions**: Smooth 1.5s fade animation
- **Responsive captions**: Dynamic text overlays on images

### Responsive Breakpoints
```css
/* Mobile devices */
@media screen and (max-width: 768px) {
  - Reduced slideshow height (600px → 400px)
  - Smaller navigation elements
  - Adjusted typography
}
```

### Color Scheme
- **Primary Blue**: `#005A9C` (headers, buttons)
- **Gradient Purple**: `linear-gradient(135deg, #667eea 0%, #764ba2 100%)`
- **Text**: `#333` on light backgrounds
- **Backgrounds**: `#f4f4f4` (light gray)

## 🛠️ Technology Stack

- **HTML5**: Semantic markup, accessible forms
- **CSS3**: Flexbox, Grid, animations, custom properties
- **Vanilla JavaScript**: DOM manipulation, event handling
- **No frameworks or libraries** - Pure web fundamentals

## 📄 Page Descriptions

### 🏠 Home Page (`index.html`)
- Hero header with travel philosophy
- 15-image rotating slideshow (5 images per city)
- Photo gallery with 10 curated images
- Navigation to all site sections

### 🗼 Paris Page (`Paris.html`)
- Eiffel Tower and Louvre experiences
- French culinary journey (croissants, bistros)
- Cultural highlights (Musée d'Orsay, street art)
- Personal reflections and transformative moments
- Embedded YouTube video content

### 🏛️ Lille Page (`Lille.html`)
- Flemish-French architectural fusion
- Palais des Beaux-Arts art collection
- Traditional waffle and moules-frites cuisine
- Braderie de Lille flea market experience
- Hidden courtyard discoveries

### ⛵ Marseille Page (`Marseille.html`)
- Notre-Dame de la Garde basilica
- Le Panier district street art
- Authentic bouillabaisse and Mediterranean cuisine
- Calanques National Park hiking
- Multicultural market experiences

### 📬 Subscribe Page (`Subscribe_Pages.html`)
- Modern gradient design
- Email capture form
- Consent checkbox for GDPR compliance
- Smooth hover effects and transitions

### ✉️ Contact Page (`contact.html`)
- Name, email, subject, message fields
- Form validation
- Accessible labels and inputs

## 🎯 Key JavaScript Functionality

### Slideshow Logic (`script.js`)
```javascript
// Auto-advance every 4 seconds
function startAutoSlide() {
    slideTimer = setTimeout(function() {
        slideIndex++;
        showSlides(slideIndex);
        startAutoSlide();
    }, 4000);
}

// Manual navigation resets timer
function changeSlide(n) {
    clearTimeout(slideTimer);
    showSlides(slideIndex += n);
    startAutoSlide();
}
```

## 🌐 Browser Support

- ✅ Chrome 90+
- ✅ Firefox 88+
- ✅ Safari 14+
- ✅ Edge 90+

## 🔜 Future Enhancements

- [ ] **Azure Cosmos DB Integration**: Store travel stories and user comments
  - User-generated content collection (reviews, tips)
  - Real-time collaboration features for trip planning
  - Global distribution for low-latency access
- [ ] **Backend API**: Node.js/Express for form submissions
- [ ] **Dark Mode**: Toggle for night viewing
- [ ] **Search Functionality**: Filter gallery by city/tag
- [ ] **Social Sharing**: Share individual stories on social media
- [ ] **Map Integration**: Interactive map showing travel routes

## 🔒 Form Handling

Currently, forms use placeholder actions:
```html
<form action="/submit-contact" method="post">
<form action="/subscribe" method="post">
```

**To make functional:**
1. Set up a backend server (Node.js, Python Flask, etc.)
2. Create API endpoints for `/submit-contact` and `/subscribe`
3. Implement email service (SendGrid, Mailchimp)
4. Add CSRF protection and input sanitization

## 📸 Image Attribution

All images in the `Assets/` folder are personal travel photographs. If using this template:
- Replace images with your own content
- Ensure proper licensing for any third-party images
- Update `alt` text to match your images

## 🤝 Contributing

This is a personal project, but suggestions are welcome!

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-idea`)
3. Commit changes (`git commit -m 'Add amazing idea'`)
4. Push to branch (`git push origin feature/amazing-idea`)
5. Open a Pull Request

## 📜 License

This project is open source and available under the [MIT License](LICENSE).

## 👤 Author

**Your Name**
- 📧 Email: eookyere4@gmail.com
- 📷 Instagram: [@mr_eugeene](https://www.instagram.com/mr_eugeene/)

## 🙏 Acknowledgments

- Travel companions who made these journeys unforgettable
- The cities of Paris, Lille, and Marseille for their inspiration
- The web development community for best practices and guidance

---

**"Paris is always a good idea." - Audrey Hepburn** 💛✨

*Built with ❤️ and wanderlust | Last updated: February 2026*

