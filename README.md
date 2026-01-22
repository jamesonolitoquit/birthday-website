# Birthday Surprise Website

A playful, animated birthday surprise website that starts as a portfolio and transforms into a festive celebration.

## Features

- **Disguised Portfolio**: Initially looks like a professional portfolio
- **Surprise Popup**: Triggers the transformation after 3 seconds
- **GSAP Animations**: Master timeline controls all major animations
- **Name Morph**: "Franchezca Anne Ortiz" rearranges to "Chazie"
- **Canvas Animals**: Cartoon cats and dogs with sprite animations
- **Scroll Reveals**: Progressive content reveals with parallax
- **Mobile Optimized**: Performance optimizations for mobile devices
- **Accessibility**: Respects `prefers-reduced-motion`

## Setup

1. Install dependencies:
   ```bash
   npm install
   ```

2. Run development server:
   ```bash
   npm run dev
   ```

3. Open [http://localhost:3000](http://localhost:3000)

## Customization

### Adding Photos
- Place images in `/public/images/`
- Update the photo placeholders in `src/app/page.tsx`

### Adding Music
- Add birthday music to `/public/birthday-song.mp3`
- Uncomment the audio code in `src/lib/gsap-timeline.ts` and `src/app/page.tsx`

### Sprite Sheets
- Add cat and dog sprite sheets to `/public/sprites/`
- Update `src/lib/canvas-animals.ts` to load and animate sprites

## Deployment

Deploy to Vercel for free hosting:

1. Push to GitHub
2. Connect to Vercel
3. Deploy automatically

## Architecture

- **State A**: Monochrome portfolio (no birthday hints)
- **State B**: Pastel birthday celebration
- **GSAP Timeline**: Controls transformation sequence
- **Canvas**: Animal animations
- **ScrollTrigger**: Parallax and reveals

## Performance

- Canvas throttling on mobile
- Respects reduced motion preferences
- Lazy loading and optimized animations
