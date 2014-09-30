---
layout: tld
---

{% raw %}
<tr width="100%" itemscope itemtype="http://schema.org/EmailMessage">
    <td valign="top" align="left" style="background:#fff; padding: 40px;" itemprop="action" itemscope itemtype="http://schema.org/ViewAction">
        <h1 style="font-size: 20px; margin: 0; color: #333;">
            Hello {{ firstname }}, </h1>

        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;" itemprop="description">
            please click this link to log in: </p>

        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">

            <a itemprop="url" href="{{ loginLink }}" style="border-radius: 3px; -moz-border-radius: 3px; -webkit-border-radius: 3px; background: #3d90b5; color: #fff; cursor: pointer; display: block; font-weight: 700; font-size: 16px; line-height: 1.25em; margin: 24px auto 24px; padding: 10px 18px; text-decoration: none; width: 180px; text-align: center;">
                <span itemprop="name">Log in</span> </a>

        </p>

    </td>
</tr>
{% endraw %}
