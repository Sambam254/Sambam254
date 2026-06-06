# Setting up Payments

## 1. PayPal (Current Setup)
We are currently using PayPal for quick launch.
- **Link:** `https://www.paypal.me/careerboost`
- **Workflow:** Users are directed to this link after filling out the intake form.

## 2. Stripe Payment Links (Future Upgrade)
To upgrade to Stripe:
1. **Create Products in Stripe**
...
- Create a product: **Resume Rewrite** - $79.00
- Create a product: **LinkedIn Optimization** - $49.00
- Create a product: **The Career Bundle** - $99.00

## 2. Generate Payment Links
- Go to **More > Payment Links** in your Stripe Dashboard.
- Click "New" and select the corresponding product.
- Enable "Collect customers' addresses" and "Collect phone numbers" if needed.
- Copy the resulting URL (e.g., `https://buy.stripe.com/test_...`).

## 3. Update index.html
Replace the placeholder `#order` hrefs in `index.html` with your actual Stripe Payment Link URLs.

- **Resume:** `href="https://buy.stripe.com/..."`
- **LinkedIn:** `href="https://buy.stripe.com/..."`
- **Bundle:** `href="https://buy.stripe.com/..."`

## 4. Redirect After Payment
In Stripe Payment Link settings, set the "After payment" behavior to "Don't show confirmation page" and redirect them to your Google Form (if you want them to fill it out after paying) or a "Thank You" page.
