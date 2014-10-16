---
layout: tld-text-en
---

{% raw %}
Dear {{ firstname }} {{ surname }},
            
Thank you very much for sharing the digital Red Ribbon.  
These are the voucher codes for your friends.

{% for voucher in vouchers %}  
{{ voucher.name }} ({{ voucher.domain }}): {{ voucher.code }}    
{% endfor %}

Please find enclosed the invoice for your purchase.

Now you send them your gift - Please find below a proposed email text.

With your support, the internet becomes one big network for the end of AIDS! We'd like to express our sincere thanks and we wish you a great digital Red Ribbon experience.

Your dotHIV Team

The term of the free domain registration is 1 year. On renewing an additional annual registration fee of 160€  will be incurred, whereby at least 90€ will support HIV Projects.

{% for voucher in vouchers %}  
+++++++++++++++++++++++++++++

Dear {{ voucher.name }},

Today I give you a digital Red Ribbon for your website: {{ voucher.domain }}  
The charitable .hiv domains generate new funds and new attention for the end of AIDS.
{% if domain %}We've joined the .hiv moment with {{ domain }}.{% endif %}  
The attached infographic explains dotHIV's work at a glance. You will find further information at https://click4life.hiv/.

You can register your own domain for free at Domaindiscount24 (http://www.domaindiscount24.com/en), dotHIV's affiliated Registrar, with the following voucher code:

{{ voucher.code }}

Most effective within the next 24 hours!

Please note: When creating a new account with DomainDiscount24, there is a box at the end of the page where you can enter a promo code.    
Please do NOT enter your voucher code there!  
You will be ask for code later in the process in your shopping cart.

It is now time to commence a new movement. What do you think? Will you participate and spread the word about the digital Red Ribbon? Just three small steps will direct you to payitforward.hiv

1. Pass on the joy and give a .hiv domain to 3 friends/ clients/ business partners. You can acquire voucher codes at http://payitforward.hiv/ at the price of 160€ plus VAT. At least 90€ will support charitable HIV Projects.
2. Spread the word on facebook and/ or twitter using hashtag #dotHIV and the links to the presentees.
3. Send the presentees your love and their own voucher code with a personal email.

I would love to see you wearing your own digital Red Ribbon. Let us together set a sign for the end of AIDS.

Yours,  
{{ firstname }} {{ surname }}

{% endfor %}

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
