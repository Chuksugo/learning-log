# 🧠 Weekly Developer Learning Log – Python/Django Backend

Welcome to my public weekly work and learning log. This document captures my journey as a professional backend developer, focusing on Python, Django, and API architecture. Each week, I reflect on what I built, learned, tested, and contributed — all aimed at growing as a backend engineer.

> Inspired by [Gergely Orosz](https://blog.pragmaticengineer.com/) and [Julia Evans](https://jvns.ca), this log is my living record of technical growth, system design exploration, and real-world backend development.

---

## 📅 Week of 2025-07-18

### 🛠️ **Project Focus**: `E-commerce Product API`
- **Tech Stack**: Django REST Framework, MySQL, Stripe
- **Core Apps**: `products`, `orders`, `vendors`, `wishlist`, `cart`

---

### ✅ **What I Accomplished**
- ✅ Developed `GET /api/products/` endpoint with:
  - 🔍 Filtering (e.g., by category, price)
  - 🔎 Search by name and description
  - 📄 Pagination (limit/offset)
- ✅ Implemented token-based authentication using `DRF SimpleJWT`
- ✅ Refactored business logic into a **service layer** to improve testability and separation of concerns
- ✅ Wrote 20+ unit and integration tests with `TestCase` + `APIClient`

---

### 🧪 **Testing Highlights**
- 📈 Achieved **87% code coverage** via `coverage.py`
- 🔧 Mocked external dependencies:
  - Stripe webhooks using `unittest.mock.patch`
- 📁 Organized test suite by concern:
  - `tests/test_models.py`
  - `tests/test_views.py`
  - `tests/test_api.py`

---

### 📄 **Documentation & Planning**
- 📝 Drafted **Inventory System Design Doc**
- ✅ Reviewed and commented on `vendor_payout_logic.md`
- 🧹 Added tech debt cleanup tasks and service refactoring to Jira backlog

---

### 👥 **Team Collaboration**
- 🔍 Reviewed 4 PRs with detailed feedback
- 🧩 Helped teammate resolve a tricky `makemigrations` merge conflict
- 🧭 Walked frontend engineer through consuming `/products/<id>/` via Swagger & Postman

---

### 💡 **What I Learned**
- 🧪 `@override_settings()` — useful for isolating test configs (e.g., mock email backends)
- 🔐 `force_authenticate()` — simplified testing of protected views in DRF
- 🧱 Modular test design across apps using consistent patterns for factories, setup, and assertions

---

### 🎯 **Next Week’s Goals**
- [ ] Integrate Stripe payment endpoint with **webhook verification**
- [ ] Extend `Product` model with **review and rating** support
- [ ] Publish detailed **API documentation** with example cURL and Postman requests
- [ ] Push for **95%+ test coverage** across all critical paths

---

## 📚 Archive

| Week | Summary |
|------|---------|
| [Week of 2025-07-18](#week-of-2025-07-18) | Product endpoint, DRF testing, mocking Stripe, and modular test design |
| Week of 2025-07-25 | *(Coming soon)* |

---

## 📝 Credits & Inspiration

- Adapted from [The Pragmatic Engineer](https://blog.pragmaticengineer.com/)
- Based on [Julia Evans’ Brag Document](https://jvns.ca/blog/brag-documents/)