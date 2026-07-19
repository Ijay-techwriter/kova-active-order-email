# KOVA Active — Order Confirmation Email

A Shopify order confirmation email rebuilt from scratch using Liquid templating.

## The Problem

The original email was hardcoded — every customer received "Hi Customer," and "Order #1234" regardless of who they were or what they ordered. Customers were calling support thinking the email was spam.

## What Was Built

A production-ready HTML email template using Shopify Liquid that dynamically pulls real customer and order data for every send.

**Liquid features used:**
- `{{ customer.first_name }}` and `{{ customer.email }}` — personalised greeting
- `{{ order.name }}` and `{{ order.created_at | date: "%B %d, %Y" }}` — real order details
- `{% for line_item in order.line_items %}` — loops through every product ordered
- `{{ line_item.price | money }}` — currency formatting using the money filter
- `{% if order.total_price > 5000000 %}` — conditional VIP message for orders over ₦50,000
- **Live preview:** https://ijay-techwriter.github.io/kova-active-order-email/demo-version/


## Folder Structure
kova-active-order-email/
├── broken-version/
│   └── index.html        # Original broken hardcoded email
├── fixed-version/
│   ├── index.html        # Rebuilt HTML with Liquid tags
│   └── order-confirmation.liquid
├── demo-version/
│   └── index.html        # Static preview with dummy data
## Skills Demonstrated

HTML email development · Liquid templating · Shopify email notifications · Conditional logic · Dynamic loops · Currency filters

## Developer

Vivian Amadi — HTML Email Developer & Email Signature Specialist
[LinkedIn](https://linkedin.com/in/vivian-amadi-ijeoma) · [Upwork](https://www.upwork.com/freelancers/~017e0c74622c57ea0c)
