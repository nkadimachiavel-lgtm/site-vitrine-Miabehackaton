---
name: LokalPay Congo Design System
colors:
  surface: '#f7f9fc'
  surface-dim: '#d8dadd'
  surface-bright: '#f7f9fc'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f2f4f7'
  surface-container: '#eceef1'
  surface-container-high: '#e6e8eb'
  surface-container-highest: '#e0e3e6'
  on-surface: '#191c1e'
  on-surface-variant: '#42474e'
  inverse-surface: '#2d3133'
  inverse-on-surface: '#eff1f4'
  outline: '#72777f'
  outline-variant: '#c2c7cf'
  surface-tint: '#386188'
  primary: '#002743'
  on-primary: '#ffffff'
  primary-container: '#0a3d62'
  on-primary-container: '#80a8d3'
  inverse-primary: '#a2caf7'
  secondary: '#7c5800'
  on-secondary: '#ffffff'
  secondary-container: '#fdbf41'
  on-secondary-container: '#6f4e00'
  tertiary: '#002b12'
  on-tertiary: '#ffffff'
  tertiary-container: '#004420'
  on-tertiary-container: '#38ba6b'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#cfe5ff'
  primary-fixed-dim: '#a2caf7'
  on-primary-fixed: '#001d34'
  on-primary-fixed-variant: '#1d496f'
  secondary-fixed: '#ffdea7'
  secondary-fixed-dim: '#fabc3e'
  on-secondary-fixed: '#271900'
  on-secondary-fixed-variant: '#5e4200'
  tertiary-fixed: '#7efba4'
  tertiary-fixed-dim: '#61de8a'
  on-tertiary-fixed: '#00210c'
  on-tertiary-fixed-variant: '#005228'
  background: '#f7f9fc'
  on-background: '#191c1e'
  surface-variant: '#e0e3e6'
typography:
  h1:
    fontFamily: Inter
    fontSize: 28px
    fontWeight: '700'
    lineHeight: 34px
    letterSpacing: -0.02em
  h2:
    fontFamily: Inter
    fontSize: 22px
    fontWeight: '600'
    lineHeight: 28px
    letterSpacing: -0.01em
  h3:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '600'
    lineHeight: 24px
    letterSpacing: 0em
  body-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
    letterSpacing: 0em
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
    letterSpacing: 0em
  label-caps:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '700'
    lineHeight: 16px
    letterSpacing: 0.05em
  reputation-score:
    fontFamily: Inter
    fontSize: 48px
    fontWeight: '800'
    lineHeight: 48px
    letterSpacing: -0.04em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  base: 4px
  xs: 8px
  sm: 12px
  md: 16px
  lg: 24px
  xl: 32px
  container-padding: 20px
  stack-gap: 16px
---

## Brand & Style

The design system is anchored in the concept of "Digital Integrity for the Local Market." It bridges the gap between traditional informal commerce in Brazzaville and the high-security world of blockchain technology. The personality is **Reliable**, **Empowering**, and **Transparent**.

The chosen style is **Modern Corporate Minimalism** with a mobile-first priority. It avoids unnecessary decorative elements to focus on clarity and speed of use in active market environments. High white space is utilized to reduce cognitive load for merchants who may be multitasking. Visual cues emphasize security through structural stability and clean, geometric precision, ensuring the platform feels like a professional financial tool rather than a speculative asset.

## Colors

This design system uses a palette rooted in trust and growth. 
- **Primary (#0a3d62):** A deep, institutional blue used for headers, primary actions, and branding to convey stability and security.
- **Accent/CTA (#f6b93b):** A vibrant yellow used sparingly for critical calls to action. It provides high contrast against the dark blue and ensures merchants can quickly identify "Pay" or "Confirm" buttons in outdoor lighting.
- **Success/Score (#27ae60):** A lush green used specifically for reputation scores and successful transaction states, symbolizing growth and positive standing.
- **Background (#f5f7fa):** A cool, light grey that provides a soft canvas, reducing screen glare during outdoor use.

## Typography

This design system utilizes **Inter** for its exceptional legibility on mobile screens and its neutral, functional character. 

Hierarchy is established through weight and scale. The `reputation-score` style is a specialized display face used solely for the merchant's blockchain credit score, making it the most prominent element on the dashboard. Body copy is set at a minimum of 14px to ensure readability in varying light conditions. All labels for data points (e.g., transaction IDs) use `label-caps` for clear categorization.

## Layout & Spacing

The layout philosophy follows a **Fluid Grid** model optimized for narrow mobile viewports. A standard 4-column grid is used for mobile, with 20px outer margins and 16px gutters.

Spacing follows a 4px baseline shift. In this design system, "High White Space" means generous vertical padding between sections (using `xl` spacing) to prevent the UI from feeling cluttered with financial data. Groups of related items (like transaction history lists) use `sm` spacing, while distinct sections of a merchant profile use `lg` spacing.

## Elevation & Depth

Visual hierarchy is achieved through **Tonal Layers** and **Ambient Shadows**. 

1.  **Base Layer:** The background is `#f5f7fa`.
2.  **Surface Layer:** Cards and containers are pure `#ffffff` with a very soft, high-diffusion shadow (`Y: 4px, Blur: 20px, Color: #0a3d62 at 5% opacity`). 
3.  **Active Layer:** Floating Action Buttons (FABs) or primary modals use a slightly more pronounced shadow to indicate interactability.

This subtle depth creates a clear distinction between the canvas and interactive elements without the visual noise of heavy borders or skeuomorphism.

## Shapes

The design system adopts a **Rounded** shape language. Standard UI elements like cards and input fields use a 0.5rem (8px) radius. Larger containers or merchant profile headers use the `rounded-lg` (16px) or `rounded-xl` (24px) variants to feel more approachable and modern.

Buttons are fully pill-shaped (rounded-full) to provide a distinct tactile affordance that separates them from data containers. This softness balances the "hard" nature of blockchain tech, making the application feel more human and accessible.

## Components

### Buttons
- **Primary:** Pill-shaped, Primary Blue background, White text. High-emphasis.
- **Secondary/CTA:** Pill-shaped, Accent Yellow background, Primary Blue text. Reserved for the "Primary Action" of the screen (e.g., *Accept Payment*).
- **Ghost:** Primary Blue text, no background, used for secondary actions like "View Details."

### Cards
Cards are the primary container for merchant data. They feature 16px internal padding, white backgrounds, and subtle ambient shadows. Every card should have a clear "Title" and "Action" area.

### Reputation Score Badge
A specialized component: a large circular or rounded-rect element featuring the `reputation-score` typography and the Success Green color. It should be accompanied by a "Verified" icon to reinforce blockchain security.

### Input Fields
Inputs use a light grey border (1px) that turns Primary Blue on focus. Labels are always visible above the field (never just placeholder text) to ensure clarity for users who may be less tech-savvy.

### Chips
Used for transaction status (e.g., "Pending," "Verified"). These are small, low-contrast pills using 10% opacity of the status color for the background and 100% opacity for the text.

### Clean Icons
Icons must be 24px stroke-based (2px width), using the Primary Blue color. They should be literal and avoid abstract metaphors to remain accessible to market merchants.