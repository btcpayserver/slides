---
theme: light
marp: true
---

![bg left:40% 40%](./media/btcpay-logo.svg)

# BTCPay Server eCommerce integrations



@ndeet, estimated block height #752730

---

# History has been made

![bg right:60% 60%](./ecommerce-integrations/btcpay-birth-emperor.png)

---

# BitPay compatible API

## Features
* make BitPay obsolete
* drop in replacement for merchants
* checkout/payments
* IPN callback notifications (insecure payload)

---

# Greenfield API

![bg right](./ecommerce-integrations/mind-blown.gif)

---

# The future
## Greenfield API

### Features
* modern REST API
* easy API key setup
* well documented using openAPI (Swagger)
* webhooks/event with signed payload
* managing wallets, pull payments/payouts (for refunds)
* more detailed information
* payment requests
* and much more: Node/Apps/User/Store management, ...


---

# eCommerce integrations

- Shopify *
- WooCommerce *
- Magento 2 *
- PrestaShop *
- Zapier *
- VirtueMart *
- OpenCart (soon) *
- Drupal Commerce
- Shopware

\* using Greenfield API

---

![bg contain](./ecommerce-integrations/shopify_checkout_1.png)

---

![bg contain](./ecommerce-integrations/shopify_checkout_2.png)

---

# Common use cases

* Basic checkout flow
* Receiving notifications (IPN) / webhook events

---

# Other interesting use cases

* separate payment methods
  - payment method based discounts, vouchers, ...
* no-redirect payment
* refunds, pull payments
* subscriptions via payment requests
* automations (Zapier)

---

# WooCommerce

## Separated payment gateways (payment methods)

- discount on payment gateways
- promotion tokens as vouchers

See: [https://docs.btcpayserver.org/FAQ/Integrations/#woocommerce-faq](https://docs.btcpayserver.org/FAQ/Integrations/#woocommerce-faq)

---

## WooCommerce: discounts on payment gateways

![](./ecommerce-integrations/payment_method_discount.png)

---

## WooCommerce: promotion tokens as vouchers

e.g. Blockstream Jade, token from presale used to claim product

![height:70%](./ecommerce-integrations/woocommerce_at_limit-payment-methods-rules.png)

---

# Custom integrations with Greenfield API


## Libraries
- C#
- PHP (btcpayserver-greenfield-php on packagist.org)
- JavaScript/NodeJS (help wanted)

---

## Custom integrations cURL / HTTP clients


```bash
curl -s \
     -H "Content-Type: application/json" \
     -H "Authorization: token $apikey" \
     -X GET \
     "$BTCPAY_INSTANCE/api/v1/stores/$store_id"
```

- [Greenfield API docs](https://docs.btcpayserver.org/API/Greenfield/v1)
- [cURL examples](https://docs.btcpayserver.org/Development/GreenFieldExample/)

---

# What's next?

---

![bg contain](./media/supporters-light.png)
