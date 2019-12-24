# Stripe Checkout in Facebook Messenger Webview Demo

https://developers.facebook.com/docs/messenger-platform/webview/

## Setup

- Create Stripe Account:
- Enable client-only checkout
- Add `username.github.io` to domain whitelist in https://dashboard.stripe.com/account/checkout/settings
- Create a one-time or recurring product in the Stripe Dashboard: https://dashboard.stripe.com/products
  - After creation click the "Use with checkout" button and copy the sku (sku_xxx) or plan (plan_xxx) ID
- Copy your publishable key from: https://dashboard.stripe.com/apikeys
- Put the URL together:
  - One-time Products: https://username.github.io/reponame/index.html?pk=<YOUR_PUBLISHABLE_KEY>&sku=<YOUR_SKU_ID>&qty=<QUANTITY_NUMBER>
  - Subscription (recurring): https://username.github.io/reponame/?pk=<YOUR_PUBLISHABLE_KEY>&plan=<YOUR_PLAN_ID>&qty=<QUANTITY_NUMBER>

## Example URL

https://thorsten-stripe.github.io/stripe-checkout-facebook-messenger-webview/index.html?pk=pk_test_g1IRNyIPvlOyweLpzIBPsean006Im59BP4&plan=plan_GPucFgVZx8Sr87&qty=1
