---
layout: tld-text-en
---

{% raw %}
Hello {{ firstname }},

Thank you for purchasing a premium invoice.for your .hiv domain name.

We have confirmed your payment and your premium Click-Counter is now active for your domain {{ domain }}.

Thanks again for your support.

++++++++++ Invoice ++++++++++

\#{{ invoice.no }}  
{{ invoice.created }}

{{ invoice.organization }}  
{{ invoice.fullname }}  
{{ invoice.address1 }}  
{{ invoice.address2 }}  
{{ invoice.country }}  
{{ invoice.vatNo }}  

{{ invoice.item_description }}: {{ invoice.item_price }}  
{% if invoice.vat_percent %}{{ invoice.vat_percent }}% VAT: {{ invoice.vat_price }}{% endif %}  
Total: {{ invoice.total_price }}

{% if invoice.show_reverse_charge_note %}
Note: Services are subject to the reverse charge.  
VAT is to be accounted for by the recipient.
{% endif %}
{% endraw %}
