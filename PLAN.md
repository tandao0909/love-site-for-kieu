# Love Site for Kieu - Project Plan

## Overview
A soft, dreamy one-page website that tells Kieu how much she is loved. Features a love letter, a relationship countdown tracker, and hidden click surprises scattered throughout.

---

## Design Direction: Soft & Dreamy

### Color Palette
- **Primary:** Soft blush pink `#F8C8D8`
- **Secondary:** Lavender `#D8BFE6`
- **Accent:** Warm rose `#E8879C`
- **Background:** Cream white `#FFF5F7` with subtle gradient to soft pink
- **Text:** Warm dark `#4A3040`

### Typography
- **Headings:** Serif or script font (e.g., "Playfair Display" or "Dancing Script" from Google Fonts)
- **Body:** Soft rounded sans-serif (e.g., "Quicksand" or "Nunito")

### Visual Style
- Soft drop shadows, rounded corners, glassmorphism cards
- Gentle floating/fade-in animations on scroll
- Subtle grain or watercolor texture overlay on background
- Decorative elements: small hearts, stars, flower petals

---

## Page Sections (Top to Bottom)

### 1. Hero Section
- Large dreamy heading: "For Kieu"
- Soft tagline like "Every moment with you is a gift"
- Gentle fade-in animation on load
- Subtle floating heart particles in background

### 2. Love Counter / Countdown Tracker
- Shows how long you've been together (days, hours, minutes, seconds - live ticking)
- Styled in a soft glassmorphism card
- Needs a configurable start date (relationship anniversary)
- Format: "We've been in love for X days, Y hours, Z minutes, S seconds"

### 3. Love Letter Section
- A beautifully styled letter/message area
- Styled like a handwritten note on soft paper
- Slightly tilted card with paper texture background
- Content: a heartfelt message (placeholder text, easy to customize)

### 4. Hidden Click Surprises (scattered throughout)
- **Heart burst:** Clicking certain elements triggers a burst of floating hearts
- **Secret messages:** Small interactive elements (a star icon, a flower, etc.) that reveal hidden love notes in a tooltip or modal when clicked
- **Envelope reveal:** A clickable sealed envelope that "opens" to show a bonus message
- At least 3-5 hidden surprises across the page to encourage exploration

### 5. Footer
- A simple closing line like "Made with all my love"
- Small heart icon

---

## Tech Stack
- **HTML** - Single `index.html` file
- **CSS** - Embedded styles (or single `style.css`), no framework needed
- **JavaScript** - Vanilla JS for countdown timer, animations, and click interactions
- **Fonts** - Google Fonts (Dancing Script + Quicksand)
- **No build tools** - Just open `index.html` in a browser

---

## Interactive Details

### Click Surprises (Implementation Notes)
1. **Heart Explosion** - Clicking the main heading spawns 15-20 small hearts that float upward and fade out (CSS keyframe animations, JS to create elements)
2. **Hidden Love Notes** - 3 small clickable icons (flower, star, cloud) placed decoratively. Each reveals a short message in a soft popup/modal
3. **Envelope** - A sealed envelope illustration at the bottom. On click, it animates open and reveals a final secret message
4. **Sparkle Trail** - Optional: subtle sparkle particles follow the mouse cursor across the page

### Countdown Timer
- JavaScript `setInterval` updating every second
- Configurable `START_DATE` constant at the top of the script
- Graceful display: "X days, Y hours, Z minutes, S seconds"

---

## File Structure
```
love-site-for-kieu/
  PLAN.md          <-- this file
  index.html       <-- main page (HTML + embedded CSS + JS)
```

Keeping it as a single HTML file for simplicity - easy to share, host, or send as a file.

---

## Customization Points (Easy to Edit)
- `START_DATE` - set the relationship start date
- Love letter text - edit the message content
- Hidden messages - change the secret notes
- Her name - currently "Kieu", easily swappable
- Colors - all defined as CSS custom properties at the top

---

## Deployment Options
- Open locally in any browser
- Host free on GitHub Pages, Netlify, or Vercel
- Or simply send her the HTML file

---

## Next Steps
1. Build the full `index.html` with all sections, styles, and interactions
2. Add placeholder love letter text (user can customize)
3. Test all click surprises and animations
4. Polish transitions and responsiveness (mobile-friendly)
