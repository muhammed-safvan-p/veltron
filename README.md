# Veltron eCommerce 🛒

> A production-style multi-role e-commerce platform where customers shop, vendors manage their stores, and admins oversee the entire platform — all in one unified system.

Built with **Node.js**, **Express.js**, **MongoDB**, and **EJS** following the **MVC architecture** pattern. Designed with real-world eCommerce workflows in mind — from cart and checkout to vendor analytics and admin control.

---

## Features

### 👤 User
- Secure authentication and session management
- Product browsing with variant-based inventory handling
- Cart, wishlist, and checkout workflows
- Multiple payment options — Razorpay, Wallet, and Cash on Delivery
- Coupon and referral reward system
- Order tracking, cancellation, and return workflows
- Wallet transaction history and profile management

### 🏪 Vendor
- Vendor onboarding and approval workflow
- Product management with stock control
- Vendor-specific order tracking
- Analytics dashboard with sales insights
- Report generation with PDF and Excel export support

### 🛡️ Admin
- Centralized platform management
- User, vendor, product, and order administration
- Revenue and sales analytics dashboard
- Coupon and banner management
- Return, refund, and payment monitoring
- Role-based access control workflows

---

## Tech Stack

| Layer | Technology |
|---|---|
| Frontend | EJS, CSS, JavaScript |
| Backend | Node.js, Express.js |
| Database | MongoDB |
| Payments | Razorpay |
| Charts | Chart.js |
| Reports | PDF & Excel generation |

---

## Architecture

```
veltron-commerce/
├── src/
│   ├── app.js
│   ├── config/            # DB, mailer, Razorpay, Passport, Multer
│   ├── constants/         # Status codes, messages, permissions
│   ├── controllers/       # admin/ · user/ · vendor/
│   ├── models/            # admin/ · common/ · user/ · vendor/
│   ├── routes/            # adminRoutes · userRoute · vendorRoute
│   ├── middleware/        # Auth guards, logger, error handler
│   ├── helpers/           # OTP, cart, password, response utils
│   └── validators/        # Request validation per role
├── views/
│   ├── layouts/           # Per-role EJS layout wrappers
│   ├── partials/          # Shared headers and sidebars
│   └── admin/ user/ vendor/ errors/
└── public/
    ├── styles/            # Role-scoped CSS
    └── js/                # Client-side scripts
```

---

## Engineering Highlights

- 🔐 Role-based authentication and authorization for three user types
- 💳 Payment gateway integration using Razorpay with wallet fallback
- 📦 Dynamic inventory and order management workflows
- 📊 Analytics visualization using Chart.js
- 📄 PDF and Excel report generation for vendors and admins
- 🔄 Coupon, referral, and reward system with wallet transactions
- 🛍️ Return and refund workflows with admin monitoring

---

## Future Improvements

- [ ] Redis caching layer for session and product data
- [ ] Docker containerization for deployment
- [ ] Automated testing (unit + integration)
- [ ] Real-time order updates using WebSockets
- [ ] CI/CD pipeline integration

---

## Final Note

Veltron eCommerce is designed as a production-oriented eCommerce platform focused on scalable backend systems, multi-role workflows, and real-world eCommerce architecture.
