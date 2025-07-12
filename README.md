# Alternative Counselling Services Website

A static website for Alternative Counselling Services, providing trauma-informed online counselling services across Australia.

## Deployment Instructions

### S3 Deployment
1. Create an S3 bucket with static website hosting enabled
2. Set bucket policy to allow public read access
3. Upload all files maintaining the directory structure
4. Configure index document as `index.html`
5. Enable CORS if needed for Formspree integration

### Formspree Setup
1. Create a Formspree account
2. Create a new form for the contact page
3. Replace the form action URL in `contact.html` with your Formspree form ID
4. Test form submission in development before deployment

## File Structure
```
.
├── index.html
├── about.html
├── services.html
├── resources.html
├── contact.html
├── assets/
│   ├── css/
│   │   └── style.css
│   └── img/
│       ├── dragonfly.svg
│       └── hero-*.jpg
├── js/
│   └── main.js
└── README.md
```

## Development
- Pure HTML5, CSS3, and vanilla JavaScript
- No build process required
- Test locally by opening index.html in a browser
- Ensure all paths are relative for S3 deployment

## Dependencies
- Google Fonts (Montserrat, Open Sans)
- Font Awesome 6
- Formspree for contact form handling 