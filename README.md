# Image Changer Pop-up

A customizable, interactive pop-up that cycles through images when a button is clicked


## Project Overview

This project creates a stylized pop-up window that displays a series of images. Each time the user clicks the button, the image changes to the next one in sequence. When the last image is reached, the button disappears and a final message is displayed.

## What you'll learn

* CSS Variables for easy customization
* Basic HTML flex structure
* JavaScript event handling
* DOM manipulation

## Features

- Customizable colors, fonts, and styling through CSS variables
- Customizable background image, main image sequence, and all the texts 
- Smooth fade transitions between images
- Mobile-responsive design
- Decorative UI elements (close and shrink buttons)

## 📁 Project Structure

```
image-changer-popup/
├── assets/
│   ├── image-content/
│   │   ├── image-1.png
│   │   ├── image-2.png
│   │   ├── image-3.png
│   │   ├── image-4.png
│   │   ├── image-5.png
│   │   └── image-6.png
│   ├── close-icon.png
│   ├── favicon.png
│   ├── main-bg.png
│   └── shrink-icon.png
├── index.html
├── style.css
└── index.js
```

## How It Works

1. The page loads with a stylized pop-up container
2. The first image is displayed automatically
3. When the user clicks the "Grow!" button:
   - The current image fades out
   - The next image is preloaded
   - Once loaded, the new image fades in
4. After reaching the final image:
   - The button disappears
   - A final message is displayed

## Customization Options

### Colors and Styling

All visual elements can be customized through CSS variables in the `:root` section of `style.css`:

```css
:root {
  /* Colors */
  --color-page-background: #50AFC9;
  --color-main-container-background: #FF5B70;
  --color-inner-container-background: #FFF7F4;
  --color-border: #9E0E2B;
  --color-button-background: #FFF;
  --color-heading-text: #FFF;
  --color-button-text: #9E0E2B;
  --color-message-text: #9E0E2B;
  
  /* Images */
  --image-path-background: url('assets/main-bg.png');
  --image-path-content: url('assets/image-content/image-1.png');
  
  /* Fonts */
  --font-family-main: "Pixelify Sans", sans-serif;
  /* ... and more variables ... */
}
```

### Text Content

Modify the following in the HTML file:

- Page title: `<title>For you &lt;3</title>`
- Header text: `<h1>For you &lt;3</h1>`
- Button text: `<button id="waterButton">Grow!</button>`
- Final message: `<div class="final-message">Have a good day!</div>`

### Images

1. Replace the images in the `assets/image-content/` directory with your own
2. Make sure to keep the same filenames or update the paths in the JavaScript array
3. You can add more images by adding more entries to the array

```javascript
const images = [
  './assets/image-content/image-1.png',
  './assets/image-content/image-2.png',
  // Add more images here...
];
```

## 🌐 Hosting on Netlify

You can easily deploy this project using Netlify's free plan:

**Prepare your project**:
* Make sure your files are named correctly: `index.html` and `index.js` (if you renamed them)
* Ensure all file paths are correct (case-sensitive)

**Sign up for Netlify**:
* Go to netlify.com and sign up for a free account
* You can sign up using GitHub, GitLab, Bitbucket, or email

**Deploy your site**: 
* Simply drag and drop your project folder onto the Netlify dashboard
* Netlify will automatically deploy your site

**Configure your site**:
* After deployment, you can customize your site name
* Go to "Site settings" → "Change site name"
* Your site will be available at `your-site-name.netlify.app`

**Update your site**:
* If you used the drag and drop method, simply drag and drop your folder again
* If you connected to Git, just push changes to your repository


## Installation

1. Download or clone this repository
2. No build process needed - open `index.html` directly in your browser
3. To modify, edit the HTML, CSS, and JavaScript files with any text editor

## Project Extension Ideas

- Add click functionality to the close and shrink icons
- Implement a restart button after reaching the final image
- Add sound effects for button clicks and transitions

