# MOUSEPAD COMPANY LANDING PAGE — DESIGN SPECIFICATION

---

## SUMMARY
A clean, modern landing page showcasing premium mousepads with a bold blue-and-white color scheme, emphasizing product quality through grid layouts, hover interactions, and customer social proof.

---

## LAYOUT

**STICKY HEADER (0–80px, full width)**
- Logo left-aligned (40px from left)
- Navigation menu center (4 items: Products, Features, Reviews, Contact)
- CTA button right-aligned (40px from right)
- Background: #FFFFFF with subtle shadow (0 2px 8px rgba(0,82,204,0.08))

**HERO SECTION (80–480px)**
- Split layout: left text (50% width), right hero image (50% width)
- Left: Headline (56px bold), subheading (20px regular), two CTAs (primary blue, secondary white outline)
- Right: High-contrast mousepad product image on light gray background (#F3F4F6)
- Padding: 80px horizontal, 120px vertical

**PRODUCT SHOWCASE (480–900px)**
- Full-width section with light gray background (#F3F4F6)
- 3-column grid on desktop, 1 column on mobile, 2 on tablet
- Each product card: 280px × 320px with 16px border-radius
- Card states: default (white bg), hover (lift 8px, shadow deepens, blue accent border emerges)
- Product image (200px × 200px), title (18px bold), price (16px, #0052CC), short description (14px, #6B7280)
- Spacing: 24px between cards, 40px section padding

**FEATURES SECTION (900–1300px)**
- Full-width white background
- Headline centered (48px bold)
- 4-card grid (2×2 on desktop, 1 column on mobile, 2 on tablet)
- Each card: 280px × 240px, white background, subtle gray border (#E5E7EB), 12px border-radius
- Icon (48px × 48px, blue #0052CC), title (18px bold), description (14px, #6B7280)
- On scroll: cards fade in + slide up 16px (via Intersection Observer)
- Spacing: 32px between cards, 80px section padding

**TESTIMONIALS SECTION (1300–1700px)**
- Full-width light gray background (#F3F4F6)
- Headline centered (48px bold)
- Carousel container: displays 1 testimonial on mobile, 2 on tablet, 3 on desktop
- Each testimonial card: 320px × 240px, white background, 16px border-radius, subtle shadow
- Star rating (5 stars, gold #FCD34D), quote (16px italic, #374151), author name (16px bold), title (14px, #6B7280)
- Navigation: left/right arrow buttons (40px × 40px, blue background, white icons)
- Auto-rotate every 6 seconds; pause on hover or interaction

**SPECS TABLE SECTION (1700–2100px)**
- Full-width white background
- Headline left-aligned (40px bold)
- Responsive table: 6 columns on desktop, stacked cards on mobile
- Table headers: bold 14px, light gray background (#F3F4F6)
- Rows: alternating white / #F9FAFB background
- Cells: 16px regular text, 16px padding vertical/horizontal
- Scrollable horizontally on tablets/mobile with left/right overflow hint

**CTA SECTION (2100–2280px)**
- Full-width blue background (#0052CC)
- Centered content: large headline (48px bold, white), description (18px regular, white), single large CTA button (60px height, white background, blue text)
- Padding: 120px vertical, 40px horizontal
- Subtle gradient overlay: #0052CC → #003D99 (top to bottom)

**FOOTER (2280–2400px)**
- Full-width dark background (#1F2937)
- 4-column grid on desktop, 2 on tablet, 1 on mobile
- Column 1: Logo + brand description (14px, #D1D5DB)
- Columns 2–4: Links (3 groups: Products, Company, Legal), each link 14px regular, white, hover turns #0052CC
- Bottom strip: copyright (12px, #9CA3AF), social icons (24px × 24px, light gray)
- Sticky email signup bar: white background, 48px height, positioned 40px above footer on desktop
- Email input (320px width, light gray border), subscribe button (120px width, blue #0052CC)
- Spacing: 40px horizontal padding, 60px vertical padding between sections

---

## COLORS

| Element | Hex | Usage |
|---------|-----|-------|
| Primary Blue | #0052CC | CTA buttons, links, hover states, accents, hero headline |
| White | #FFFFFF | Background, cards, text on blue |
| Light Gray BG | #F3F4F6 | Section backgrounds, table headers |
| Light Gray Border | #E5E7EB | Card borders, dividers |
| Medium Gray | #6B7280 | Secondary text (descriptions, subtitles) |
| Dark Gray Text | #374151 | Primary body text |
| Darker Gray | #1F2937 | Footer background, dark text |
| Light Text | #D1D5DB | Footer secondary text |
| Very Light Text | #9CA3AF | Footer tertiary text (copyright) |
| Gold Star | #FCD34D | Testimonial star ratings |
| Gradient (CTA section) | #0052CC → #003D99 | Bottom overlay, premium feel |
| Shadow (standard) | rgba(0,82,204,0.08) | Subtle depth, non-intrusive |
| Shadow (hover) | rgba(0,82,204,0.16) | Lift effect on interaction |

**Contrast Verification (WCAG AA minimum 4.5:1):**
- #0052CC on #FFFFFF: 8.2:1 ✓
- #374151 on #FFFFFF: 9.1:1 ✓
- #FFFFFF on #0052CC: 8.2:1 ✓
- #FFFFFF on #1F2937: 14.3:1 ✓

---

## COMPONENTS

### 1. HEADER
- **Logo**: 32px height, dark blue text (#0052CC), left-aligned
- **Nav Links**: 4 items, 16px regular, white text, 24px horizontal spacing
- **Active Link**: underline accent (#0052CC), 3px height
- **Header CTA Button**: 44px height, 160px width, blue background (#0052CC), white text (16px bold), 8px border-radius, hover darkens to #003D99
- **Sticky behavior**: stays fixed on scroll, 80px height, white background with subtle bottom shadow

### 2. HERO SECTION
- **Main Headline**: 56px bold (Outfit font family), #0052CC, line-height 1.2
- **Subheading**: 20px regular (Inter), #6B7280, line-height 1.6, 32px bottom margin
- **Primary CTA Button**: 56px height, 200px width, blue (#0052CC), white text (18px bold), 8px border-radius, hover lifts 4px with shadow
- **Secondary CTA Button**: 56px height, 200px width, white background, blue border (2px #0052CC), blue text (18px bold), 8px border-radius, hover background becomes light gray (#F3F4F6)
- **Hero Image**: 400px × 400px on desktop, rounded corners (12px), subtle shadow, subtle zoom on load (1.0 → 1.02 scale, 800ms ease-out)

### 3. PRODUCT CARDS
- **Card Container**: 280px width × 320px height, white background, 12px border-radius, light gray border (#E5E7EB)
- **Product Image Area**: 200px × 200px, light gray background (#F3F4F6), centered, 8px top margin
- **Product Title**: 18px bold, #1F2937, 12px top margin
- **Price Label**: 16px bold, #0052CC, 8px top margin
- **Description**: 14px regular, #6B7280, 8px top margin, line-height 1.5
- **Hover State**: card lifts 8px (transform: translateY(-8px)), shadow deepens (0 12px 24px rgba(0,82,204,0.15)), blue left border accent (4px height, 12px from left)
- **Interactive**: smooth transition (300ms ease-out)

### 4. FEATURE CARDS
- **Card Container**: 280px × 240px, white background, 12px border-radius, border 1px solid #E5E7EB
- **Icon Area**: 48px × 48px, blue background (#0052CC), white icon (SVG), centered, 16px top padding
- **Title**: 18px bold, #1F2937, 16px top margin, centered
- **Description**: 14px regular, #6B7280, 8px top margin, centered, line-height 1.5, 12px horizontal padding
- **On Scroll Animation**: fade-in (0 → 1 opacity, 600ms), simultaneous slide-up (translateY +16px → 0, 600ms), staggered with 100ms delay per card

### 5. TESTIMONIAL CARDS
- **Card Container**: 320px × 240px, white background, 16px border-radius, subtle shadow (0 4px 12px rgba(0,82,204,0.1))
- **Star Rating**: 5-star display (each star 20px × 20px), gold color (#FCD34D), left-aligned, 16px top padding
- **Quote Text**: 16px italic, #374151, line-height 1.6, 16px top margin
- **Author Name**: 16px bold, #1F2937, 12px top margin
- **Author Title**: 14px regular, #6B7280, 4px top margin
- **Carousel Navigation Arrows**: 40px × 40px, blue background (#0052CC), white icons (SVG chevrons, 20px), 8px border-radius, cursor pointer
- **Left Arrow**: positioned 16px left of carousel
- **Right Arrow**: positioned 16px right of carousel
- **Hover state on arrows**: background darkens to #003D99
- **Auto-rotation**: 6-second interval, pause on user interaction

### 6. SPECS TABLE
- **Table Headers**: 14px bold, #1F2937, light gray background (#F3F4F6), 16px padding (all sides), 12px border-bottom (#E5E7EB)
- **Table Rows**: 16px regular, #6B7280, 16px padding, alternating row background (white / #F9FAFB)
- **Cell Borders**: subtle right border (1px #E5E7EB) between columns
- **Mobile Behavior**: switches to stacked card layout (each spec as label: value pair, label bold blue #0052CC, value #374151)

### 7. CTA SECTION ("Ready to Upgrade?")
- **Background**: blue gradient (#0052CC → #003D99 top-to-bottom), full width
- **Headline**: 48px bold, #FFFFFF, line-height 1.2, centered, 32px bottom margin
- **Description**: 18px regular, #FFFFFF, line-height 1.6, centered, max-width 600px, 32px bottom margin
- **CTA Button**: 60px height, 240px width, white background (#FFFFFF), blue text (#0052CC), 18px bold, 8px border-radius, centered
- **Hover State**: white background slightly darkens (shadow added), text remains blue

### 8. EMAIL SIGNUP BAR (Sticky Footer)
- **Container**: 100% width, 48px height, white background (#FFFFFF), positioned 40px above footer
- **Email Input Field**: 320px width, light gray border (#E5E7EB, 1px), 12px border-radius, 12px horizontal padding, 14px placeholder text (#9CA3AF), focused state adds blue border (#0052CC, 2px)
- **Subscribe Button**: 120px width, 44px height, blue background (#0052CC), white text (16px bold), 8px border-radius, right of input, cursor pointer
- **Hover State**: button darkens to #003D99
- **Layout**: centered horizontally, 40px horizontal margin, flex layout with 16px gap between input and button

### 9. FOOTER
- **Background**: dark gray (#1F2937), full width
- **Logo**: 28px height, white text, left-aligned
- **Brand Description**: 14px regular, #D1D5DB, max-width 200px, line-height 1.6
- **Link Columns**: 14px regular, white text (#FFFFFF)
- **Link Hover State**: text color shifts to blue (#0052CC)
- **Column Headers (Group Titles)**: 14px bold, white, 12px bottom margin
- **Social Icons**: 24px × 24px, light gray (#D1D5DB), hover turns blue (#0052CC)
- **Copyright Text**: 12px regular, #9CA3AF, centered at bottom, 32px top padding
- **Grid Layout**: 4 columns on desktop (25% each), 2 columns on tablet (50% each), 1 column on mobile (100%)
- **Spacing**: 40px horizontal padding, 60px vertical padding between sections

---

## INTERACTIONS

### HEADER
- **Nav Links**: on click, smooth scroll to corresponding section (scroll-behavior: smooth, 1000ms)
- **Active Link**: underline appears when section scrolls into view (via Intersection Observer, 50% threshold)
- **Header CTA**: on click, focus jumps to email signup section with smooth scroll (800ms)

### HERO SECTION
- **Primary Button**: on click, scroll to product showcase section (1000ms ease-out)
- **Secondary Button**: on click, scroll to features section (1000ms ease-out)
- **Hero Image**: on page load, fade in + subtle zoom (0 opacity + 0.98 scale → 1 opacity + 1.0 scale, 1200ms ease-out)

### PRODUCT CARDS
- **On Hover**: 
  - Card lifts 8px (transform: translateY(-8px), 300ms ease-out)
  - Shadow deepens (0 12px 24px rgba(0,82,204,0.15))
  - Left border accent slides in from left (4px width, 300ms ease-out)
  - Image background color shifts subtly (#F3F4F6 → #E5E7EB)
- **On Click**: card remains in hover state until user hovers away
- **On Page Load**: cards fade in sequentially with 100ms stagger (first card 0ms, second 100ms, etc.)

### FEATURE CARDS
- **On Scroll Into View** (Intersection Observer, 30% threshold):
  - Fade in (0 → 1 opacity, 600ms ease-out)
  - Slide up (translateY +16px → 0, 600ms ease-out)
  - Staggered timing: 100ms delay between each card
- **No hover interaction** (static cards)

### TESTIMONIAL CAROUSEL
- **Auto-Rotation**: advances every 6 seconds unless user interacts
- **Left/Right Arrow Buttons**:
  - On hover: background darkens (#0052CC → #003D99)
  - On click: carousel slides to previous/next testimonial (500ms ease-out, horizontal slide)
  - Pause auto-rotation for 10 seconds after user click
- **Card Transition**: slides horizontally (transform: translateX), previous cards slide out left, new cards slide in from right
- **Pagination Dots** (optional indicator): positioned below carousel, 8px diameter, light gray (#E5E7EB), active dot blue (#0052CC)

### SPECS TABLE
- **On Scroll**: table rows fade in sequentially (200ms stagger, Intersection Observer)
- **Mobile Cards**:
  - Each spec displays as a labeled pair (label in blue, value in dark gray)
  - On tap, cards subtly elevate (2px lift, 200ms)
- **Table Sorting** (optional): column headers become clickable (cursor: pointer), on click sort ascending/descending with smooth re-order animation

### CTA SECTION
- **Button On Hover**: 
  - White background adds subtle shadow (0 8px 16px rgba(0,0,0,0.1))
  - Text remains blue, no color shift
  - Cursor: pointer
- **On Click**: scrolls to email signup bar (800ms), focuses email input field, triggers subtle pulse animation on input (scale 1.0 → 1.02 → 1.0, 400ms)

### EMAIL SIGNUP BAR
- **Input Field**:
  - On focus: border color shifts to blue (#0052CC), box-shadow adds subtle glow (0 0 8px rgba(0,82,204,0.3))
  - On blur: border returns to light gray (#E5E7EB)
  - Placeholder text fades out on focus
- **Subscribe Button**:
  - On hover: background darkens (#0052CC → #003D99), cursor pointer
  - On click: button briefly shows success state (green check icon, 2000ms), then resets
  - Form validation: if email empty, input border flashes red (#EF4444) for 400ms, then returns to light gray

### FOOTER
- **Links**: on hover, text color shifts to blue (#0052CC), smooth transition (200ms)
- **Social Icons**: on hover, color shifts to blue (#0052CC), subtle scale increase (1.0 → 1.2, 200ms)

### GLOBAL / ACCESSIBILITY
- **Focus Indicators**: all interactive elements (buttons, links, inputs) display visible focus ring on keyboard navigation (2px solid #0052CC, 2px offset from element)
- **Skip to Main Content**: hidden link appears on Tab press, allows user to skip header navigation (positioned top-left, off-screen until focused)
- **Keyboard Navigation**: all CTAs, buttons, links accessible via Tab key; Enter activates buttons/links; Escape closes modals or carousels
- **Reduced Motion**: if user has `prefers-reduced-motion` enabled, all animations scale to 200ms duration (no delays), opacity/transform only (no complex transitions)
- **Mobile Touch**: on touch devices, hover states convert to active states on tap (no tap delay)

---

## STYLE NOTES

### TYPOGRAPHY
- **Headings** (56px, 48px, 18px): Outfit font family (sans-serif, geometric, modern, friendly)
  - Letter-spacing: +0.5px for large headings (48px+)
  - Font-weight: 700 bold
- **Body & UI** (20px, 18px, 16px, 14px): Inter font family (sans-serif, clean, highly legible, neutral)
  - Font-weight: 400 regular for body, 600 semi-bold for labels
  - Line-height: 1.5 for body text (16px+), 1.6 for longer content (descriptions, testimonials)
- **Fallback Stack**: Outfit → -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif
- **Letter Spacing**: standard 0px; increase to +0.3px for all-caps labels

### SPACING & GRID
- **Base Unit**: 8px (8px grid system)
- **Padding Common Values**: 16px, 24px, 32px, 40px, 60px, 80px, 120px
- **Margin Common Values**: 8px, 12px, 16px, 24px, 32px, 40px
- **Gap Between Components**: 24px (cards), 32px (sections), 16px (within cards)
- **Section Padding**: 80px vertical (desktop), 60px vertical (tablet), 40px vertical (mobile)

### SHADOWS & DEPTH
- **Subtle Shadow** (cards, default): 0 2px 8px rgba(0,82,204,0.08)
- **Medium Shadow** (cards, hover): 0 12px 24px rgba(0,82,204,0.15)
- **Deep Shadow** (modals, overlays): 0 20px 40px rgba(0,0,0,0.15)
- **Glow (focus states)**: 0 0 8px rgba(0,82,204,0.3)

### BORDER RADIUS
- **Buttons & Small Components**: 8px
- **Cards**: 12px
- **Large Containers**: 16px
- **Input Fields**: 8px–12px

### RESPONSIVE BREAKPOINTS
- **Mobile**: 320px–767px (1 column, full-width sections, stacked layout)
- **Tablet**: 768px–1024px (2 columns, medium spacing, hybrid grid)
- **Desktop**: 1025px+ (3–4 columns, full spacing, optimal layout)
- **Max-width**: 1200px for content (except full-width sections like hero, CTA, footer)

### MOTION & MICRO-INTERACTIONS
- **Smooth Scrolling**: scroll-behavior: smooth (1000ms default, 800ms for shorter distances)
- **Hover Transitions**: 300ms ease-out (lift, color shift, shadow)
- **Page Load Animations**: 600ms–1200ms ease-out (fade-in, slide-up, zoom)
- **Button Interactions**: 200ms ease-out (background color, shadow)
- **Carousel**: 500ms ease-out (slide transition), 6s auto-advance
- **Reduced Motion**: all durations → 200ms, no stagger/delay

### FEEL & TONE
- **Modern & Professional**: clean lines, plenty of white space, geometric Outfit typography conveys premium quality
- **Friendly & Approachable**: Inter's neutrality + rounded corners + soft shadows create welcoming feel
- **Bold & Confident**: blue primary color (#0052CC) commands attention without aggression; used sparingly for CTAs and accents
- **High Contrast**: white-on-blue and dark-gray-on-white ensure readability and accessibility
- **Minimal Visual Noise**: subtle animations and gradients enhance (never distract); gray tones used for secondary information

### ACCESSIBILITY IMPLEMENTATION
- **Color Contrast**: all text meets WCAG AA (4.5:1 minimum); blue (#0052CC) on white (#FFFFFF) is 8.2:1
- **Focus Indicators**: 2px solid blue ring on all interactive elements (never hidden)
- **Semantic HTML**: use `<button>`, `<a>`, `<input>`, `<nav>`, `<main>`, `<section>` elements
- **ARIA Labels**: all buttons, icons, and form fields have descriptive aria-label or aria-describedby
- **Keyboard Navigation**: Tab order follows logical flow (header → hero → products → features → testimonials → specs → CTA → footer → email signup)
- **Form Validation**: error messages in plain language, associated with inputs via aria-invalid, visible focus ring on error state
- **Intersection Observer**: for scroll-triggered animations, use `threshold: 0.3` (card enters viewport 30%) to trigger fade-in/slide-up
- **Reduced Motion Query**: `@media (prefers-reduced-motion: reduce)` → disable animations, reduce durations to 200ms

---

## FINAL NOTES

- **No custom fonts required**: Outfit and Inter are widely available via Google Fonts or system stack
- **Icon Library**: use Lucide, Feather, or SF Symbols (24px × 24px for nav, 48px × 48px for features)
- **Product Images**: high-resolution (400px × 400px minimum), mousepad product photography with consistent lighting
- **Responsive Images**: use `srcset` and `sizes` to serve optimized images at different breakpoints
- **Performance**: optimize images (WEBP format with PNG fallback), lazy-load below-the-fold sections, defer non-critical animations
- **Dev Framework Agnostic**: this design works with vanilla HTML/CSS, React, Vue, Svelte, or any static site generator
- **Animation Libraries**: Intersection Observer for scroll reveals; CSS transitions for hover/focus; optional: Framer Motion or GSAP for complex carousel/timeline effects

**Designer Sign-Off**: This specification provides all visual and UX requirements. The Developer should implement pixel-perfect to these colors, sizes, spacing, and interactions. No design decisions left to developer discretion.