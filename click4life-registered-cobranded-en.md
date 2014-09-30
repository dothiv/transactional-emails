---
layout: click4life-cobranded-en
---

{% assign ownerName = '{{ ownerName }}' %}
{% assign domainName = '{{ domainName }}' %}
{% assign loginLink = '{{ loginLink }}' %}
{% assign claimToken = '{{ claimToken }}' %}
{% assign registrar = '{{ registrar }}' %}

<tr width="100%" itemscope itemtype="http://schema.org/EmailMessage">
    <td valign="top" align="left" style="background:#fff; padding: 40px;" itemprop="action" itemscope itemtype="http://schema.org/ViewAction">
        <h1 style="font-size: 20px; margin: 0; color: #333;">
            Hello {{ ownerName }}, </h1>

        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            Thank you for registering a .hiv domain name at {{ registrar }}. </p>

        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            <strong>{{ domainName }}</strong> is your digital Red Ribbon!<br> Use it with pride. </p>

        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            Your .hiv domain can help save lives. dotHIV rewards every visit with a small donation to
            HIV organizations around the world, like 'WE ACTx for hope' from Rwanda, which helps women
            living with HIV to give birth to and raise healthy babies. </p>

        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            To make this work, all you need to do is join dotHIV’s micro donation program: </p>

        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">

            <a itemprop="url" href="{{ loginLink }}" style="border-radius: 3px; -moz-border-radius: 3px; -webkit-border-radius: 3px; background: #e00073; color: #fff; cursor: pointer; display: block; font-weight: 700; font-size: 16px; line-height: 1.25em; margin: 24px auto 24px; padding: 10px 18px; text-decoration: none; width: 180px; text-align: center;">
                <span itemprop="name">Log in</span> </a>

        </p>

        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333; text-align: center;">
            Your token: </p>

        <p style="text-align: center;">
            <code style="background-color: #EDEDED; padding: 0.5em; font-weight: bold;">{{ claimToken }}</code>
        </p>

        <ol style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            <li itemprop="description">Log into your .hiv profile by clicking the link above (valid for
                14 days) 
            </li>
            <li>Claim your .hiv domain name with the token</li>
            <li>Generate a Click-Counter after your wishes and taste.</li>
            <li>Include it on your .hiv domain.</li>
        </ol>

        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">

            It takes no more than 10 minutes, to make your website part of the dotHIV movement and to
            show your website visitors that you care. </p>

        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            Learn more about .hiv domain names and the work of the charitable initiative dotHIV behind
            it at <a href="https://click4life.hiv/">click4life.hiv</a>. </p>

        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            <em>Together</em>, we can end AIDS. </p>
    </td>
</tr>
