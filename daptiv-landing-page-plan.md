# 🎯 Daptiv Landing Page Implementation Plan

## **Project Structure**
Create a new repository `daptiv-landing` with clean, maintainable static site:
```
daptiv-landing/
├── index.html              # Main landing page
├── styles.css              # All styles (mobile-first)
├── script.js               # Minimal JS (email capture, smooth scroll)
├── assets/
│   ├── logo.svg           # Daptiv logo
│   ├── favicon.ico        # Favicon
│   └── og-image.png       # Social media preview
├── .gitignore
├── README.md
└── vercel.json            # Deployment config
```

## **Design Implementation (getplanta.com-inspired)**

### 1. **Hero Section**
- **Headline**: "Your personal running coach: listening 24/7, adapting daily"
- **Subheadline**: "Daptiv uses AI and proven coaching science to create training plans that actually adapt to how you feel"
- **CTA Button**: "Join Waitlist - First 100 users get $5/month for life" (cyan background)
- **Trust indicator**: "🔒 Your data stays private. No tracking. No sharing."

### 2. **Features Grid** (3 cards, clean design)
- **Card 1**: "Conversational Coaching"
  - Icon: 💬
  - "Tell your coach how you really feel. No forms, no ratings - just natural conversation about your training."
  
- **Card 2**: "Truly Adaptive Plans"
  - Icon: 🎯
  - "Plans that adjust daily based on your feedback, energy, and life - not rigid schedules."
  
- **Card 3**: "Science-Based Training"
  - Icon: 🧬
  - "Built on proven methodologies used by world-class coaches, adapted by AI to fit you."

### 3. **How It Works** (3 steps)
1. "Chat about your running goals and experience"
2. "Get a personalized 4-week adaptive plan"
3. "Check in daily - your plan evolves with you"

### 4. **Trust Section**
- "Your Privacy Matters"
  - ✓ All data stored locally on your device
  - ✓ Anonymous to AI - no personal data shared
  - ✓ Delete everything anytime
  - ✓ No social features or data mining

### 5. **Scientific Backing**
- "Proven Methods, Personalized Delivery"
- Brief text about Daptiv methodology
- "Used by elite coaches worldwide"

### 6. **Waitlist CTA**
- Early bird pricing highlight
- Email capture form
- "Be among the first 100 - Lock in $5/month forever"

## **Color Scheme & Styling**
```css
:root {
  --cyan: #0891B2;      /* Primary - CTAs, links */
  --amber: #F59E0B;     /* Accents, highlights */
  --forest: #059669;    /* Trust, success states */
  --gray-50: #F8FAFC;   /* Background */
  --gray-900: #0F172A;  /* Text */
}
```

## **Technical Features**
1. **Email Capture**: Simple form posting to Cloudflare Workers or ConvertKit
2. **Analytics**: Cloudflare Web Analytics (free, privacy-focused)
3. **SEO**: Meta tags, Open Graph, structured data
4. **Performance**: 
   - Inline critical CSS
   - Lazy load images
   - Minified assets
   - < 50KB total page weight

## **Mobile-First Responsive**
- Single column on mobile
- Touch-friendly buttons (48px min height)
- 16px+ readable fonts
- Sticky CTA button on mobile scroll

## **Deployment**
1. Push to GitHub repo
2. Connect to Cloudflare Pages or Vercel
3. Custom domain: daptiv.app
4. SSL automatically handled

## **Copy Tone**
- Friendly but knowledgeable
- Focus on benefits, not features
- Personal ("your coach") not corporate ("our platform")
- Emphasize listening and adaptation

Would you like me to start building this landing page in a new repository?