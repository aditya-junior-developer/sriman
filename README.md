# SRIMAN — Premium Dry Fruits & Nuts

A premium e-commerce storefront for **SRIMAN**, a dry fruits, nuts, snacks, and gift hamper brand. Built with HTML, CSS, and JavaScript, with Firebase Authentication and Supabase-powered backend services.

---

## About SRIMAN

SRIMAN aims to bring quality dry fruits, nuts, delicious snacks, and thoughtfully curated gift hampers to customers across India.

The website is designed around a premium brand experience, combining an elegant visual identity, responsive layouts, smooth animations, and convenient shopping features.

## Product Collection

The planned catalogue includes:

### Snacks
- Masala Makhana
- Caramel Chocolate Popcorn
- Strawberry Popcorn
- Salty Popcorn

### Dry Fruits & Nuts
- Almonds (Badam)
- Cashews (Kaju)
- Walnuts (Akhrot)
- Pistachios (Pista)
- Raisins (Kishmish)
- Dates (Khajoor)
- Plain Fox Nuts (Makhana)

### Gifts
- Curated Gift Hampers

*Product availability, pricing, weights, and specifications are managed through the catalogue and should be confirmed before purchase.*

---

## Features

### Customer Experience
- Responsive storefront for desktop, tablet, and mobile.
- Premium brand-focused design and animations.
- Product catalogue with category browsing.
- Product search and filtering when catalogue data is available.
- Shopping cart and wishlist interface.
- Product detail views.
- Customer account registration and login.
- Google sign-in through Firebase Authentication.
- Password reset and email verification support.
- Customer order history.
- Contact and enquiry form.

### Administration
- Admin dashboard.
- Product creation and editing.
- Product archiving.
- Inventory management.
- Order management.
- Backend-controlled stock operations.

### Backend Integration
- Supabase database and Edge Functions.
- Firebase Authentication.
- Server-side order and inventory operations.
- Configurable catalogue and customer data.

---

## Technology Stack

| Technology | Purpose |
|---|---|
| HTML5 | Website structure |
| CSS3 | Styling, responsive layouts and animations |
| JavaScript | Frontend functionality |
| Firebase Authentication | Customer authentication |
| Supabase | Database and backend services |
| Supabase Edge Functions | Server-side operations |
| Vercel | Website hosting and deployment |

---

## Project Structure

The storefront is designed to be deployable as a single HTML file.

```text
SRIMAN/
└── index.html
```

The HTML contains the frontend structure, styles, scripts, brand logo, and embedded visual assets.

External services are required for authentication, database access, and backend functionality.

---

## Configuration

The frontend uses Firebase and Supabase.

### Firebase

Firebase Authentication is used for:
- Email and password authentication.
- Google sign-in.
- Password reset.
- Email verification.

Configure the Firebase project's authorized domains in the Firebase Console before deploying the website.

### Supabase

Supabase provides:
- Product catalogue data.
- Order-related backend operations.
- Inventory management.
- Customer and administrative data.

The frontend connects to a Supabase Edge Function:

```text
/functions/v1/store-api
```

The Edge Function and database schema must be deployed and configured in the Supabase project.

**Security note:** Never expose Supabase service-role keys, private API secrets, payment credentials, or other server-side secrets in `index.html` or any public GitHub repository.

---

## Local Development

1. Clone the repository:

```bash
git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
```

2. Open the project folder.

3. Run `index.html` using a local development server or deploy it to a hosting provider.

4. Ensure Firebase and Supabase services are configured and accessible.

---

## Deployment

The frontend can be hosted using services such as:

- Vercel
- Netlify
- GitHub Pages (frontend-only hosting)

For a functional deployment, configure the backend separately:

1. Apply the required Supabase database schema and migrations.
2. Deploy the `store-api` Supabase Edge Function.
3. Configure the required server-side environment variables and permissions.
4. Configure Firebase authorized domains.
5. Configure and verify the admin authorization process.
6. Test authentication, catalogue loading, orders, and inventory operations.

A successful frontend deployment alone does not mean the complete commerce backend is production-ready.

---

## Payments & Delivery

The website's order-request workflow should not be confused with a completed payment integration.

A real payment system requires:
- A supported payment gateway.
- Server-side payment verification.
- Secure webhook handling.
- Order payment-status updates.

Delivery and shipment tracking also require integration with a logistics provider.

Do not treat an order request as a confirmed paid order until the backend verifies payment.

---

## Important Notes

- The website is built for the SRIMAN brand.
- Product prices and weights must be entered and verified by the administrator.
- Product visuals may be conceptual and should not be treated as approved packaging artwork.
- FSSAI and other applicable business compliance details must be verified before commercial operations.
- Never publish private credentials or customer information in this repository.
- Test all backend integrations before accepting real customer orders.

---

## Brand Identity

**Brand:** SRIMAN  
**Tagline:** Premium Dry Fruits & Nuts  
**Category:** Dry Fruits, Nuts, Snacks & Gift Hampers  
**Market:** India  
**Visual Identity:** Chocolate Brown · Forest Green · Warm Ivory · Muted Gold

---

## Project Status

The repository contains the SRIMAN storefront frontend and its integration points.

Production operation depends on the deployment and verification of the connected authentication, database, backend, payment, and delivery services.

---

## License

All SRIMAN brand assets, logos, product visuals, and original brand content are reserved to their respective owner unless otherwise stated.

Do not reuse SRIMAN branding or assets for commercial purposes without permission.

---

**SRIMAN — Premium Dry Fruits & Nuts**  
*Thoughtfully selected. Beautifully presented.*
