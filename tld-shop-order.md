---
layout: tld
---

{% raw %}
<tr width="100%">
    <td valign="top" align="left" style="background:#fff; padding: 40px;">
        <h1 style="font-size: 20px; margin: 0; color: #333;">
            Dear {{ firstname }} {{ lastname }},</h1>
            
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            Thank you for registering a .hiv domain name.
        </p>
            
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            {{ domain }} is your digital Red Ribbon! Use it with pride.
        </p>
        
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            dotHIV rewards every visit with a small donation to HIV organizations around the world, like ‘WE ACTx for hope’ from Rwanda, which helps women living with HIV to give birth to and raise healthy babies.
        </p>
        
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            For technical reasons, it might take up to 48 hours until {{ domain }} is online. So please bear with us. 
        </p>
        
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            To adapt your Click-Counter and access your Click Stats, you can log into your customer account with your email {{ email }} <a href="https://click4life.hiv/en/account">here</a>.
        </p>
        
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            Now let the world know about the second entrance to your homepage that helps save lives: Download the “<a href="https://click4life.hiv/en/p/about/getactive#about-getactive-howto">Tell-the-World-Package</a>” with an easy toolbox that helps you to direct your users to {{ domain }}.
        </p>
        
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            Together, we can end AIDS.
        </p>
    </td>
</tr>
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
                <td style="text-align: right; white-space: nowrap;">
                    {{ invoice.item_price }}
                </td>
            </tr>
            {% if invoice.vat_percent %}
                <tr>
                    <td>
                        {{ invoice.vat_percent }}% VAT
                    </td>
                    <td style="text-align: right; white-space: nowrap;">
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
                <td style="text-align: right; white-space: nowrap;">
                    <strong>{{ invoice.total_price }}</strong>
                </td>
            </tr>
            </tfoot>
        </table>
    </td>
</tr>
{% endraw %}
