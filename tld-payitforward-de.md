---
layout: tld-de
---

{% raw %}
<tr width="100%">
    <td valign="top" align="left" style="background:#fff; padding: 40px;">
        <h1 style="font-size: 20px; margin: 0; color: #333;">
            Hallo {{ firstname }} {{ surname }},</h1>
            
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            Vielen Dank, dass Sie die digitale rote Schleife weitertragen!<br/>
            Dies sind die Gutschein-Codes für Ihre Freunde.
        </p>
            
        {% for voucher in vouchers %}
            <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
                {{ voucher.name }} ({{ voucher.domain }}): 
                <code style="background-color: #EDEDED; font-weight: bold;">{{ voucher.code }}</code>
            </p>
        {% endfor %}
        
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            Die Rechnung für Ihren Einkauf finden Sie im Anhang.
        </p>
        
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            Nun senden Sie ihnen Ihr Geschenk – Einen Textvorschlag für Ihre Email haben wir weiter unten für Sie vorbereitet.
        </p>
        
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            Mit Ihrer Hilfe wird das Internet zu einem immer größer werdenden Netzwerk für das Ende von AIDS! Wir sagen herzlichen Dank und wünschen viel Freude an Ihrer eigenen digitalen Roten Schleife.
        </p>
        
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            Ihr dotHIV Team
        </p>
        
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            <small>Die Laufzeit der kostenlosen Domainregistrierung beträgt 1 Jahr. Bei Verlängerung fallen pro Folgejahr weitere 160 € Registrierungsgebühr an, von der mindestens 90 € an HIV Projekte gehen.</small>
        </p>
    </td>
</tr>
<!-- {% for voucher in vouchers %} -->
<tr width="100%">
    <td valign="top" align="left" style="background:#fafafa; padding: 40px;">
        <h1 style="font-size: 15px; margin: 0; color: #333;">
            Hallo {{ voucher.name }},</h1>
        
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            heute schenke ich Dir eine digitale rote Schleife für Deine Website: {{ voucher.domain }}<br/>
            Die gemeinnützigen .hiv-Domains schaffen neue Gelder und neue Aufmerksamkeit für das Ende von AIDS. 
            {% if domain %}Wir sind mit {{ domain }} dabei.{% endif %}
            <br/>
            Das <a href="https://www.youtube.com/watch?v=l3ZHd8qbSpE">.hiv Video</a> erklärt die Arbeit von dotHIV auf einen Blick. 
            Weitere Infos findest Du auf <a href="https://click4life.hiv">click4life.hiv</a>.
        <p>
                    
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            Bei dotHIV's Parterregistrar <a href="http://www.domaindiscount24.com/de">Domaindiscount24</a> kannst Du Deine Domain mit diese Gutscheincode kostenfrei registrieren:
        </p>
        
        <p style="text-align: center;">
            <code style="background-color: #EDEDED; padding: 0.5em; font-weight: bold;">{{ voucher.code }}</code>
        </p>
        
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            Am besten in den nächsten 24 Stunden!
        </p>
        
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            Nun gilt es, eine neue Bewegung zu starten. Wie wär’s? Machst Du mit und trägst die digitale Rote Schleife weiter? Es sind nur drei kleine Schritte auf <a href="http://payitforward.hiv">payitforward.hiv</a>
        </p>
        
        <ol style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            <li>Gib die Freude weiter und spendiere 3 Freunden / Kunden / Geschäftspartnern eine .hiv-Domain. 
            Auf <a href="http://payitforward.hiv">payitforward.hiv</a> sind die Gutschein-Codes für 160 € zzgl. MwSt. zu erwerben. 
            Mindestens 90 € pro Domain gehen an gemeinnützige HIV-Projekte.</li>
            <li>Lass Facebook und/oder Twitter davon wissen, mit Hashtag #dotHIV und einem Link auf die Beschenkten.</li>
            <li>Schicke den Beschenkten ihren Code per E-Mail, die Freude macht. So wie diese hier.</li>
        </ol>
                
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            Ich freue mich sehr, wenn Du Deine digitale Rote Schleife trägst. Gemeinsam setzen wir ein Zeichen für das Ende von AIDS!

        </p>
        
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            Dein {{ firstname }} {{ surname }}
        </p>
    </td>
</tr>
<!-- {% endfor %} -->
<tr width="100%">
    <td valign="top" align="left" style="background:#fff; padding: 40px;">
            
        <h2>Rechnung</h2>
        
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
                        {{ invoice.vat_percent }}% MwSt.
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
                    <strong>Summe</strong>
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
