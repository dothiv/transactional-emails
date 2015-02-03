---
layout: tld-text-de
---

{% raw %}
Hallo {{ firstname }} {{ lastname }},  
Herzlichen Dank, dass Sie sich für eine .hiv Adresse entschieden haben.

{{ domain }} ist Ihre digitale Rote Schleife! Wir hoffen, Sie nutzen sie mit Stolz.

dotHIV belohnt jeden Besuch mit einer kleine Spende an HIV Organisationen auf der ganzen Welt. Organisationen wie ‘We actX for Hope’ aus Ruanda, die betroffene Frauen dabei hilft, gesunde Kinder zur Welt zu bringen und großzuziehen.

Aus technischen Gründen kann es bis zu 48 Stunden dauern, bis {{ domain }} online erreichbar ist. Herzlichen Dank für Ihr Verständnis.

Um Ihren Click-Counter anzupassen und auf Ihre Klick-Statistiken zuzugreifen, können Sie sich hier mit Ihrer Emailadresse {{ email }} in Ihr Kundenprofil einloggen: https://click4life.hiv/de/account

Zusammen können wir AIDS besiegen.

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
{% if invoice.vat_percent %}{{ invoice.vat_percent }}% MwSt: {{ invoice.vat_price }}{% endif %}    
Summe: {{ invoice.total_price }}

{% if invoice.show_reverse_charge_note %}
Note: Services are subject to the reverse charge.  
VAT is to be accounted for by the recipient.
{% endif %}
{% endraw %}
