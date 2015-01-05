---
layout: click4life-de
---

{% raw %}
<tr width="100%" itemscope itemtype="http://schema.org/EmailMessage">
    <td valign="top" align="left" style="background:#fff; padding: 40px;" itemprop="action" itemscope itemtype="http://schema.org/ViewAction">
        <h1 style="font-size: 20px; margin: 0; color: #333;">
            Hallo {{ firstname }} {{ surname }}, </h1>
            
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            Vielen Dank, dass Sie den Click-Counter konfiguriert haben. Sie sind nur noch einen kleinen Schritt davon entfernt, Teil des .hiv Mikro-Spenden-Programms zu werden.
        </p>
        
        {% if forward %}
        
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            Es gibt zwei Wege um sicherzustellen, dass der Click-Counter auf Ihrer Domain <strong>{{ domainName }}</strong> funktioniert und dass Ihre Besucher nach <em>{{ forward }}</em> weitergeleitet werden:
        </p>
        
        <h2 style="font-size: 16px; margin: 0; color: #333;">1) Ein neuer Webspace für {{ domainName }}</h2>
        
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            Richten Sie einen Webspace für die Domain ein und platzieren Sie die angehängte <code style="padding: 0px 4px; color: #d14; background-color: #f7f7f9; border: 1px solid #e1e1e8;">index.html</code> im Root-Verzeichnis des Webspaces.
        </p>
        
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            <strong>- ODER -</strong>
        </p>
        
        <h2 style="font-size: 16px; margin: 0; color: #333;">2) Richten Sie einen CNAME für {{ domainName }} ein</h2>
        
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            Bei den meisten Registraren können Sie CNAME-Einträge für Ihre .hiv-Domain einrichten. Verwenden Sie einfach <code style="padding: 0px 4px; color: #d14; background-color: #f7f7f9; border: 1px solid #e1e1e8;">iframe.clickcounter.hiv</code> als CNAME für Ihre <code style="padding: 0px 4px; color: #d14; background-color: #f7f7f9; border: 1px solid #e1e1e8;">www</code>-Subdomain.
        </p>

        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            Da man keine CNAME-Einträge für Basis-Domains einrichten kann, müssen Sie zusätzlich eine Weiterleitung von <code style="padding: 0px 4px; color: #d14; background-color: #f7f7f9; border: 1px solid #e1e1e8;">{{ domainName }}</code> nach <code style="padding: 0px 4px; color: #d14; background-color: #f7f7f9; border: 1px solid #e1e1e8;">www.{{ domainName }}</code> einrichten.
        </p>
        
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            <em>Bitte beachten Sie, dass es bis zu 24 Stunden dauern kann, bis diese Änderungen aktiv werden, sollten Sie Ihre .hiv bereits einmal aufgerufen haben.</em>
        </p>
        
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
             <a href="https://tld.hiv/en/c/howto/cname" style="color: #3d90b5;">Auf dieser Seite</a> haben wir Registrar-spezifische Anleitungen zum Anlegen von CNAME-Einträgen zusammengestellt. 
        </p>
                
        {% else %}
        
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            Es ist nur ein kleiner Ausflug in den Quellcode Ihrer Homepage: Damit der Click-Counter auf Ihrer Domain <strong>{{ domainName }}</strong> angezeigt wird, müssen Sie folgende Zeile Code direkt vor dem <code style="padding: 0px 4px; color: #d14; background-color: #f7f7f9; border: 1px solid #e1e1e8;">&lt;/body&gt;</code>-Tag ihrer Seite einbinden:
        </p>
        
        <pre style="padding: 2px 4px; color: #d14; background-color: #f7f7f9; border: 1px solid #e1e1e8;">&lt;script<br/>    src=&quot;//dothiv-registry.appspot.com/static/clickcounter.min.js&quot;<br/>    type=&quot;text/javascript&quot;&gt;<br/>&lt;/script&gt;</pre>
        
        {% endif %}
        
        <h2 style="font-size: 16px; margin: 0; color: #333;">Erledigt?</h2>
        
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            Wunderbar! Nun hilft jeder Besuch auf Ihrer .hiv Domain dabei, AIDS ein Ende zu setzen. 
        </p>
        
        <h2 style="font-size: 16px; margin: 0; color: #333;">Need help?</h2>
        
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            Sollten Sie Hilfe bei der Installation des Click-Counters haben, zögern Sie nicht, sich an uns zu wenden: <a href="mailto:support@tld.hiv" style="color: #3d90b5;">support@tld.hiv</a>
        </p>

    </td>
</tr>
{% endraw %}
