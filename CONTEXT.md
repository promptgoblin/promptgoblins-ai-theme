# Prompt Goblins Discourse Theme - Project Context

## Overview
Custom Discourse theme for **Prompt Goblins** - an AI engineering blog/forum run by Mike. The goal is a unique, tasteful, modern design that stands out while remaining clean and readable.

## Brand Identity

### Logo Options
- **Goblin Mode (Light)**: Silly goblin with tongue out, energetic vibe (new-logo-option-3)
- **Chill Mode (Dark)**: Relaxed goblin with reflective glasses, calm smirk (new-logo-option-2)
- Logos feature an illustrated goblin in a hoodie at a retro computer with ">>> PROMPT GOBLINS" text

### Theme Concept
- **Light Mode = "Goblin Mode"**: Fun, energetic, playful - the chaotic default
- **Dark Mode = "Chill Mode"**: Relaxed, focused reading - late night calm vibes
- This flips the typical expectation (light=boring, dark=edgy)

## Color Palette

### Goblin Mode (Light)
From mockup at forum-palette.lovable.app:
- Background: Off-white / concrete beige (NOT too yellow - more gray)
- Cards/Content sections: White or slightly lighter
- Primary accent: Pistachio green `#93C572`
- Secondary accent: Cyan/teal `#3DBFBF`
- Text: Dark charcoal `#2D2D2D`
- Should have pops of color, vibrant but not overwhelming

### Chill Mode (Dark)
From mockup:
- Background: Deep indigo `#1A1B2E` (NOT gray - indigo/blue)
- Cards/Content: Slightly lighter indigo `#252640`
- Primary accent: Pistachio `#93C572` (same as light)
- Secondary accent: Muted teal `#5FAAAA`
- Text: Soft white `#E8E8EC`

## Design Requirements

### Typography
- Terminal vibes but VERY readable
- Modern courier-type font, not dated
- Space Grotesk was tried but not readable enough
- Need something that feels terminal/tech but is easy on the eyes

### Layout
- Standard Discourse layout with sidebar
- Logo should be directly above sidebar when open
- Sidebar background should NOT show behind main content when closed
- Main content area needs distinct background from page background
- All content sections (posts, cards) should have consistent different background

### Visual Style
- Modern, crisp, clean
- Rounded corners (8-12px)
- Subtle shadows for depth
- Good contrast throughout (check all text/background combinations)
- Check hover states for readability
- Remove pointless gradients (topic list had transparent gradient at bottom)

### Mode Toggle
- Should say "Chill Mode 🌙" when in light mode (click to activate dark)
- Should say "Goblin Mode ☀️" when in dark mode (click to activate light)
- Use modern icons, not default Discourse ones

## Outstanding Issues (from last session)

1. **Font**: Current font not readable enough - need modern terminal font
2. **Logo size**: Should be 2x bigger on desktop (100px height was set but not showing)
3. **Gradient**: Remove pointless gradient in topic list
4. **Backgrounds**: Content sections need consistent different background from main bg
5. **Contrast**: Audit all text/background combos including hover states
6. **Light mode beige**: Too yellow - make it more concrete/gray but lighter
7. **Sidebar**: Background bleeds behind content when closed
8. **Logo alignment**: Should align directly above sidebar when open
9. **Mode toggle**: Needs custom text (Goblin/Chill) and modern icons
10. **Goblin mode vibrancy**: Needs more pops of color while staying comfortable
11. **Dark mode colors**: Gray doesn't work with blue - use indigo from mockup
12. **Modernization**: All elements (buttons, outlines, etc.) need modern touches

## File Structure
```
prompt-goblins-theme/
├── about.json              # Theme metadata and color schemes
├── settings.yml            # Configurable theme settings
├── common/
│   ├── common.scss         # Shared styles
│   ├── head_tag.html       # Font imports
│   └── after_header.html   # Custom scripts
├── desktop/
│   └── desktop.scss        # Desktop-specific styles
├── mobile/
│   └── mobile.scss         # Mobile-specific styles
├── locales/
│   └── en.yml              # Translations
├── assets/                 # Theme assets
├── discourse-logos/        # Optimized logos for Discourse settings
│   ├── logo-light.png      # Main logo for Goblin Mode
│   ├── logo-dark.png       # Main logo for Chill Mode
│   ├── logo-small-*.png    # Small/square versions
│   └── mobile-logo-*.png   # Mobile versions
└── reference-images/       # Mockups and logo options
```

## GitHub Repository
`git@github.com:promptgoblin/promptgoblins-ai-theme.git`

## Live Site
https://promptgoblins.ai

## Mockup Reference
Originally at forum-palette.lovable.app (now private)
Screenshots saved in reference-images/ folder

## Technical Notes
- Theme installed via GitHub URL in Discourse Admin
- Update by pushing to GitHub, then clicking "Update" in Discourse theme settings
- Color schemes defined in about.json
- Logo uploads done in Admin > Settings > Branding (not in theme)
