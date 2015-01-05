---
layout: click4life-de
---

{% raw %}
<tr width="100%" itemscope itemtype="http://schema.org/EmailMessage">
    <td valign="top" align="left" style="background:#fff; padding: 40px;" itemprop="action" itemscope itemtype="http://schema.org/ViewAction">
        <h1 style="font-size: 20px; margin: 0; color: #333;">
            Hallo {{ change.user.firstname }} {{ change.user.surname}},</h1>

        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            Sie haben eine Änderung an Ihrem Nutzerkonto angefordert, die von Ihnen bestätigt werden muss: 
        </p>
        {% if change.properties.email is defined %}
            <dl>
                <dt>Neue E-Mail-Adresse</dt>
                <dd>{{ change.properties.email }}</dd>
            </dl>
        {% endif %}
        
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            Bitte geben Sie diesen Token auf Ihrer Profilseite ein, um diese Änderung zu bestätigen: 
        </p>
        
        <p style="text-align: center;">
            <code style="background-color: #EDEDED; padding: 0.5em; font-weight: bold;">{{ change.token }}</code>
        </p>
    </td>
</tr>
{% endraw %}
