---
layout: tld-text-de
---

{% raw %}
Hallo {{ firstname }} {{ surname }},

Vielen Dank, dass Sie den Click-Counter konfiguriert haben. Sie sind nur noch einen kleinen Schritt davon entfernt, Teil des .hiv Mikro-Spenden-Programms zu werden.

{% if forward %}
Es gibt zwei Wege um sicherzustellen, dass der Click-Counter auf Ihrer Domain {{ domainName }} funktioniert und dass Ihre Besucher nach {{ forward }} weitergeleitet werden:

\#\# 1) Ein neuer Webspace für {{ domainName }}

Richten Sie einen Webspace für die Domain ein und platzieren Sie die angehängte index.html im Root-Verzeichnis des Webspaces.

 - ODER -

\#\# 2) Richten Sie einen CNAME für {{ domainName }} ein

Bei den meisten Registraren können Sie CNAME-Einträge für Ihre .hiv-Domain einrichten. Verwenden Sie einfach iframe.clickcounter.hiv als CNAME für Ihre www-Subdomain.

Da man keine CNAME-Einträge für Basis-Domains einrichten kann, müssen Sie zusätzlich eine Weiterleitung von {{ domainName }} nach www.{{ domainName }} einrichten.

Bitte beachten Sie, dass es bis zu 24 Stunden dauern kann, bis diese Änderungen aktiv werden, sollten Sie Ihre .hiv bereits einmal aufgerufen haben.

Auf dieser Seite haben wir Registrar-spezifische Anleitungen zum Anlegen von CNAME-Einträgen zusammengestellt: https://tld.hiv/en/c/howto/cname 

{% else %}
Es ist nur ein kleiner Ausflug in den Quellcode Ihrer Homepage: Damit der Click-Counter auf Ihrer Domain <strong>{{ domainName }}</strong> angezeigt wird, müssen Sie folgende Zeile Code direkt vor dem </body>-Tag ihrer Seite einbinden:

&lt;script src=&quot;//dothiv-registry.appspot.com/static/clickcounter.min.js&quot; type=&quot;text/javascript&quot;&gt;<br/>&lt;/script&gt;
{% endif %}

\#\# Erledigt?

Wunderbar! Nun hilft jeder Besuch auf Ihrer .hiv Domain dabei, AIDS ein Ende zu setzen. 

\#\# Need help?

Sollten Sie Hilfe bei der Installation des Click-Counters haben, zögern Sie nicht, sich an uns zu wenden: support@tld.hiv

{% endraw %}
