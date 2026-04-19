# Minimal Test Plan

## Functional smoke tests
- Open each main tool and confirm render without errors.
- Generate at least one output in: Adapt, Hashtag, Caption, Video Script, Ads.
- Validate copy-to-clipboard actions where available.

## Accessibility checks
- Navigate with keyboard only (`Tab`, `Shift+Tab`, `Enter`, `Esc`).
- Confirm visible focus ring on interactive controls.
- Confirm skip link focuses main content.
- Confirm icon-only buttons expose labels to assistive tech.

## SEO/share checks
- Validate `meta description` exists.
- Validate Open Graph tags (`title`, `description`, `image`, `url`).
- Validate JSON-LD parses as `SoftwareApplication`.
- Validate favicon and theme-color in browser.

## Responsive checks
- Desktop width ≥ 1280px.
- Tablet width around 768px.
- Mobile width around 390px: sidebar toggles and closes on `Esc`.
