---
layout: page
title: ./Services
permalink: /services/
---
## Our Services

{% for service in site.services %}
  <div x-data="{ open: false }">
    <h2>{{ service.name }} - {{ service.description }}</h2>
    <p>{{ service.introtext  }} <br /><button x-on:click="open = ! open"> ./more </button></p>
    
    <div x-show="open" style="padding-left: 20px;">
      {{ service.content }} 
    </div>
  </div>
{% endfor %}

---

_How much we charge_

All services are available on an hourly rate, per-project or via a fixed retainer. For our _most common_ DevOps services, we charge around the AU$250 per hour mark - but every job is different. Please get in touch to discuss.

For web, translation and copy-editing services, we charge around the AU$50 per hour ballpark, again by negotiation

If you're a startup with a tiny budget, that's OK. Give us a shout, if your project has a noble goal or has an intriguing purpose, we can definitely come to an arrangement. Educational and Social Service organisations _always_ get a discount.

We won't work for companies in the gambling, mobile gaming, petrochemical, mining or incarceration industries, and we won't touch blockchain projects with a giant stick. Sorry not sorry.