---
layout: tld-text-en
---

{% raw %}
Hello {{ firstname }},

Thank you for purchasing a premium subscription for your .hiv domain name.

We have confirmed your payment and your premium Click-Counter is now active for your domain {{ domain }}.

Thanks again for your support.

++++++++++ Invoice ++++++++++

\#{{ invoice.no }}

{{ subscription.fullname }}  
{{ subscription.address1 }}  
{{ subscription.address2 }}  
{{ subscription.country }}

{{ subscription.taxNo }}  
{{ subscription.vatNo }}  
{{ subscription.type }}

{{ invoice.item_description }}: {{ invoice.item_price }}  
{% if invoice.vat > 0 %}{{ invoice.vat_percent }}% VAT: {{ invoice.vat_price }}{% endif %}  
Total: {{ invoice.total_price }}
{% endraw %}
