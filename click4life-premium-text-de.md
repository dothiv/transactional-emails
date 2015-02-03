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
{{ invoice.created }}

{{ invoice.fullname }}  
{{ invoice.address1 }}  
{{ invoice.address2 }}  
{{ invoice.country }}  
{{ invoice.organization }}  
{{ invoice.vatNo }}  

{{ invoice.item_description }}: {{ invoice.item_price }}  
{% if invoice.vat_percent %}{{ invoice.vat_percent }}% MwSt.: {{ invoice.vat_price }}{% endif %}  
Summe: {{ invoice.total_price }}

{% if invoice.show_reverse_charge_note %}
Note: Services are subject to the reverse charge.  
VAT is to be accounted for by the recipient.
{% endif %}
{% endraw %}
