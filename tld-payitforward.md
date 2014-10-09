---
layout: tld
---

{% raw %}
<tr width="100%">
    <td valign="top" align="left" style="background:#fff; padding: 40px;">
        <h1 style="font-size: 20px; margin: 0; color: #333;">
            Dear {{ firstname }} {{ surname }},</h1>
            
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            Thank you very much for sharing the digital Red Ribbon.<br/>
            These are the voucher codes for your friends.
        </p>
            
        {% for voucher in vouchers %}
            <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
                {{ voucher.name }} ({{ voucher.domain }}): 
                <code style="background-color: #EDEDED; font-weight: bold;">{{ voucher.code }}</code>
            </p>
        {% endfor %}
        
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            Please find enclosed the invoice for your purchase.
        </p>
        
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            Now you send them your gift - Please find below a proposed email text.
        </p>
        
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            With your support, the internet becomes one big network for the end of AIDS! We'd like to express our sincere thanks and we wish you a great digital Red Ribbon experience.
        </p>
        
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            Your dotHIV Team
        </p>
        
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            <small>The term of the free domain registration is 1 year. On renewing an additional annual registration fee of 160€  will be incurred, whereby at least 90€ will support HIV Projects.</small>
        </p>
    </td>
</tr>
<!-- {% for voucher in vouchers %} -->
<tr width="100%">
    <td valign="top" align="left" style="background:#fafafa; padding: 40px;">
        <h1 style="font-size: 15px; margin: 0; color: #333;">
                    Dear {{ voucher.name }},</h1>
        
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            Today I give you a digital Red Ribbon for your website: {{ voucher.domain }}<br/>
            The charitable .hiv domains generate new funds and new attention for the end of AIDS.
            {% if domain %}We've joined the .hiv moment with {{ domain }}.{% endif %}
            <br/>
            The <a href="https://www.youtube.com/watch?v=l3ZHd8qbSpE">.hiv movie</a> explains dotHIV's 
            work at a glance. You will find further information at <a href="https://click4life.hiv">click4life.hiv</a>.
        <p>
                    
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            You can register your own domain for free at <a href="http://www.domaindiscount24.com/en">Domaindiscount24</a>, dotHIV's affiliated Registrar, with the following voucher code:
        </p>
        
        <p style="text-align: center;">
            <code style="background-color: #EDEDED; padding: 0.5em; font-weight: bold;">{{ voucher.code }}</code>
        </p>
        
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            Most effective within the next 24 hours!
        </p>
        
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            It is now time to commence a new movement. What do you think? Will you participate and spread the word about the digital Red Ribbon? Just three small steps will direct you to <a href="http://payitforward.hiv">payitforward.hiv</a>.
        </p>
        
        <ol style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            <li>Pass on the joy and give a .hiv domain to 3 friends/ clients/ business partners. You can acquire voucher codes at <a href="http://payitforward.hiv">payitforward.hiv</a> at the price of 160€ plus VAT. At least 90€ will support charitable HIV Projects.</li>
            <li>Spread the word on facebook and/ or twitter using hashtag #dotHIV and the links to the presentees.</li>
            <li>Send the presentees your love and their own voucher code with a personal email.</li>
        </ol>
                
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            I would love to see you wearing your own digital Red Ribbon. Let us together set a sign for the end of AIDS.
        </p>
        
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            Yours,<br/>
            {{ firstname }} {{ surname }}
        </p>
    </td>
</tr>
<!-- {% endfor %} -->
<tr width="100%">
    <td valign="top" align="left" style="background:#fff; padding: 40px;">
            
        <h2>Invoice</h2>
        
        <p>
            #{{ invoice.no }}<br/>
            {{ invoice.created }}
        </p>
        
        <p>
            {{ invoice.fullname }}<br/>
            {{ invoice.address1 }}<br/>
            {{ invoice.address2 }}<br/>
            {{ invoice.country }}<br/>
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
