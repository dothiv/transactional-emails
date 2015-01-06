---
layout: tld-text-de
---

{% raw %}
Hallo {{ firstname }} {{ lastname }},  
Herzlichen Dank, dass Sie sich für eine .hiv Adresse entschieden haben.

{{ domain }} ist Ihre digitale Rote Schleife! Wir hoffen, Sie nutzen sie mit Stolz.

dotHIV belohnt jeden Besuch mit einer kleine Spende an HIV Organisationen auf der ganzen Welt. Organisationen wie ‘We actX for Hope’ aus Ruanda, die betroffene Frauen dabei hilft, gesunde Kinder zur Welt zu bringen und großzuziehen.

Aus technischen Gründen kann es bis zu 48 Stunden dauern, bis {{ domain }} online erreichbar ist. Herzlichen Dank für Ihr Verständnis.

Um Ihren Click-Counter anzupassen und auf Ihre Klick-Statistiken zuzugreifen, können Sie sich hier mit Ihrer Emailadresse {{ email }} in Ihr Kundenprofil hier einloggen: https://click4life.hiv/de/account

Nun soll die Welt auch vom neuen, zweiten Eingang zu Ihrer Homepage erfahren, der mithilft, Leben zu retten. In unserem “Tell-the-World-Package” finden Sie 12 Tipps für einfache und schnelle Maßnahmen, die Ihre User auf {{ domain }} aufmerksam machen: https://click4life.hiv/de/p/about/getactive#about-getactive-howto

Zusammen können wir AIDS besiegen.

++++++++++ Rechnung ++++++++++

\#{{ invoice.no }}  
{{ invoice.created }}

{{ invoice.fullname }}  
{{ invoice.address1 }}  
{{ invoice.address2 }}  
{{ invoice.country }}  
{{ invoice.vatNo }}

{{ invoice.item_description }}: {{ invoice.item_price }}  
{% if invoice.vat_percent %}{{ invoice.vat_percent }}% MwSt: {{ invoice.vat_price }}{% endif %}    
Summe: {{ invoice.total_price }}

{% endraw %}
