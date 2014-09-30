---
layout: click4life-en
---

{% raw %}
<tr width="100%" itemscope itemtype="http://schema.org/EmailMessage">
    <td valign="top" align="left" style="background:#fff; padding: 40px;" itemprop="action" itemscope itemtype="http://schema.org/ViewAction">
        <h1 style="font-size: 20px; margin: 0; color: #333;">
            Hello {{ firstname }},</h1>

        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            Thank you for purchasing a premium subscription for your .hiv domain name. </p>

        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            We have confirmed your payment and your premium Click-Counter is now active for your domain <strong>{{ domain }}</strong>. </p>

        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            Thanks again for your support. </p>
            
        <h2>Invoice</h2>
        
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
        
        <table>
            <tbody>
            <tr>
                <td>
                    {{ invoice.item_description }}
                </td>
                <td class="money">
                    {{ invoice.item_price }}
                </td>
            </tr>
            {% if invoice.vat > 0 %}
                <tr>
                    <td>
                        {{ invoice.vat_percent }}% VAT
                    </td>
                    <td class="money">
                        {{ invoice.vat_price }}
                    </td>
                </tr>
            {% endif %} 
            </tbody>
            <tfoot>
            <tr>
                <td>
                    Total
                </td>
                <td class="money">
                    {{ invoice.total_price }}
                </td>
            </tr>
            </tfoot>
        </table>
    </td>
</tr>
{% endraw %}
