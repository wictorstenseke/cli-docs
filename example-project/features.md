# Features - Example Project

> Track features and user stories for this project.

---

## 🚧 In Progress

### User Authentication System
**Description:** Implement secure user registration, login, and session management to allow users to create accounts and access personalized features.

**Priority:** High
**Owner:** unassigned
**Effort:** L
**Created:** 2026-01-16
**Updated:** 2026-01-23
**Dependencies:** Project Setup & Infrastructure

**Details:**
- Email/password registration with input validation (min length, format checks)
- Secure password hashing with bcrypt (min cost factor 12)
- JWT-based authentication with short-lived access tokens and refresh tokens
- Password reset via email link (expire after 1 hour)
- Email verification on sign-up before account activation

**Acceptance Criteria:**
- [ ] Users can register with email/password and receive a verification email
- [ ] Unverified accounts cannot log in
- [ ] Passwords are hashed and never stored in plain text
- [ ] JWT tokens expire and refresh correctly
- [ ] Password reset flow works end-to-end

**Notes:** OAuth (Google, GitHub) can be added as a separate planned feature once core auth is stable.

---

## 📋 Planned

### Product Catalog
**Description:** Create a browsable catalog of products with search, filtering, and sorting capabilities.

**Priority:** High
**Owner:** unassigned
**Effort:** L
**Created:** 2026-01-23
**Dependencies:** Project Setup & Infrastructure

**Details:**
- Product listing page with pagination (25 items/page)
- Full-text search by name, description, and category
- Filter by price range, category, and availability (in stock / out of stock)
- Sort by price (asc/desc), popularity, and newest
- Product detail page with image gallery, description, and stock status

**Acceptance Criteria:**
- [ ] Products load within 2 seconds on a standard connection
- [ ] Search returns results matching name, description, or category
- [ ] Filters and sort can be combined and reflected in the URL
- [ ] Out-of-stock products are visually distinct and cannot be added to cart

**Notes:** Requires integration with inventory management. Pagination should use cursor-based approach for performance at scale.

---

### Shopping Cart
**Description:** Allow users to add products to a cart and manage quantities before checkout.

**Priority:** Medium
**Owner:** unassigned
**Effort:** M
**Created:** 2026-01-23
**Dependencies:** User Authentication System, Product Catalog

**Details:**
- Add/remove items and update quantities
- Persist cart server-side for authenticated users
- LocalStorage fallback for guest users; merge on login
- Cart summary with per-item subtotal and grand total
- Enforce stock limits — prevent adding more than available inventory
- Show clear error when an item goes out of stock while in cart

**Acceptance Criteria:**
- [ ] Cart persists across page reloads for logged-in users
- [ ] Guest cart merges with user cart on login (no duplicate items)
- [ ] Attempting to exceed stock shows an error and caps quantity
- [ ] Out-of-stock items in cart display a warning and block checkout

**Notes:** Edge cases: item goes out of stock while in cart, price changes after item added (display original vs. current price).

---

### Checkout & Payment Processing
**Description:** Secure checkout flow with payment processing via Stripe.

**Priority:** Medium
**Owner:** unassigned
**Effort:** XL
**Created:** 2026-01-23
**Dependencies:** Shopping Cart

**Details:**
- Multi-step checkout: address → shipping method → payment → review
- Stripe Elements integration for card payments (PCI-compliant iframe)
- Stripe Webhooks to handle async payment confirmation
- Order confirmation page with order number and summary
- Transactional email receipt to customer on successful payment
- Failed payment handling: clear error messages and retry flow
- Refund support via Stripe dashboard (admin-initiated)

**Acceptance Criteria:**
- [ ] Payment form is rendered via Stripe Elements (no raw card data on our servers)
- [ ] Order is not created until payment is confirmed via webhook
- [ ] Failed payments show a user-friendly error and allow retry
- [ ] Customer receives confirmation email within 1 minute of successful payment
- [ ] Partial refunds can be issued from the admin dashboard

**Notes:** Never handle raw card numbers — use Stripe Elements only. PCI SAQ A compliance required. Test with Stripe test cards before going live.

---

## ✅ Done

### Project Setup & Infrastructure
**Description:** Initial project scaffolding, development environment, and deployment pipeline.

**Completed:** 2026-01-15
**Owner:** unassigned
**Effort:** M

**Notes:** Monorepo structure with shared TypeScript types. CI/CD pipeline configured with GitHub Actions. Vercel for frontend, Railway for backend, Neon for managed Postgres.

---

## ❌ Cancelled/Rejected

_No cancelled features yet._

---

<!-- Effort legend: S = hours, M = 1-3 days, L = 1-2 weeks, XL = weeks+ -->
