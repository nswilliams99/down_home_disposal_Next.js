# Design Guidelines for Down Home Disposal Website

## Design Approach
**Reference-Based + Brand-Driven Approach**: This is a service-based business website where trust, clarity, and local authenticity are paramount. The design should reflect small-business professionalism with clean, accessible layouts prioritizing quick contact actions and service information.

## Brand Colors (User-Specified - MUST USE EXACTLY)
- Primary Blue: `#2563EB`
- Accent Red: `#DC2626`
- Accent Yellow: `#FBBF24`
- Background: White `#FFFFFF`
- Text: Dark Gray `#1F2937`
- Light Gray (backgrounds): `#F3F4F6`

## Typography
- **Headlines**: Bold, clean sans-serif (Inter or Poppins) - large, confident sizing
- **Body Text**: Regular weight, highly readable
- Clear hierarchy: Large hero headlines, prominent section titles, readable body copy
- Phone numbers should be oversized and button-styled for emphasis

## Layout System
- **Spacing**: Use Tailwind units of 4, 6, 8, 12, 16, 20, 24, 32 for consistent rhythm
- **Mobile-first responsive**: Stack to single column on mobile, expand to grids on desktop
- **Container widths**: Max-width containers (max-w-6xl) for content sections
- **Section padding**: Generous vertical spacing (py-16 to py-24) between sections

## Component Library

### Navigation Header
- Sticky/fixed top navigation with company name left, links right
- Mobile: Hamburger menu pattern
- Phone number prominently displayed in header (clickable tel: link)
- Clean, minimal design with subtle shadow/border bottom

### Hero Section (Home Page)
- **Large hero image**: Use provided truck image (`Down_Home_disposal truck Pic_1764016401259.webp`) as background
- Prominent headline with contrasting text over image
- Pricing callout prominently displayed
- Two CTAs: Primary "Call Now" button (tel: link) and secondary "View Service Areas" button
- **Critical**: Buttons on hero image must have blurred/translucent backgrounds for readability

### Feature Cards (3-column on desktop, stack mobile)
- Icon at top, bold title, descriptive text
- Equal height cards with subtle background (light gray)
- Icons: Use Font Awesome or Heroicons CDN for trash cart, calendar, dollar sign icons

### Schedule/Table Display
- Clean card or table layout for pickup days (Tuesday/Wednesday/Thursday)
- Easy to scan: Day name prominent, locations listed clearly beneath
- Consider card-based layout over traditional table for better mobile experience

### Call-to-Action Sections
- Large, button-styled phone number (tel: link)
- Email as clickable mailto: link
- Hours of operation clearly visible
- High contrast, impossible to miss

### Footer
- Multi-column on desktop (company info | navigation | contact)
- Single column stack on mobile
- Include "Website by Trash Joes" credit line
- All contact info clickable (tel: and mailto: links)

## Page-Specific Layouts

### Home Page Structure
1. Hero with truck image background
2. About section (2-column: text + supporting element on desktop)
3. Three-feature cards section (grid)
4. Holiday schedule (4 holidays in clean grid/card layout)
5. Contact CTA section (centered, prominent)

### Service Areas Page
- Intro paragraph explaining service scope
- Pickup schedule as prominent cards/sections by day
- Service details highlighted box/card
- "Not sure?" CTA section with contact buttons

### Privacy Policy Page
- Long-form content with clear section breaks
- Hierarchical headings (H2 for main sections, H3 for subsections)
- Readable line-length (max-w-3xl for text content)
- Contact section at bottom

## Images
- **Hero Image**: Use provided truck photo (`Down_Home_disposal truck Pic_1764016401259.webp`) as full-width hero background on home page
- Apply subtle dark overlay for text readability
- Ensure buttons have blurred backgrounds when placed over image

## Accessibility & UX
- All phone numbers MUST be `tel:` links: `tel:+19313092245`
- All emails MUST be `mailto:` links
- High contrast text (dark gray on white, white on primary blue)
- Touch-friendly button sizes (minimum 44px tap targets)
- Semantic HTML structure
- Alt text for all images

## Key Design Principles
- **Trust & Clarity**: Clean, professional, no-nonsense layouts
- **Action-Oriented**: Phone/email CTAs prominent throughout
- **Local Business Feel**: Friendly, approachable, not corporate
- **Mobile-First**: Most customers will call from mobile devices
- **Fast Loading**: Minimal animations, optimize images

## Animation Guidelines
- Minimal, purposeful animations only
- Subtle hover states on buttons/links
- No distracting scroll animations or parallax effects
- Focus on speed and performance