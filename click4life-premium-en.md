---
layout: click4life-en
---

{% raw %}
<tr width="100%" itemscope itemtype="http://schema.org/EmailMessage">
    <td valign="top" align="left" style="background:#fff; padding: 40px;" itemprop="action" itemscope itemtype="http://schema.org/ViewAction">
        <h1 style="font-size: 20px; margin: 0; color: #333;">
            Hello {{ firstname }},</h1>

        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            Thank you for purchasing a premium invoice.for your .hiv domain name. </p>

        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            We have confirmed your payment and your premium Click-Counter is now active for your domain <strong>{{ domain }}</strong>. </p>

        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            Thanks again for your support. </p>
            
        <h2>Invoice</h2>
        
        <p>
            #{{ invoice.no }}<br>
            {{ invoice.created }}
        </p>
        
        <p>
            {{ invoice.fullname }}<br>
            {{ invoice.address1 }}<br>
            {{ invoice.address2 }}<br>
            {{ invoice.country }}<br>
            {{ invoice.vatNo }}
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
            {% if invoice.vat_percent %}
                <tr>
                    <td>
                        {{ invoice.vat_percent }}% VAT
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
                    <strong>Total</strong>
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
