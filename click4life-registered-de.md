---
layout: click4life-de
---

{% assign ownerName = '{{ ownerName }}' %}
{% assign domainName = '{{ domainName }}' %}
{% assign loginLink = '{{ loginLink }}' %}
{% assign claimToken = '{{ claimToken }}' %}

<tr width="100%" itemscope itemtype="http://schema.org/EmailMessage">
    <td valign="top" align="left" style="background:#fff; padding: 40px;" itemprop="action" itemscope itemtype="http://schema.org/ViewAction">
        <h1 style="font-size: 20px; margin: 0; color: #333;">
            Hallo {{ ownerName }}, </h1>

        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            Herzlichen Dank, dass Sie sich für eine .hiv Adresse entschieden haben. </p>

        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            <strong>{{ domainName }}</strong> ist Ihre digitale Rote Schleife!<br> Wir hoffen, Sie
            nutzen sie mit Stolz. </p>

        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            Ihre .hiv Webseite kann helfen, Leben zu retten. dotHIV belohnt jeden Besuch mit einer
            kleine Spende an HIV Organisationen auf der ganzen Welt. Organisationen wie 'We actX for
            Hope' aus Ruanda, die betroffene Frauen dabei hilft, gesunde Kinder zur Welt zu bringen und
            großzuziehen. </p>

        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            Alles was es dazu braucht, ist Ihre Teilnahme am dotHIV Mikro-Spenden-Programm: </p>

        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">

            <a itemprop="url" href="{{ loginLink }}" style="border-radius: 3px; -moz-border-radius: 3px; -webkit-border-radius: 3px; background: #e00073; color: #fff; cursor: pointer; display: block; font-weight: 700; font-size: 16px; line-height: 1.25em; margin: 24px auto 24px; padding: 10px 18px; text-decoration: none; width: 180px; text-align: center;">
                <span itemprop="name">Log in</span> </a>

        </p>

        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333; text-align: center;">
            Ihr Token: </p>

        <p style="text-align: center;">
            <code style="background-color: #EDEDED; padding: 0.5em; font-weight: bold;">{{ claimToken }}</code>
        </p>

        <ol style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            <li itemprop="description">Loggen Sie sich in Ihr .hiv Profil ein indem Sie auf den obigen
                Link klicken. (14 Tage gültig)
            </li>
            <li>Aktivieren Sie Ihre .hiv-Domain mit dem Token.</li>
            <li>Gestalten Sie Ihren Clickcounter nach Ihrem Geschmack and Ihren Anforderungen.</li>
            <li>Integrieren Sie ihn auf Ihrer .hiv domain.</li>
        </ol>

        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">

            In nur 10 Minuten wird Ihre Webseite so zum Teil der dotHIV Bewegung. Und lässt Ihre
            Seitenbesucher Anteil nehmen an Ihrem Engagement. </p>

        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            Erfahren Sie mehr über .hiv Adressen und die gemeinnützige Arbeit der dotHIV Initiative
            unter <a href="https://click4life.hiv/">click4life.hiv</a>. </p>

        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            <em>Zusammen</em>, können wir AIDS besiegen. </p>
    </td>
</tr>
