---
layout: page
title: Products
permalink: /products/
---

# Our Stainless Steel Products

Browse our complete catalog of premium tableware. Click any product for detailed specifications and pricing.

{% for product in site.products %}
  <div class="product-card">
    <h3><a href="{{ product.url }}">{{ product.title }}</a></h3>
    <p>{{ product.description }}</p>
    <span class="price">{{ product.price }}</span>
  </div>
{% endfor %}
