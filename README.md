# CareerBoost Landing Page

This is a single-page, responsive landing page for the CareerBoost resume optimization service.

## Features
- **Hero Section:** Clear value proposition and CTA.
- **Pricing:** Three-tier pricing ($79, $49, $99).
- **Process:** Simple 3-step explanation of how the service works.
- **Testimonials:** Social proof placeholders.
- **Order Flow:** Ready to be linked to a Google Form or payment processor.
- **Responsive:** Optimized for mobile and desktop.
- **Framework:** Built with Tailwind CSS (via CDN) for easy customization.

## Deployment
1. **Host on GitHub Pages:**
   - Create a new repository named `careerboost-web`.
   - Upload `index.html`.
   - Enable GitHub Pages in the repository settings.
2. **Order Flow Setup:**
   - Create a Google Form with fields for: Name, Email, Service Choice, Current Resume Upload.
   - Link the "Get Started" and "Choose" buttons to the Google Form URL.
   - Set up a PayPal/Stripe payment link and include it in the Google Form confirmation message or a follow-up email.

## Files
- `index.html`: The main landing page.
- `success.html`: Order confirmation page (redirect users here after form submission).
- `form-structure.md`: Recommended fields for Google Form.
- `payment-links.md`: Guide for payment integration.

## Customization
- **Colors:** You can change the primary/secondary colors in the `<script>` tag at the top of `index.html`.
- **Forms:** Replace the `#order` button links with your actual Google Form URL.
- **Testimonials:** Update the placeholders with real customer feedback once available.
