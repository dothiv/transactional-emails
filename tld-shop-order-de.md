---
layout: tld-de
---

{% raw %}
<tr width="100%">
    <td valign="top" align="left" style="background:#fff; padding: 40px;">
        <h1 style="font-size: 20px; margin: 0; color: #333;">
            Hallo {{ firstname }} {{ lastname }},</h1>
            
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            Herzlichen Dank, dass Sie sich für eine .hiv Adresse entschieden haben.
        </p>
            
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            {{ domain }} ist Ihre digitale Rote Schleife! Wir hoffen, Sie nutzen sie mit Stolz.
        </p>
        
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            dotHIV belohnt jeden Besuch mit einer kleine Spende an HIV Organisationen auf der ganzen Welt. 
            Organisationen wie ‘We actX for Hope’ aus Ruanda, die betroffene Frauen dabei hilft, gesunde Kinder zur Welt zu bringen und großzuziehen.
        </p>
        
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            Aus technischen Gründen kann es bis zu 48 Stunden dauern, bis {{ domain }} online erreichbar ist. Herzlichen Dank für Ihr Verständnis. 
        </p>
        
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            Um Ihren Click-Counter anzupassen und auf Ihre Klick-Statistiken zuzugreifen, können Sie sich <a href="https://click4life.hiv/de/account">hier</a> mit Ihrer Emailadresse {{ email }} in Ihr Kundenprofil einloggen.
        </p>
        
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            Zusammen können wir AIDS besiegen.
        </p>
    </td>
</tr>
<tr width="100%">
    <td valign="top" align="left" style="background:#fff; padding: 40px;">
            
        <h2>Rechnung</h2>
        
        <p>
            #{{ invoice.no }}<br/>
            {{ invoice.created }}
        </p>
        
        <p>
            {{ invoice.fullname }}<br/>
            {{ invoice.address1 }}<br/>
            {{ invoice.address2 }}<br/>
            {{ invoice.country }}<br/>
            {{ invoice.organization }}<br/>
            {{ invoice.vatNo }}
        </p>
        
        <table style="width: 100%">
            <tfoot>
            <tr>
                <td>
                    <strong>Summe</strong>
                </td>
                <td style="text-align: right; white-space: nowrap;">
                    <strong>{{ invoice.total_price }}</strong>
                </td>
            </tr>
            {% if invoice.show_reverse_charge_note %}
            <tr>
            <td colspan="2">
                Note: Services are subject to the reverse charge.<br/>
                VAT is to be accounted for by the recipient.
            </td>
            </tr>
            {% endif %}
            </tfoot>
            <tbody>
            <tr>
                <td>
                    {{ invoice.item_description }}
                </td>
                <td style="text-align: right; white-space: nowrap;">
                    {{ invoice.item_price }}
                </td>
            </tr>
            {% if invoice.vat_percent %}
                <tr>
                    <td>
                        {{ invoice.vat_percent }}% MwSt.
                    </td>
                    <td style="text-align: right; white-space: nowrap;">
                        {{ invoice.vat_price }}
                    </td>
                </tr>
            {% endif %} 
            </tbody>
        </table>
    </td>
</tr>
{% endraw %}
