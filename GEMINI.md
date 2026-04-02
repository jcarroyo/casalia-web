# Casalia Web Project Context

This project is a static website for **Casalia**, a home care agency that provides specialized services like childcare (nanas), cleaning/organization (hogar), and elderly care.

## Project Overview

- **Purpose:** A marketing landing page for Casalia agency.
- **Main Technologies:**
    - **HTML5:** Core structure of the landing page.
    - **CSS3:** Custom styles and design system tokens.
    - **Tailwind CSS:** Used via CDN for layout and utility-first styling.
    - **Google Fonts:** Uses *Plus Jakarta Sans* for headlines and *Manrope* for labels/text.
    - **Material Symbols:** Used for iconography.

## Architecture

The project is a simple static website consisting of:
- `index.html`: The main entry point containing the structure and section-based layout (Hero, Mission, Services, CTA, Footer).
- `style.css`: Defines the "Curated Sanctuary" design system, including color tokens, typography rules, and custom component styles (`.btn-primary`, `.card`, `.glass-header`).
- `images/`: Directory for local assets like `logo_casalia.png`.

## Running the Project

Since this is a pure static website, there is no build step required.

- **Development:** Open `index.html` directly in any modern web browser or use a simple development server like the "Live Server" extension in VS Code.
- **Deployment:** The project is ready for deployment to any static hosting service (Netlify, Vercel, GitHub Pages, etc.).

## Development Conventions

- **Design System:** Always adhere to the CSS variables defined in `:root` within `style.css` (e.g., `--primary`, `--secondary`, `--background`).
- **Tailwind Integration:** Tailwind is configured via a script tag in `index.html`. Any changes to the Tailwind theme should be made there.
- **Styling Strategy:**
    - Use Tailwind utility classes for layout, spacing, and responsive behavior.
    - Use custom CSS classes in `style.css` for complex components, animations, and specific design system effects (like glassmorphism or organic asymmetry).
- **Typography:** Headlines should use `Plus Jakarta Sans` with an "editorial" feel. Labels and secondary text use `Manrope`.
- **External Assets:** Most images are currently served from Google's CDN. Consider downloading and hosting them locally in the `images/` directory for production stability.
