---
layout: click4life-de
---

{% raw %}
<tr width="100%" itemscope itemtype="http://schema.org/EmailMessage">
    <td valign="top" align="left" style="background:#fff; padding: 40px;" itemprop="action" itemscope itemtype="http://schema.org/ViewAction">
        <h1 style="font-size: 20px; margin: 0; color: #333;">
            Hallo {{ firstname }} {{ surname }}, </h1>

        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            Vielen Dank, dass Sie ein Premium Abonnement für Ihre .hiv Domain gebucht haben.</p>

        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            Wir haben Ihre Zahlungsdaten bestätigt; Ihr Premium Click-Counter ist nun für Ihre .hiv domain <strong>{{ domain }}</strong> aktiviert. </p>

        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            Nochmals vielen Dank für Ihre Unterstützung. </p>
            
        <h2>Rechnung</h2>
                
        <p>
            #{{ invoice.no }}
        </p>
        
        <p>
            {{ subscription.fullname }}<br>
            {{ subscription.address1 }}<br>
            {{ subscription.address2 }}<br>
            {{ subscription.country }}
        </p>
        
        <p>
            {{ subscription.taxNo }}<br>
            {{ subscription.vatNo }}<br>
            <small>{{ subscription.type }}</small>
        </p>
        
        <table style="width: 100%">
            <tbody>
            <tr>
                <td>
                    {{ invoice.item_description }}
                </td>
                <td style="text-align: right;">
                    {{ invoice.item_price }}
                </td>
            </tr>
            {% if invoice.vat > 0 %}
                <tr>
                    <td>
                        {{ invoice.vat_percent }}% MwSt.
                    </td>
                    <td style="text-align: right;">
                        {{ invoice.vat_price }}
                    </td>
                </tr>
            {% endif %} 
            </tbody>
            <tfoot>
            <tr>
                <td>
                    <strong>Summe</strong>
                </td>
                <td style="text-align: right;">
                    <strong>{{ invoice.total_price }}</strong>
                </td>
            </tr>
            </tfoot>
        </table>
    </td>
</tr>
{% endraw %}
