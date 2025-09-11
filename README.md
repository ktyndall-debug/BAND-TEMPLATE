# Band Website Template

## 🎸 Modern, Edgy Band Website

A fully responsive, modern band website template with a dark, edgy design featuring neon accents and smooth animations.

## 📁 Project Structure

```
BAND TEMPLATE/
│
├── index.html       # Main HTML file with all sections
├── styles.css       # Complete styling with animations
├── script.js        # JavaScript for interactivity
└── README.md        # Documentation (this file)
```

## 🎨 Features

### Design
- **Dark, bold color palette** with black, deep reds, and neon accents
- **Glitch text effects** on the hero title
- **Smooth animations** and transitions throughout
- **Fully responsive** design for all devices
- **High-contrast** modern aesthetic

### Sections
1. **Home** - Hero section with video background and glitch effects
2. **About** - Band biography with stats
3. **Music** - Spotify embed and album showcase
4. **Videos** - YouTube/Vimeo embeds
5. **Tour** - Event calendar with ticket links
6. **Gallery** - Photo grid with lightbox
7. **Merch** - Product cards for merchandise
8. **Contact** - Booking form and social links

### Interactive Features
- Smooth scroll navigation
- Mobile-responsive menu
- Gallery lightbox
- Form validation
- Parallax scrolling effects
- Cart functionality for merch
- Social media integration
- Easter egg (Konami code)

## 🚀 Getting Started

### 1. Basic Setup
1. Open the project folder
2. Replace all `[BAND NAME]` placeholders with your actual band name
3. Update `[YOUR CITY]`, `[STATE]`, `[YEAR]`, and other placeholders
4. Add your actual content (bio, tour dates, etc.)

### 2. Adding Media

#### Background Video (Hero Section)
- Replace `placeholder-video.mp4` with your video file
- Recommended format: MP4, under 10MB
- Dimensions: 1920x1080 or higher

#### Images Needed
- `placeholder-band-photo.jpg` - Main band photo for About section
- `placeholder-album1.jpg`, `placeholder-album2.jpg`, `placeholder-album3.jpg` - Album artwork
- `placeholder-gallery1.jpg` through `placeholder-gallery6.jpg` - Performance photos
- `placeholder-merch1.jpg` through `placeholder-merch4.jpg` - Product images

#### Image Recommendations
- Format: JPG or WebP for photos, PNG for logos
- Optimize images for web (compress to reduce file size)
- Gallery images: 800x800px minimum
- Album art: 500x500px
- Merch photos: 400x400px

### 3. Music Integration

#### Spotify
1. Go to Spotify for Developers
2. Get your album/playlist embed code
3. Replace `[SPOTIFY_ALBUM_ID]` in the iframe src

#### Apple Music / Bandcamp
- Add respective embed codes in the Music section
- Follow similar iframe structure

### 4. Video Integration

#### YouTube
1. Get the video ID from your YouTube URL
2. Replace `[VIDEO_ID_1]` and `[VIDEO_ID_2]` in the iframe src

#### Vimeo
- Use Vimeo's embed code generator
- Replace the existing iframe with your Vimeo embed

### 5. Customization Guide

#### Colors (in styles.css)
```css
:root {
    --primary-black: #0a0a0a;      /* Main background */
    --deep-red: #8B0000;           /* Primary accent */
    --bright-red: #DC143C;         /* Hover states */
    --neon-red: #FF073A;           /* Neon effects */
    --neon-cyan: #00FFFF;          /* Glitch effect */
    --neon-pink: #FF1493;          /* Glitch effect */
}
```

#### Fonts
Currently using:
- Headers: 'Bebas Neue' (display font)
- Body: 'Barlow' (clean, modern)

To change fonts:
1. Update Google Fonts link in `index.html`
2. Update font variables in `styles.css`

#### Animation Speed
Adjust transition speeds in CSS:
```css
--transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
```

### 6. Form Setup

The contact form currently shows an alert. To make it functional:

#### Option 1: Formspree (Easy)
1. Sign up at formspree.io
2. Add to form tag: `action="https://formspree.io/f/YOUR_FORM_ID" method="POST"`
3. Remove the preventDefault in JavaScript

#### Option 2: Custom Backend
- Set up a server endpoint
- Update the form submission JavaScript
- Handle email sending on your server

### 7. Social Media Links

Update these in the Contact section:
```html
<a href="https://facebook.com/yourbandname">
<a href="https://instagram.com/yourbandname">
<a href="https://twitter.com/yourbandname">
<a href="https://youtube.com/yourbandname">
<a href="https://open.spotify.com/artist/yourartistid">
```

### 8. SEO Optimization

#### Meta Tags (in index.html)
- Update the description meta tag
- Add Open Graph tags for social sharing:
```html
<meta property="og:title" content="Band Name - Official Website">
<meta property="og:description" content="Your band description">
<meta property="og:image" content="path/to/share-image.jpg">
```

#### Structured Data
Add schema.org markup for better search results:
```html
<script type="application/ld+json">
{
  "@context": "http://schema.org",
  "@type": "MusicGroup",
  "name": "Your Band Name",
  "url": "https://yourbandwebsite.com",
  "genre": "Rock/Alternative"
}
</script>
```

### 9. Performance Tips

1. **Optimize Images**
   - Use WebP format when possible
   - Compress images (TinyPNG, ImageOptim)
   - Use lazy loading for gallery images

2. **Minimize CSS/JS**
   - Use minification tools for production
   - Consider using a CDN for libraries

3. **Video Optimization**
   - Keep hero video under 10MB
   - Consider using a video CDN
   - Provide poster image for mobile

### 10. Deployment

#### GitHub Pages (Free)
1. Create a GitHub repository
2. Upload all files
3. Enable GitHub Pages in settings
4. Your site will be at: `username.github.io/repository-name`

#### Netlify (Free tier available)
1. Sign up at netlify.com
2. Drag and drop your folder
3. Get instant deployment with HTTPS

#### Traditional Hosting
- Upload files via FTP
- Ensure index.html is in the root directory

## 🎉 Easter Egg

Try the Konami Code on the website:
↑ ↑ ↓ ↓ ← → ← → B A

## 📝 Placeholder Checklist

Replace these placeholders before launching:

- [ ] `[BAND NAME]` - Your band name
- [ ] `[YOUR CITY]` - Your city
- [ ] `[STATE]` - Your state
- [ ] `[YEAR]` - Year band formed
- [ ] `[INFLUENCES]` - Musical influences
- [ ] `[SPOTIFY_ALBUM_ID]` - Spotify album ID
- [ ] `[VIDEO_ID_1]`, `[VIDEO_ID_2]` - YouTube video IDs
- [ ] `placeholder-*.jpg` - All placeholder images
- [ ] `placeholder-video.mp4` - Hero background video
- [ ] `booking@[bandname].com` - Contact email
- [ ] Social media URLs
- [ ] Tour dates and venues
- [ ] Merch products and prices

## 🛠 Troubleshooting

### Mobile Menu Not Working
- Ensure JavaScript is enabled
- Check console for errors
- Verify script.js is linked properly

### Images Not Loading
- Check file paths (case-sensitive on some servers)
- Ensure images are in the same directory
- Verify file extensions match

### Animations Laggy
- Reduce animation complexity on mobile
- Optimize image sizes
- Consider reducing parallax effects

## 💡 Advanced Customization

### Adding New Sections
1. Add HTML section with unique ID
2. Add corresponding styles in CSS
3. Update navigation menu
4. Add smooth scroll functionality

### Custom Animations
- Modify keyframes in styles.css
- Adjust timing functions
- Add new animation classes

### Integration Ideas
- Add Instagram feed widget
- Integrate merchandise with Shopify
- Add mailing list signup (Mailchimp)
- Include blog section
- Add member profiles
- Create discography timeline

## 📧 Support

For questions or customization help:
- Check the code comments
- Test in different browsers
- Use browser developer tools
- Validate HTML/CSS online

## 📄 License

This template is free to use and modify for your band website. 
Rock on! 🤘

---

*Built with ❤️ for the underground music scene*