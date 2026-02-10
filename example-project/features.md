# Features - Example Project

> Track features and user stories for this project.

---

## 🚧 In Progress

### User Authentication System
**Description:** Implement secure user registration, login, and session management to allow users to create accounts and access personalized features.

**Details:**
- Email/password registration with validation
- Secure password hashing (bcrypt)
- JWT-based authentication
- Password reset functionality
- Email verification

**Notes:** Consider adding OAuth (Google, GitHub) in the future for easier sign-up.

---

## 📋 Planned

### Product Catalog
**Description:** Create a browsable catalog of products with search, filtering, and sorting capabilities.

**Details:**
- Product listing page with pagination
- Search by name, description, category
- Filter by price range, category, availability
- Sort by price, popularity, newest
- Product detail pages with images and descriptions

**Notes:** Need to integrate with inventory management system.

---

### Shopping Cart
**Description:** Allow users to add products to a cart and manage quantities before checkout.

**Details:**
- Add/remove items from cart
- Update quantities
- Persist cart in database for logged-in users
- LocalStorage fallback for guest users
- Cart summary with subtotal calculation

**Notes:** Must handle edge cases like out-of-stock items.

---

### Checkout & Payment Processing
**Description:** Secure checkout flow with payment processing using Stripe.

**Details:**
- Shipping address form
- Payment method selection
- Stripe integration for card payments
- Order confirmation page
- Email receipt to customer

**Notes:** Need to handle failed payments and refunds.

---

## ✅ Done

### Project Setup & Infrastructure
**Description:** Initial project scaffolding, development environment, and deployment pipeline.

**Completed:** 2026-01-15

**Notes:** Set up monorepo structure with shared TypeScript types. CI/CD pipeline configured with GitHub Actions.

---

## ❌ Cancelled/Rejected

_No cancelled features yet._
