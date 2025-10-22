# Personal Portfolio Website

A modern, responsive personal portfolio website showcasing professional experience, skills, and achievements. Built with vanilla HTML, CSS, and JavaScript with a clean, minimalist design and dark mode support.

## Features

- **Responsive Design**: Fully responsive layout that works seamlessly on desktop, tablet, and mobile devices
- **Dark/Light Mode**: Toggle between dark and light themes with persistent preference storage
- **Dynamic Content**: All content loaded from a JSON file for easy updates without touching the code
- **Smooth Animations**: Elegant transitions and hover effects throughout the site
- **Accessibility**: Semantic HTML and ARIA labels for better accessibility
- **Fast Loading**: Minimal dependencies, optimized for quick load times
- **Modern UI**: Clean, professional design with contemporary styling

## Sections

1. **Home/Hero**: Introduction with profile picture and call-to-action buttons
2. **About**: Professional summary with key statistics and achievements
3. **Experience**: Detailed work history with responsibilities
4. **Skills**: Categorized technical and soft skills
5. **Education**: Academic background and certifications
6. **Contact**: Contact information and social media links

## Technologies Used

- **HTML5**: Semantic markup
- **CSS3**: Custom properties (CSS variables), Flexbox, Grid
- **JavaScript**: Vanilla JS for interactivity and dynamic content
- **Font Awesome**: Icons for social media and UI elements

## Project Structure

```
.
├── index.html          # Main HTML file
├── data.json          # Portfolio content and data
├── profile.jpg        # Profile picture
├── resume.pdf         # Downloadable resume
└── README.md          # This file
```

## Setup and Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/rohitsharma19/rohitsharma19.github.io.git
   cd rohitsharma19.github.io
   ```

2. **Update your information**:
   - Edit `data.json` with your personal information, experience, skills, etc.
   - Replace `profile.jpg` with your profile picture
   - Replace `resume.pdf` with your resume

3. **Deploy**:
   - **GitHub Pages**: Push to your `username.github.io` repository
   - **Other hosting**: Upload all files to your web hosting service

## Customizing Your Portfolio

### Updating Content

All content is managed through the `data.json` file. Simply update the JSON structure with your information:

```json
{
  "personal": {
    "name": "Your Name",
    "title": "Your Title",
    "tagline": "Your tagline",
    ...
  },
  "experience": [...],
  "skills": {...},
  ...
}
```

### Changing Colors

The site uses CSS custom properties for easy theming. Edit the `:root` and `[data-theme="dark"]` sections in the `<style>` tag within `index.html`:

```css
:root {
    --bg-primary: #ffffff;
    --accent: #3b82f6;
    ...
}
```

### Adding Sections

1. Add your section HTML in `index.html`
2. Add corresponding data to `data.json`
3. Update the JavaScript `populateData()` function to populate your new section

## Configuration

### Theme Toggle

The theme preference is stored in `localStorage` and persists across sessions. Users can toggle between light and dark modes using the moon/sun icon in the navigation.

### Responsive Breakpoints

- **Desktop**: > 768px
- **Mobile**: ≤ 768px

Adjust breakpoints in the media queries section of the CSS.

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## Performance

- No external CSS frameworks (Bootstrap, Tailwind, etc.)
- Minimal JavaScript
- Font Awesome loaded from CDN
- Images optimized for web
- Fast loading with no build process required

## Deployment

### GitHub Pages

1. Ensure your repository is named `username.github.io`
2. Push your code to the main/master branch
3. Your site will be available at `https://username.github.io`

### Custom Domain

To use a custom domain with GitHub Pages:

1. Add a `CNAME` file with your domain name
2. Configure DNS settings with your domain provider
3. Enable HTTPS in GitHub Pages settings

## Local Development

Since this is a static site, you can use any local server:

**Using Python**:
```bash
python -m http.server 8000
```

**Using Node.js**:
```bash
npx http-server
```

**Using VS Code**:
Install the "Live Server" extension and click "Go Live"

Visit `http://localhost:8000` (or appropriate port) in your browser.

## License

This project is open source and available for personal and commercial use.

## Credits

- Built with [Claude AI](https://claude.ai)
- Icons by [Font Awesome](https://fontawesome.com)

## Contact

For questions or feedback, reach out via:
- Email: rohitsharma19@gmail.com
- LinkedIn: [linkedin.com/in/rhtsh](https://www.linkedin.com/in/rhtsh)
- GitHub: [github.com/rohitsharma19](https://github.com/rohitsharma19)

---

Made with ❤️ using Claude AI
