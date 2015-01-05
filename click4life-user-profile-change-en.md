---
layout: click4life-en
---

{% raw %}
<tr width="100%" itemscope itemtype="http://schema.org/EmailMessage">
    <td valign="top" align="left" style="background:#fff; padding: 40px;" itemprop="action" itemscope itemtype="http://schema.org/ViewAction">
        <h1 style="font-size: 20px; margin: 0; color: #333;">
            Hello {{ change.user.firstname }}, </h1>

        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            You've requested a change to your account which requires a confirmation by you: 
        </p>
        {% if change.properties.email is defined %}
            <dl>
                <dt>New email address</dt>
                <dd>{{ change.properties.email }}</dd>
            </dl>
        {% endif %}
        
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            Please enter this token on your profile page to confirm this change. 
        </p>
        
        <p style="text-align: center;">
            <code style="background-color: #EDEDED; padding: 0.5em; font-weight: bold;">{{ change.token }}</code>
        </p>
    </td>
</tr>
{% endraw %}
