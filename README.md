# Wyndemere Halloween Medallion Hunt

A simple static HTML website for a Halloween medallion hunt. No JavaScript required - just edit the HTML file to add new clues!

## Features

- **Simple HTML Structure**: Easy to edit and understand
- **Responsive Design**: Works on all devices  
- **Halloween Theme**: Spooky orange and purple design
- **No Dependencies**: Just HTML and CSS - works anywhere

## How to Add New Daily Clues

### Step 1: Add the New Clue
In `index.html`, find the section with clues and add a new clue using this template:

```html
<!-- Day X Clue - Available Now -->
<div class="clue-card available">
    <div class="clue-header">
        <h3>Day X - [Date]</h3>
        <span class="clue-status available">Available Now</span>
    </div>
    <div class="clue-content">
        <p class="clue-text">Your clue text goes here.</p>
        <p class="clue-hint">💡 Hint: Your hint goes here</p>
    </div>
</div>
```

### Step 2: Update "Coming Soon" Clues
To reveal a clue, find the commented-out clue and:

1. **Remove** the "Coming Soon" version:
```html
<!-- Remove this entire block -->
<div class="clue-card upcoming">
    <div class="clue-header">
        <h3>Day 2 - October 25, 2025</h3>
        <span class="clue-status upcoming">Coming Soon</span>
    </div>
    <div class="clue-content">
        <p class="upcoming-text">Next clue will be revealed tomorrow!</p>
    </div>
</div>
```

2. **Uncomment** the actual clue by removing `<!--` and `-->`:
```html
<!-- Change this: -->
<!--
<div class="clue-card available">
    <div class="clue-header">
        <h3>Day 2 - October 25, 2025</h3>
        <span class="clue-status available">Available Now</span>
    </div>
    <div class="clue-content">
        <p class="clue-text">By the water's gentle flow, where the lily pads do grow.</p>
        <p class="clue-hint">💡 Hint: Near the community pond</p>
    </div>
</div>
-->

<!-- To this: -->
<div class="clue-card available">
    <div class="clue-header">
        <h3>Day 2 - October 25, 2025</h3>
        <span class="clue-status available">Available Now</span>
    </div>
    <div class="clue-content">
        <p class="clue-text">By the water's gentle flow, where the lily pads do grow.</p>
        <p class="clue-hint">💡 Hint: Near the community pond</p>
    </div>
</div>
```

## File Structure

```
wyndemerehalloween/
├── index.html          # Main HTML file (edit this to add clues)
├── styles.css          # Halloween-themed CSS
└── README.md           # This file
```

## Quick Start

1. Open `index.html` in any web browser
2. To add new clues, edit the HTML file
3. Save and refresh the browser to see changes
4. No server required - works as local files or on any web host

## Deployment

This static website can be hosted anywhere:

- **GitHub Pages**: Push to GitHub and enable Pages
- **Netlify**: Drag and drop the folder  
- **Any Web Host**: Upload the files to any web server
- **Local Use**: Just open `index.html` in a browser

No server-side configuration required!