---
order: 0
homepage: true
key: home
layout: product
title: A central platform to store, share and analyse your data
description: The Data Platform will enhance data usage across the Ministry of Justice
includeInBreadcrumbs: false
---
<div class="govuk-grid-row">
{% for item in collections.homepageLinks %}
  <section class="govuk-grid-column-one-third-from-desktop govuk-!-margin-bottom-8">
    <h2 class="govuk-heading-m govuk-!-font-size-27"><a href="{{ item.url | url }}">{{ item.data.title}}</a></h2>
    <p class="govuk-body">{{ item.data.description | markdown("inline") }}</p>
  </section>
{% endfor %}
</div>
