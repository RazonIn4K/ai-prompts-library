# Sales Page Layout Prompts for FG Funnels

**CATEGORY:** Sales Pages / Funnel Building / Layout Design
**PURPOSE:** Ready-to-use layout prompts for arranging sales page sections in FG Funnels blocks while maintaining reference site fidelity
**VARIABLES:** `{brand_color_primary}`, `{brand_color_secondary}`, `{logo_url}`, `{hero_image_url}`, `{testimonial_images}`, `{program_name}`, `{price}`, `{cta_text}`
**TONE:** Conversion-focused, visually clear, mobile-responsive, brand-consistent

---

## 1. Hero Section Layout

### Purpose
The hero is your above-the-fold first impression. It must communicate the transformation, establish authority, and drive immediate action.

### FG Funnels Block Configuration

```
SECTION: Hero
├── Container: Full-width, 100vh minimum height
├── Background: Gradient overlay on image OR solid brand color
└── Content Grid: 2-column (60/40 split) on desktop, stacked on mobile

LEFT COLUMN (60%):
├── Pre-headline badge (optional): Small text, pill-shaped
│   └── Style: Background {brand_color_secondary}, uppercase, 12px, letter-spacing 2px
├── Main Headline: H1
│   └── Style: 48-64px, bold, line-height 1.1, max-width 600px
├── Subheadline: Supporting promise
│   └── Style: 20-24px, regular weight, 60% opacity, max-width 500px
├── Bullet Points (3 max): Quick wins/outcomes
│   └── Style: Icon + text, 16px, checkmarks or custom icons
├── CTA Button: Primary action
│   └── Style: Large (60px height), {brand_color_primary}, rounded, shadow
│   └── Text: "{cta_text}" - action-oriented, 18px bold
└── Trust Badge Row: Payment icons, guarantee seal, "As seen in" logos
    └── Style: Grayscale, 40px height, spaced evenly

RIGHT COLUMN (40%):
├── Hero Image/Video: Product mockup, course preview, or founder image
│   └── Style: Slight rotation (-3deg), drop shadow, or device frame
└── Floating Elements (optional): Testimonial snippet, student count badge
    └── Style: Glass morphism card, positioned absolute
```

### Spacing Guidelines
- Section padding: 80px top, 120px bottom (desktop) / 60px all (mobile)
- Element spacing: 24px between headline elements
- CTA margin-top: 32px from last content element

### Mobile Behavior
- Stack columns (image moves above or below content based on preference)
- Headline: 32-40px
- Full-width CTA button
- Hide floating elements or reposition below main content

### Example FG Funnels Settings
```
Block Type: Hero with Media
Layout: Split (Left Text, Right Image)
Background: Image with overlay OR Gradient
Padding: Custom (80px 5% 120px 5%)
Max Width: 1200px centered
```

---

## 2. Credibility Section Layout

### Purpose
Build trust immediately after the hero by showcasing authority markers, social proof, and "why me" positioning.

### FG Funnels Block Configuration

```
SECTION: Credibility Bar + Authority
├── Sub-section A: Logo Bar (optional)
│   ├── Container: Full-width, light gray or white background
│   ├── Headline: "As Featured In" or "Trusted By"
│   │   └── Style: 14px uppercase, centered, letter-spacing 2px, muted color
│   └── Logo Row: 4-6 logos
│       └── Style: Grayscale, 50% opacity, hover to full color, 60px height max
│       └── Spacing: Equal distribution with flex, gap 48px
│
├── Sub-section B: Founder/Expert Introduction
│   ├── Container: 2-column grid (40/60 or 50/50)
│   ├── LEFT: Founder Image
│   │   └── Style: Circular or rounded rectangle, border accent color, slight shadow
│   │   └── Size: 300-400px width
│   ├── RIGHT: Bio Content
│   │   ├── Eyebrow: "Meet Your [Coach/Instructor/Guide]"
│   │   │   └── Style: 14px uppercase, {brand_color_primary}
│   │   ├── Name: H2
│   │   │   └── Style: 36-42px, bold
│   │   ├── Credentials: Short list of achievements
│   │   │   └── Style: Inline badges or comma-separated, 16px
│   │   ├── Story Paragraph: 2-3 sentences, relatable transformation
│   │   │   └── Style: 18px, line-height 1.7, max-width 550px
│   │   └── Proof Points: Icon + stat grid
│   │       └── Layout: 3-column mini-grid
│   │       └── Format: Large number + descriptor (e.g., "10K+" / "Students Trained")
│
└── Sub-section C: Quick Stats Bar (optional)
    ├── Container: Full-width accent background
    └── Stats: 3-4 key numbers
        └── Layout: Horizontal flexbox, evenly spaced
        └── Style: Large numbers (48px), small labels (14px), centered
```

### Spacing Guidelines
- Logo bar: 40px padding vertical
- Founder section: 80px padding vertical
- Stats bar: 48px padding vertical
- Between sub-sections: No gap (seamless flow)

### Mobile Behavior
- Logo bar: 2 rows of logos or horizontal scroll
- Founder: Stack image above bio, center-aligned
- Stats: 2x2 grid or vertical stack

### Example FG Funnels Settings
```
Block Type: Content with Image
Layout: Side by Side
Background: White or Light Gray (#F9FAFB)
Stats Block Type: Counter/Stats Row
Animation: Fade in on scroll (optional)
```

---

## 3. Program Breakdown Layout

### Purpose
Show exactly what's included with clear visual hierarchy. Transform features into benefits and make the value stack irresistible.

### FG Funnels Block Configuration

```
SECTION: Program Breakdown
├── Section Header
│   ├── Eyebrow: "What's Inside" or "The Complete Curriculum"
│   │   └── Style: 14px uppercase, {brand_color_primary}, centered
│   ├── Headline: H2
│   │   └── Style: 36-48px, bold, centered, max-width 700px
│   └── Subtext: Brief description of transformation journey
│       └── Style: 18px, muted, centered, max-width 600px
│
├── Module Grid: Main curriculum display
│   ├── Layout Option A: Accordion Style
│   │   ├── Container: Max-width 800px, centered
│   │   ├── Each Module:
│   │   │   ├── Header Row: Module # + Title + Expand Icon
│   │   │   │   └── Style: 20px bold, padding 24px, border-bottom
│   │   │   └── Expanded Content: Lesson list, outcomes
│   │   │       └── Style: Bulleted list, 16px, indented 24px
│   │   └── Active State: {brand_color_primary} left border, light bg
│   │
│   ├── Layout Option B: Card Grid
│   │   ├── Grid: 2 or 3 columns
│   │   ├── Each Card:
│   │   │   ├── Module Number: Circle badge, top-left
│   │   │   │   └── Style: {brand_color_primary} bg, white text, 40px
│   │   │   ├── Title: H3
│   │   │   │   └── Style: 22px bold
│   │   │   ├── Description: What they'll learn
│   │   │   │   └── Style: 16px, muted, 3-4 lines max
│   │   │   └── Lesson Count: "X Lessons" pill
│   │   │       └── Style: Small pill badge, secondary color
│   │   └── Card Style: White bg, subtle shadow, rounded 12px, hover lift
│   │
│   └── Layout Option C: Timeline/Roadmap
│       ├── Container: Vertical line (center or left-aligned)
│       ├── Each Node:
│       │   ├── Circle Marker: On the line
│       │   │   └── Style: {brand_color_primary}, 16px diameter
│       │   ├── Content Card: Offset from line
│       │   │   └── Alternating left/right on desktop
│       │   └── Week/Phase Label: Above title
│       └── Connector: Dashed or solid line, muted color
│
├── Bonus Stack (below modules)
│   ├── Header: "Plus These Exclusive Bonuses"
│   │   └── Style: 28px, centered, with decorative line
│   ├── Bonus Cards: Horizontal scroll or grid
│   │   ├── Each Bonus:
│   │   │   ├── Image/Icon: Visual representation
│   │   │   ├── Title: Bonus name
│   │   │   ├── Value: "Value: $XXX" (struck through optional)
│   │   │   └── Description: 1-2 sentences
│   │   └── Style: Accent border or ribbon "BONUS" tag
│   └── Total Value: Sum statement
│       └── Style: 24px, bold, centered
│
└── CTA Block: Mid-page conversion point
    ├── Container: Accent background or gradient
    ├── Text: Urgency/scarcity message
    └── Button: Same style as hero CTA
```

### Spacing Guidelines
- Section header to grid: 48px
- Between modules/cards: 24px
- Bonus section margin-top: 64px
- CTA block padding: 64px vertical

### Mobile Behavior
- Card grid: Single column
- Accordion: Full-width, same functionality
- Timeline: Left-aligned only, no alternating
- Horizontal scroll for bonus cards with snap points

### Example FG Funnels Settings
```
Block Type: Feature List or Content Boxes
Layout: Grid (2-3 columns) or Accordion
Background: Light gray or white with subtle pattern
Card Style: Shadow, Rounded
Animation: Stagger fade-in on scroll
```

---

## 4. Testimonials Section Layout

### Purpose
Provide social proof through diverse, specific success stories. Build "people like me" identification.

### FG Funnels Block Configuration

```
SECTION: Testimonials
├── Section Header
│   ├── Eyebrow: "Success Stories" or "What Students Say"
│   │   └── Style: 14px uppercase, {brand_color_primary}
│   ├── Headline: H2
│   │   └── Style: 36-48px, bold, centered
│   └── Subtext: Highlight transformation pattern
│       └── Style: 18px, muted, centered
│
├── Layout Option A: Masonry Grid (Best for volume)
│   ├── Grid: 3 columns desktop, 2 tablet, 1 mobile
│   ├── Each Testimonial Card:
│   │   ├── Quote Icon: Top-left decorative
│   │   │   └── Style: Large, muted {brand_color_primary}, 20% opacity
│   │   ├── Testimonial Text: The quote
│   │   │   └── Style: 16-18px, italic optional, line-height 1.6
│   │   ├── Result Highlight: Specific outcome (bold or highlighted)
│   │   │   └── Style: Inline bold or {brand_color_primary} text
│   │   ├── Divider: Thin line
│   │   ├── Avatar: Circular photo
│   │   │   └── Style: 48px, border, positioned left
│   │   ├── Name: Full name
│   │   │   └── Style: 16px bold
│   │   └── Context: Role/location/niche
│   │       └── Style: 14px muted
│   └── Card Styling: White bg, soft shadow, rounded 16px, varied heights
│
├── Layout Option B: Featured Carousel (Best for video/long-form)
│   ├── Container: Full-width with overflow hidden
│   ├── Main Display: Large featured testimonial
│   │   ├── If Video: Embedded player with custom thumbnail
│   │   │   └── Style: 16:9 aspect, rounded, play button overlay
│   │   ├── If Text: Large quote display
│   │   │   └── Style: 24px, max-width 800px, centered
│   │   └── Attribution: Below media/quote
│   ├── Navigation: Dots or thumbnail strip
│   │   └── Style: Below main content, 16px from bottom
│   └── Arrows: Left/right navigation
│       └── Style: Circular buttons, subtle shadow, edge-positioned
│
├── Layout Option C: Two-Column Highlight (Best for transformation stories)
│   ├── Grid: 2 columns, alternating image/content sides
│   ├── Each Story:
│   │   ├── Image Column: Before/after or success photo
│   │   │   └── Style: Full column height, object-fit cover
│   │   ├── Content Column:
│   │   │   ├── "Before" State: Pain point description
│   │   │   │   └── Style: Muted text, crossed out or faded
│   │   │   ├── "After" State: Transformation achieved
│   │   │   │   └── Style: Bold, {brand_color_primary}
│   │   │   ├── Full Quote: Their words
│   │   │   └── Attribution: Name + context
│   │   └── Divider: Between stories if stacked
│
├── Social Proof Bar (optional, below testimonials)
│   ├── Container: Accent background
│   └── Elements: Review count, star rating, platform badges
│       └── Style: Horizontal layout, centered
│       └── Example: "⭐ 4.9 average from 500+ reviews"
│
└── Trust Elements
    ├── Verification Badge: "Verified Purchase" or platform logo
    └── Date: "Posted [Month Year]" for recency
```

### Spacing Guidelines
- Section header to testimonials: 48px
- Between testimonial cards: 24px (grid gap)
- Social proof bar: 48px margin-top
- Section padding: 80px vertical

### Mobile Behavior
- Masonry becomes single column
- Carousel maintains swipe functionality
- Two-column becomes stacked
- Reduce quote font size to 16px

### Example FG Funnels Settings
```
Block Type: Testimonials
Layout: Grid, Carousel, or Cards
Background: Light gray (#F3F4F6) or subtle gradient
Card Style: White with shadow
Animation: Fade-in stagger or slide-in from bottom
```

---

## 5. FAQ Section Layout

### Purpose
Overcome objections, reduce support load, and provide final reassurance before purchase decision.

### FG Funnels Block Configuration

```
SECTION: FAQ
├── Section Header
│   ├── Eyebrow: "Got Questions?"
│   │   └── Style: 14px uppercase, {brand_color_primary}
│   ├── Headline: "Frequently Asked Questions"
│   │   └── Style: 36-42px, bold, centered
│   └── Subtext: "Everything you need to know before joining"
│       └── Style: 18px, muted, centered
│
├── FAQ Container
│   ├── Layout: Centered, max-width 800px
│   ├── Style: Clean, minimal, focus on readability
│   │
│   ├── Layout Option A: Classic Accordion
│   │   ├── Each FAQ Item:
│   │   │   ├── Question Row (clickable):
│   │   │   │   ├── Question Text: H3 or strong paragraph
│   │   │   │   │   └── Style: 18-20px, semi-bold, left-aligned
│   │   │   │   └── Toggle Icon: Plus/minus or chevron
│   │   │   │       └── Style: Right-aligned, transitions on open
│   │   │   ├── Answer Panel (collapsible):
│   │   │   │   └── Style: 16px, line-height 1.7, padding 16px 0
│   │   │   │   └── May include: Links, bold text, bullet lists
│   │   │   └── Divider: Thin border-bottom between items
│   │   └── States:
│   │       ├── Closed: Icon rotated 0deg
│   │       ├── Open: Icon rotated 45deg (plus) or 180deg (chevron)
│   │       └── Hover: Slight background tint
│   │
│   ├── Layout Option B: Two-Column Grid (for many FAQs)
│   │   ├── Grid: 2 columns desktop, 1 mobile
│   │   ├── Each FAQ Card:
│   │   │   ├── Question: Bold header
│   │   │   │   └── Style: 18px bold, margin-bottom 8px
│   │   │   └── Answer: Always visible
│   │   │       └── Style: 16px, muted slightly
│   │   └── Card Style: No border, or subtle left border accent
│   │
│   └── Layout Option C: Tabbed Categories (for complex products)
│       ├── Tab Row: Category labels
│       │   └── Categories: "About the Program", "Payment", "Access", "Support"
│       │   └── Style: Horizontal tabs, active state underline
│       └── Tab Content: Accordion within each tab
│
├── FAQ Organization (recommended groupings)
│   ├── Category 1: About the Product/Program
│   │   └── What's included, who it's for, format, timeline
│   ├── Category 2: Investment & Payment
│   │   └── Price, payment plans, refund policy
│   ├── Category 3: Access & Delivery
│   │   └── How to access, tech requirements, start date
│   ├── Category 4: Support & Guarantee
│   │   └── Help available, guarantee details, contact
│   └── Category 5: Results & Expectations
│       └── Typical results, time commitment, prerequisites
│
├── Still Have Questions? Block
│   ├── Container: Centered below FAQ
│   ├── Text: "Still have questions? We're here to help."
│   │   └── Style: 18px, centered
│   └── Options:
│       ├── Contact Link: "Email us at [support email]"
│       ├── Chat Widget: "Chat with us" button
│       └── Calendar Link: "Book a quick call"
│       └── Style: Text link or small secondary button
│
└── Final CTA Block
    ├── Container: Full-width accent background
    ├── Headline: Urgency statement
    │   └── Example: "Ready to Transform Your [Outcome]?"
    │   └── Style: 32px, bold, white text
    ├── Subtext: Scarcity or guarantee reminder
    │   └── Style: 18px, white 80% opacity
    ├── CTA Button: Primary conversion button
    │   └── Style: Large, contrasting color (white or light)
    └── Trust Line: Guarantee badge + "Cancel anytime" or similar
        └── Style: Small text below button, icons optional
```

### Spacing Guidelines
- Section header to FAQ: 48px
- Between FAQ items: 0 (dividers separate)
- FAQ to "Still Questions" block: 48px
- Final CTA section padding: 80px vertical

### Mobile Behavior
- Full-width accordion
- Larger touch targets (minimum 48px height for questions)
- Two-column grid becomes single column
- Tabs become dropdown or vertical stack

### Example FG Funnels Settings
```
Block Type: FAQ Accordion
Layout: Centered, max-width container
Background: White or very light gray
Icon Style: Plus/Minus or Chevron
Animation: Smooth expand/collapse (300ms ease)
```

---

## Complete Page Flow Reference

### Recommended Section Order
```
1. HERO SECTION
   └── Hook, promise, primary CTA

2. CREDIBILITY SECTION
   └── Logos → Founder intro → Quick stats

3. PROBLEM AGITATION (optional)
   └── Pain points, "sound familiar?" content

4. PROGRAM BREAKDOWN
   └── Curriculum → Bonuses → Value stack → Mid-page CTA

5. TESTIMONIALS
   └── Social proof variety → Platform badges

6. FAQ SECTION
   └── Objection handling → Support options → Final CTA

7. FOOTER CTA (sticky optional)
   └── Last-chance conversion bar
```

### Global Styling Tokens for FG Funnels

```css
/* Typography Scale */
--heading-xl: 48-64px  /* Hero headlines */
--heading-lg: 36-42px  /* Section headlines */
--heading-md: 24-28px  /* Subsection headlines */
--heading-sm: 18-22px  /* Card titles, FAQ questions */
--body-lg: 18-20px     /* Subheadlines, featured text */
--body-md: 16px        /* Standard body copy */
--body-sm: 14px        /* Captions, eyebrows */
--body-xs: 12px        /* Badges, fine print */

/* Spacing Scale */
--section-padding: 80px (desktop) / 48px (mobile)
--container-max: 1200px
--content-max: 800px
--element-gap-lg: 48px
--element-gap-md: 24px
--element-gap-sm: 16px

/* Animation Tokens */
--transition-fast: 150ms ease
--transition-base: 300ms ease
--transition-slow: 500ms ease

/* Shadow Scale */
--shadow-sm: 0 1px 2px rgba(0,0,0,0.05)
--shadow-md: 0 4px 6px rgba(0,0,0,0.07)
--shadow-lg: 0 10px 15px rgba(0,0,0,0.1)
--shadow-xl: 0 20px 25px rgba(0,0,0,0.15)
```

---

## FG Funnels Implementation Checklist

### Before Building
- [ ] Gather all brand assets (colors, fonts, logo)
- [ ] Collect testimonials with photos and specific results
- [ ] Write all copy following reference site structure
- [ ] Prepare images (hero, founder, product mockups)
- [ ] Define primary and secondary CTAs

### During Build
- [ ] Start with mobile layout, then expand to desktop
- [ ] Test all interactive elements (accordions, carousels)
- [ ] Verify CTA buttons are prominent and consistent
- [ ] Check spacing consistency between sections
- [ ] Ensure images are optimized (<200KB per image)

### After Building
- [ ] Preview on multiple devices and browsers
- [ ] Test all links and form submissions
- [ ] Verify load speed (<3 seconds)
- [ ] A/B test headline and CTA variations
- [ ] Connect analytics and conversion tracking

---

## Example Usage

**Input Variables:**
```
{brand_color_primary} = "#7C3AED" (purple)
{brand_color_secondary} = "#DDD6FE" (light purple)
{logo_url} = "/assets/logo.svg"
{hero_image_url} = "/assets/hero-course-mockup.png"
{program_name} = "Automation Accelerator"
{price} = "$997"
{cta_text} = "Enroll Now & Get Instant Access"
```

**Sample Hero Configuration:**
```
FG Funnels Block: Hero Split Layout
├── Background: Linear gradient (#7C3AED → #5B21B6)
├── Left Column:
│   ├── Badge: "LIMITED SPOTS AVAILABLE"
│   ├── H1: "Build Your First Profitable Automation in 30 Days"
│   ├── Subheadline: "The step-by-step system for freelancers ready to scale"
│   ├── Bullets: ✓ No coding required ✓ Done-with-you templates ✓ Lifetime access
│   ├── CTA: [Enroll Now & Get Instant Access] (white button)
│   └── Trust: 🔒 Secure checkout • 30-day guarantee • 500+ enrolled
└── Right Column:
    └── Course mockup image with floating "4.9 ⭐" badge
```
