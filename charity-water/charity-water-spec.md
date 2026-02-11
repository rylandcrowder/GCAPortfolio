# charity: water Landing Page - Specification Document

## Overview
A clean, impactful landing page for charity: water featuring a split-screen design with compelling copy on the left and an emotional hero image on the right.

## Color Palette
- **Navy Blue**: `#003366` - Primary text, headings
- **Black**: `#000000` - Logo text
- **Yellow**: `#ffc907` - CTA button, brand accent
- **Cream**: `#fff7e1` - Left panel background
- **White**: `#ffffff` - General text, backgrounds

## Layout Structure

### Container
- Full viewport height (100vh)
- Split into two equal columns (50/50) on desktop
- Stacked vertically on mobile

### Left Panel
- **Background**: `#fff7e1` (cream)
- **Padding**: Generous padding (60-80px on desktop, 40px on mobile)
- **Content alignment**: Left-aligned, vertically centered

### Right Panel
- **Background**: Hero image (full coverage)
- **Image**: `hero-image.jpg` or `hero-image.png`
- **Object-fit**: Cover (fills entire panel while maintaining aspect ratio)

## Typography

### Logo
- **Text**: "charity: water"
- **Icon**: Yellow jerry can icon to the left
- **Font**: Serif font (similar to Tiempos or Georgia)
- **Size**: 24-28px
- **Color**: `#000000`
- **Spacing**: Lowercase with letter-spacing
- **Position**: Top left of left panel

### Main Heading
- **Text**: "Everyone deserves clean water"
- **Font**: Bold sans-serif (similar to Inter, Helvetica, or Arial)
- **Size**: 48-56px on desktop, 32-40px on mobile
- **Color**: `#003366`
- **Line height**: 1.2
- **Margin**: 60px top from logo, 30px bottom

### Subheading
- **Text**: "For only $10 per month, you can provide 3 people with access to safe and clean water"
- **Font**: Regular sans-serif
- **Size**: 20-24px on desktop, 18-20px on mobile
- **Color**: `#003366`
- **Line height**: 1.5
- **Margin**: 40px bottom

### CTA Button
- **Text**: "Join the Change"
- **Background**: `#ffc907` (yellow)
- **Color**: `#003366` (navy text)
- **Font**: Bold sans-serif
- **Size**: 18-20px
- **Padding**: 18px 48px
- **Border-radius**: 50px (fully rounded pill shape)
- **Border**: None
- **Margin**: 40px bottom
- **Hover state**: Slightly darker yellow or subtle shadow
- **Cursor**: Pointer

### Trust Statement
- **Text**: "100% of gifts will fund water projects"
- **Font**: Regular sans-serif
- **Size**: 14-16px
- **Color**: `#003366`
- **Position**: Below CTA button

## Assets Required

### Logo Icon
- **Filename**: `logo-icon.svg` or `logo-icon.png`
- **Type**: Yellow jerry can icon
- **Dimensions**: ~32-40px square
- **Color**: `#ffc907`

### Hero Image
- **Filename**: `hero-image.jpg` or `hero-image.png`
- **Content**: Photo of person(s) with water containers near a water source
- **Aspect ratio**: Vertical/portrait orientation preferred
- **Quality**: High resolution (at least 1200px width)
- **Position**: Right 50% of viewport

## Responsive Behavior

### Desktop (≥1024px)
- Two-column layout (50/50 split)
- Left panel with all text content
- Right panel with hero image
- Maximum width consideration for very wide screens

### Tablet (768px - 1023px)
- Two-column layout maintained
- Slightly reduced padding
- Font sizes slightly smaller

### Mobile (<768px)
- Single column, stacked layout
- Hero image on top (40-50vh height)
- Text content below
- Reduced padding (20-30px)
- Smaller font sizes
- Full-width CTA button

## Component Structure

```
<body>
  <main class="landing-page">
    <section class="content-panel">
      <header>
        <logo>
          <icon />
          <text>charity: water</text>
        </logo>
      </header>
      
      <div class="content-wrapper">
        <h1>Everyone deserves clean water</h1>
        <p class="subheading">
          For only $10 per month, you can provide 3 people 
          with access to safe and clean water
        </p>
        <button class="cta">Join the Change</button>
        <p class="trust-statement">
          100% of gifts will fund water projects
        </p>
      </div>
    </section>
    
    <section class="hero-panel">
      <img src="hero-image.jpg" alt="People accessing clean water" />
    </section>
  </main>
</body>
```

## Spacing Guidelines
- Logo to heading: 60-80px
- Heading to subheading: 30-40px
- Subheading to CTA: 40-50px
- CTA to trust statement: 30px
- Panel padding (desktop): 60-80px
- Panel padding (mobile): 30-40px

## Accessibility Requirements
- Semantic HTML5 elements
- Alt text for images
- Sufficient color contrast (WCAG AA minimum)
- Keyboard navigable CTA button
- Focus states visible
- Responsive font sizing

## Browser Support
- Modern browsers (Chrome, Firefox, Safari, Edge)
- CSS Grid or Flexbox for layout
- Responsive images with srcset if needed

## Additional Notes
- The design emphasizes simplicity and emotional impact
- The split-screen creates a strong visual balance
- The yellow CTA button stands out against the cream background
- The navy blue creates a professional, trustworthy feel
- All copy should match exactly as specified
- The hero image should evoke emotional connection to the cause
