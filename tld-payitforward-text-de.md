---
layout: tld-text-de
---

{% raw %}
Hallo {{ firstname }} {{ surname }},
            
Vielen Dank, dass Sie die digitale rote Schleife weitertragen!  
Dies sind die Gutschein-Codes für Ihre Freunde.

{% for voucher in vouchers %}  
{{ voucher.name }} ({{ voucher.domain }}): {{ voucher.code }}    
{% endfor %}

Die Rechnung für Ihren Einkauf finden Sie im Anhang.

Nun senden Sie ihnen Ihr Geschenk – Einen Textvorschlag für Ihre Email haben wir weiter unten für Sie vorbereitet.

Mit Ihrer Hilfe wird das Internet zu einem immer größer werdenden Netzwerk für das Ende von AIDS! Wir sagen herzlichen Dank und wünschen viel Freude an Ihrer eigenen digitalen Roten Schleife.

Ihr dotHIV Team

Die Laufzeit der kostenlosen Domainregistrierung beträgt 1 Jahr. Bei Verlängerung fallen pro Folgejahr weitere 160 € Registrierungsgebühr an, von der mindestens 90€ an HIV Projekte gehen.

{% for voucher in vouchers %}  
+++++++++++++++++++++++++++++

Hallo {{ voucher.name }},

heute schenke ich Dir eine digitale rote Schleife für Deine Website: {{ voucher.domain }}  
Die gemeinnützigen .hiv-Domains schaffen neue Gelder und neue Aufmerksamkeit für das Ende von AIDS.  
{% if domain %}Wir sind mit {{ domain }} dabei.{% endif %}
Die beiliegende Infografik erklärt die Arbeit von dotHIV auf einen Blick. Weitere Infos findest Du auf https://click4life.hiv/.

Bei dotHIV's Parterregistrar Domaindiscount24 (http://www.domaindiscount24.com/de) kannst Du Deine Domain mit diese Gutscheincode kostenfrei registrieren:

{{ voucher.code }}

Am besten in den nächsten 24 Stunden!

Bitte beachten Sie: wenn Sie bei DomainDiscount24 einen neuen Account anlegen, gibt es am Ende des Formulars eine Eingabefeld für einen Promo Code.    
Bitte geben Sie dort nicht Ihren Gutscheincode ein!  
Sie werden bei einem späteren Schritt im Warenkorb nochmal nach dem Gutscheincode gefragt.

Nun gilt es, eine neue Bewegung zu starten. Wie wär’s? Machst Du mit und trägst die digitale Rote Schleife weiter? Es sind nur drei kleine Schritte auf payitforward.hiv

1. Gib die Freude weiter und spendiere 3 Freunden / Kunden / Geschäftspartnern eine .hiv-Domain. Auf http://payitforward.hiv/ sind die Gutschein-Codes für 160 € zzgl. MwSt. zu erwerben. Mindestens 90 € pro Domain gehen an gemeinnützige HIV-Projekte.  
2. Lass Facebook und/oder Twitter davon wissen, mit Hashtag #dotHIV und einem Link auf die Beschenkten.  
3. Schicke den Beschenkten ihren Code per E-Mail, die Freude macht. So wie diese hier.

Ich freue mich sehr, wenn Du Deine digitale Rote Schleife trägst. Gemeinsam setzen wir ein Zeichen für das Ende von AIDS!

Dein {{ firstname }} {{ surname }}

{% endfor %}

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
