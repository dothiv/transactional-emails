---
layout: click4life-en
---

{% assign firstname = '{{ firstname }}' %}
{% assign domain = '{{ domain }}' %}

<tr width="100%" itemscope itemtype="http://schema.org/EmailMessage">
    <td valign="top" align="left" style="background:#fff; padding: 40px;" itemprop="action" itemscope itemtype="http://schema.org/ViewAction">
        <h1 style="font-size: 20px; margin: 0; color: #333;">
            Hello {{ firstname }}, </h1>

        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            Thank you for purchasing a premium subscription for your .hiv domain name. </p>

        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            We have confirmed your payment and your premium Click-Counter is now active for your domain <strong>{{ domain }}</strong>. </p>

        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            Thanks again for your support. </p>

    </td>
</tr>
