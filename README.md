# Havillah Stripe Checkout Backend

This is the backend server that powers the Stripe Checkout integration for [havillahmarketplace.com](https://havillahmarketplace.com).

It handles the creation of Stripe Checkout sessions, passing the cart items (product name, price, quantity, and image) and redirecting users to Stripe for payment.

---

## 🔧 How to Use

1. Send a `POST` request to `/create-checkout-session` with this payload:
```json
{
  "items": [
    {
      "name": "Product Name",
      "price": 18.50,
      "quantity": 1,
      "image": "https://your-cdn.com/product-image.jpg"
    }
  ]
}
