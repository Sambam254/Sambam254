# CareerBoost Order Flow Documentation

This directory contains the functional order intake flow for the CareerBoost service.

## The Flow
1. **Landing Page:** Customer clicks "Get Started" or "Choose" on the main landing page.
2. **Order Intake (`order.html`):**
    - Customer fills out the intake form (Name, Email, Service, Job Title, Links to current resume/LinkedIn).
3. **Submission:** Customer submits the form (sent via FormSubmit.co to careerboost.service@gmail.com).
4. **Confirmation (`confirmation.html`):** Customer sees a "Thank You" page and is instructed that a payment link will be sent to their email.
5. **Payment:** Specialist reviews the intake and sends a PayPal/Venmo link to the customer.

## Implementation Details
- **Styling:** Uses Tailwind CSS via CDN for a modern, responsive look consistent with the main site.
- **Form Handling:** The form is connected to **FormSubmit.co**, which sends submissions directly to `careerboost.service@gmail.com`.
- **Redirects:** After submission, FormSubmit.co redirects the user to the `confirmation.html` page.

## Delivery Process (Internal)
1. Receive PayPal notification of payment.
2. Receive form submission (Email/Backend).
3. Resume Specialist starts work.
4. Deliver via email to the address provided in the form.

## Files
- `order.html`: The main checkout and intake page.
- `confirmation.html`: The thank-you page after submission.
