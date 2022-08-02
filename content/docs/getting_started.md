---
title: Getting Started
type: doc

---

### Pre Requisites

- a website ( a simple static website will do )
-

### First Step

- add the tagshop js script to your page

```html
<!-- 
    TAG_SHOP_DOMAIN would be https://app.tagshop.com/ or your own domain if you choose to host your own
    TAG_SHOP_URL would be TAG_SHOP_DOMAIN
    TAG_SHOP_ACCOUT is a combination of your VendorID and a VendorKey used to authorize this site
-->

<script
  id="tagshop"
  src="{{ TAG_SHOP_DOMAIN }}/cart.js"
  data-path="{{ TAG_SHOP_URL }}"
  data-auth="{{ TAG_SHOP_ACCOUT }}"
></script>
```

### Second Step

- add a shopping cart icon to your website

```html
<a href="#" class="cart-icon" data-tagshop-cart-actuator>
  <em class="fa fa-shopping-basket"></em>
  <span class="counter">0</span>
</a>
```

### Third Step

- add the buy button to your website

```html
<button
  type="button"
  title="Add to Cart"
  class="btn btn-cart shop-item"
  data-tagshop-product-name="the name of your product"
  data-tagshop-product-id="603575377c97acff5a146d01"
  data-tagshop-product-price="145.35"
>
  <i class="fa fa-cart"></i> <span> Add to Cart</span>
</button>
```

