# Prompt Goblins Discourse Theme

A custom Discourse theme for the Prompt Goblins AI engineering community.

## Features

- **Two Color Schemes**:
  - **Goblin Mode** (light): Playful, energetic vibes with the silly goblin logo
  - **Chill Mode** (dark): Relaxed, focused reading with the chill goblin logo
- Clean, modern design with rounded corners
- Pistachio green accent color throughout
- Custom category colors
- Responsive mobile design
- Accessible focus states
- Smooth transitions (respects prefers-reduced-motion)

## Installation

### From GitHub

1. Go to **Admin > Customize > Themes**
2. Click **Install** and select **From a git repository**
3. Enter: `https://github.com/YOUR-USERNAME/prompt-goblins-theme`
4. Click **Install**

### Manual Upload

1. Download/clone this repository
2. Zip the theme folder
3. Go to **Admin > Customize > Themes**
4. Click **Install** and select **From your device**
5. Upload the zip file

## Setup After Installation

### 1. Set the Color Schemes

1. Go to **Admin > Customize > Colors**
2. You should see "Goblin Mode" and "Chill Mode" color schemes
3. Set "Goblin Mode" as the default light scheme
4. Set "Chill Mode" as the default dark scheme

### 2. Upload Logos

1. Go to **Admin > Settings > Branding**
2. Upload `assets/logo-goblin-mode.png` as the **logo**
3. Upload `assets/logo-chill-mode.png` as the **logo dark**
4. Optionally create and upload a favicon

### 3. Enable Dark Mode Toggle

1. Go to **Admin > Settings > User Preferences**
2. Search for "dark mode"
3. Ensure users can select their color scheme preference

## Customization

Theme settings are available at **Admin > Customize > Themes > Prompt Goblins > Settings**:

- Logo heights
- Primary/secondary accent colors
- Border radius
- Category colors
- Feature toggles

## Color Palette

### Goblin Mode (Light)
| Element | Color |
|---------|-------|
| Background | `#F5F5DC` |
| Cards | `#FFFFFF` |
| Text | `#2D2D2D` |
| Pistachio accent | `#93C572` |
| Cyan accent | `#3DBFBF` |

### Chill Mode (Dark)
| Element | Color |
|---------|-------|
| Background | `#1A1B2E` |
| Cards | `#252640` |
| Text | `#E8E8EC` |
| Pistachio accent | `#93C572` |
| Cyan accent | `#5FAAAA` |

## File Structure

```
prompt-goblins-theme/
├── about.json           # Theme metadata and color schemes
├── settings.yml         # Configurable theme settings
├── common/
│   └── common.scss      # Shared styles (both modes)
├── desktop/
│   └── desktop.scss     # Desktop-specific styles
├── mobile/
│   └── mobile.scss      # Mobile-specific styles
├── locales/
│   └── en.yml           # English translations
├── assets/
│   ├── logo-goblin-mode.png
│   └── logo-chill-mode.png
└── reference-images/    # Design mockups (not included in theme)
```

## License

MIT License - feel free to use and modify.
