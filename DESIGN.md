---
name: Fresh Harvest Professional
colors:
  surface: '#f4fafd'
  surface-dim: '#d4dbdd'
  surface-bright: '#f4fafd'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#eef5f7'
  surface-container: '#e8eff1'
  surface-container-high: '#e2e9ec'
  surface-container-highest: '#dde4e6'
  on-surface: '#161d1f'
  on-surface-variant: '#414942'
  inverse-surface: '#2b3234'
  inverse-on-surface: '#ebf2f4'
  outline: '#717971'
  outline-variant: '#c1c9bf'
  surface-tint: '#366847'
  primary: '#00361a'
  on-primary: '#ffffff'
  primary-container: '#1a4d2e'
  on-primary-container: '#88bd95'
  inverse-primary: '#9dd3aa'
  secondary: '#8a5100'
  on-secondary: '#ffffff'
  secondary-container: '#fd9d27'
  on-secondary-container: '#673b00'
  tertiary: '#16341c'
  on-tertiary: '#ffffff'
  tertiary-container: '#2c4b31'
  on-tertiary-container: '#97ba99'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#b8f0c5'
  primary-fixed-dim: '#9dd3aa'
  on-primary-fixed: '#00210e'
  on-primary-fixed-variant: '#1d5031'
  secondary-fixed: '#ffdcbe'
  secondary-fixed-dim: '#ffb86f'
  on-secondary-fixed: '#2c1600'
  on-secondary-fixed-variant: '#693c00'
  tertiary-fixed: '#c8ecc8'
  tertiary-fixed-dim: '#acd0ad'
  on-tertiary-fixed: '#03210b'
  on-tertiary-fixed-variant: '#2f4e33'
  background: '#f4fafd'
  on-background: '#161d1f'
  surface-variant: '#dde4e6'
typography:
  display-lg:
    fontFamily: Montserrat
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Montserrat
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
  headline-lg-mobile:
    fontFamily: Montserrat
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  title-md:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '600'
    lineHeight: 24px
  body-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  body-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  label-bold:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '700'
    lineHeight: 16px
    letterSpacing: 0.05em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 48px
  gutter: 20px
  margin-mobile: 16px
  margin-desktop: 64px
---

## Brand & Style

The brand personality is rooted in the "Farm-to-Table Professional" aesthetic. It balances the organic, community-focused nature of a local grocery (Rancho) with the efficiency and reliability of a modern e-commerce platform (Flexível). The UI is designed to evoke a sense of freshness, organization, and effortless logistics.

The design style follows a **Corporate / Modern** approach with subtle **Tactile** hints. It uses ample whitespace to ensure clarity—crucial for data-heavy inventory lists—while employing soft shadows and organic color hits to maintain a friendly, approachable atmosphere for the everyday consumer.

- **Trustworthy:** Through structured grids and clear data visualization.
- **Vibrant:** Through the strategic use of high-saturation secondary accents.
- **Efficient:** Through optimized information density in product listings and admin views.

## Colors

The palette is anchored by a deep **Forest Green** representing growth and freshness, and a **Sun-Kissed Orange** used exclusively for action-oriented elements like "Add to Cart," "Checkout," and limited-time promotions. 

- **Primary (Dark Green):** Used for headers, primary navigation, and reinforcing brand presence.
- **Secondary (Orange):** The "Call to Action" color. It provides a high-contrast focal point against the green and white.
- **Neutral/Surface:** A clean, slightly cool gray scale prevents the UI from feeling "muddy" and ensures that product photography stands out.
- **Functional Colors:** Success (Green-Emerald), Error (Red-Coral), and Warning (Amber) should be used for system status messages.

## Typography

This system utilizes a dual-font strategy. **Montserrat** is used for headlines to provide a bold, geometric, and modern character that mirrors the logo's weight. **Inter** is used for all body text, UI labels, and data tables to ensure maximum legibility and a neutral, professional tone.

- **Hierarchy:** Use `title-md` for product names in cards and `body-sm` for secondary metadata like weight or SKU.
- **Case:** Use Uppercase for `label-bold` in category chips or small table headers to differentiate from interactive text.
- **Performance:** Inter's tall x-height makes it ideal for the small-print details found in grocery inventories and pricing.

## Layout & Spacing

The system is built on a rigorous **4px baseline grid**. 

- **Grid Model:** A 12-column fluid grid for desktop and a 4-column grid for mobile. 
- **Containers:** The max-width for content containers is 1280px. 
- **Admin Dashboard:** Uses a "No Grid" contextual layout for the sidebar but maintains a fixed 280px width, while the main content area remains fluid with consistent 32px padding (`lg` + `sm` units).
- **Reflow:** On mobile, product grids should transition from 4 columns to 2 columns to keep images large enough for visibility.

## Elevation & Depth

Visual hierarchy is managed through **Tonal Layers** and **Ambient Shadows**.

1.  **Level 0 (Background):** Solid `#F8F9FA`. Used for the main canvas.
2.  **Level 1 (Surface):** White cards with a very soft, diffused shadow (`0px 4px 12px rgba(0,0,0,0.05)`). Used for product cards and main content blocks.
3.  **Level 2 (Navigation/Floating):** Headers and the Shopping Cart Sidebar. These use a slightly more pronounced shadow or a subtle 1px border (`#E0E0E0`) to distinguish from the background.
4.  **Level 3 (Modals/Overlays):** High-elevation shadows with a 15% opacity tint of the primary color to give the depth a "natural" feel.

Avoid using heavy borders; rely on the subtle shift from background to surface color to define sections.

## Shapes

The shape language is consistently **Rounded**, reflecting the "Friendly/Modern" requirement.

- **Small elements (Checkboxes, inputs):** 8px radius (`rounded`).
- **Medium elements (Product cards, category chips):** 16px radius (`rounded-lg`).
- **Buttons:** 12px radius, striking a balance between a professional rectangle and a friendly pill.
- **Interactive States:** On hover, cards should lift slightly (increase shadow) rather than change shape.

## Components

### Product Cards
- **Structure:** Image (top), Title (Inter Semi-Bold), Weight/Unit (Inter Regular/Gray), Price (Montserrat Bold/Green), and a floating Orange "+" button at the bottom-right corner.
- **Interaction:** Entire card surface is clickable to view details, but the orange "+" button adds to cart instantly.

### Category Chips
- **Style:** Light Green background (`#E8F5E9`) with Dark Green text.
- **Active State:** Solid Dark Green background with White text.
- **Shape:** Full pill-shape (32px radius).

### Shopping Cart Sidebar
- **Style:** White surface, full height, right-aligned. 
- **Header:** Sticky header with "Your Basket" and a close icon.
- **Footer:** Fixed total price and "Checkout" button in secondary Orange.

### Admin Forms
- **Inputs:** 1px border in Light Gray, turning Primary Green on focus.
- **Labels:** Positioned above the field in `label-bold` style.
- **Tables:** Use alternating row stripes (Zebra striping) in `#F8F9FA` for readability in long inventory lists.

### Professional Forms
- Use clear error states with red icons and helper text below the field.
- Primary buttons should be full-width on mobile to provide a large tap target.