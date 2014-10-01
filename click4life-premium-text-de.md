---
layout: tld-text-de
---

{% raw %}
Hallo {{ firstname }} {{ surname }},

Vielen Dank, dass Sie ein Premium Abonnement für Ihre .hiv Domain gebucht haben.

Wir haben Ihre Zahlungsdaten bestätigt; Ihr Premium Click-Counter ist nun für Ihre .hiv domain {{ domain }} aktiviert.

Nochmals vielen Dank für Ihre Unterstützung.

++++++++++ Rechnung ++++++++++

\#{{ invoice.no }}

{{ subscription.fullname }}  
{{ subscription.address1 }}  
{{ subscription.address2 }}  
{{ subscription.country }}

{{ subscription.taxNo }}  
{{ subscription.vatNo }}  
{{ subscription.type }}

{{ invoice.item_description }}: {{ invoice.item_price }}  
{% if invoice.vat > 0 %}{{ invoice.vat_percent }}% MwSt.: {{ invoice.vat_price }}{% endif %}  
Summe: {{ invoice.total_price }}
{% endraw %}
