# Professional Portfolio Website Template

A modern, minimal, and visually focused portfolio template built with **HTML, CSS, and vanilla JavaScript**.

## Project Structure

```text
/
├── index.html
├── assets/
│   ├── css/
│   │   └── style.css
│   ├── js/
│   │   └── main.js
│   └── img/
│       ├── profile.svg
│       └── project-1.svg ... project-8.svg
└── README.md
```

## How to Add New Projects

1. Open `index.html` and locate the `#projects` section.
2. Duplicate one `.project-card` block.
3. Update:
   - `img src` to the new image path in `assets/img/`
   - `alt` text (describe the image clearly)
   - Category, title, and description text.
4. Keep total projects between 6 and 12 for best layout balance.

## How to Change Portfolio Data

Edit content directly in `index.html`:

- **Name / brand**: header brand text, hero heading, footer.
- **Role and value statement**: hero section.
- **Services**: cards inside `#services`.
- **About details**: biography, experience, and skills in `#about`.
- **Testimonials**: testimonial cards section.
- **Contact info**: email and WhatsApp links in `#contact`.

## How to Update Images

1. Add optimized images to `assets/img/`.
2. Replace current file names in `index.html` with your own.
3. Recommended image approach:
   - Project images: similar dimensions for consistent cards (e.g. 1200×800).
   - Profile image: square ratio (e.g. 800×800).
4. Always keep meaningful `alt` text for accessibility and SEO.

## How to Change Colors

Open `assets/css/style.css` and edit the variables in `:root`:

- `--color-primary`
- `--color-secondary`
- `--color-accent`
- `--color-bg`
- `--color-text`
- `--color-muted`

Only these six variables are used in the design system.

## How Contact Form Works (No Backend)

The form in `#contact` is handled by `assets/js/main.js`.

On submit, JavaScript creates a pre-filled `mailto:` link with:

- Name
- Email
- Message

This opens the user’s default email client, so no backend is required.

## Deploy to GitHub Pages

1. Push this project to a GitHub repository.
2. In GitHub, open **Settings → Pages**.
3. Under **Build and deployment**:
   - Source: **Deploy from a branch**
   - Branch: choose `main` (or your default branch), folder `/ (root)`
4. Save settings and wait for deployment.
5. GitHub will provide your live Pages URL.

## Performance & Accessibility Notes

- Uses semantic HTML structure and one `<h1>`.
- Includes Open Graph and meta description tags.
- Uses lazy-loaded project images.
- Honors `prefers-reduced-motion`.
- Includes visible keyboard focus styles and a skip link.
