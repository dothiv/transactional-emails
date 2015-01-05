---
layout: tld-text-de
---

{% raw %}
Hallo {{ change.user.firstname }} {{ change.user.surname}},

Sie haben eine Änderung an Ihrem Nutzerkonto angefordert, die von Ihnen bestätigt werden muss:

{% if change.properties.email is defined %}
Neue E-Mail-Adresse: {{ change.properties.email }}
{% endif %}

Bitte geben Sie diesen Token auf Ihrer Profilseite ein, um diese Änderung zu bestätigen:

{{ change.token }}

{% endraw %}
