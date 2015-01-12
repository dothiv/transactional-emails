---
layout: tld-text-en
---

{% raw %}
Dear {{ firstname }} {{ lastname }},  
Thank you for registering a .hiv domain name.

{{ domain }} is your digital Red Ribbon! Use it with pride.

dotHIV rewards every visit with a small donation to HIV organizations around the world, like ‘WE ACTx for hope’ from Rwanda, which helps women living with HIV to give birth to and raise healthy babies.

For technical reasons, it might take up to 48 hours until {{ domain }} is online. So please bear with us.

To adapt your Click-Counter and access your Click Stats, you can log into your customer account with your email {{ email }} here: https://click4life.hiv/en/account

Together, we can end AIDS.

++++++++++ Invoice ++++++++++

\#{{ invoice.no }}  
{{ invoice.created }}

{{ invoice.fullname }}  
{{ invoice.address1 }}  
{{ invoice.address2 }}  
{{ invoice.country }}  
{{ invoice.vatNo }}

{{ invoice.item_description }}: {{ invoice.item_price }}  
{% if invoice.vat_percent %}{{ invoice.vat_percent }}% VAT: {{ invoice.vat_price }}{% endif %}    
Total: {{ invoice.total_price }}

{% endraw %}
