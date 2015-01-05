---
layout: tld-text-en
---

{% raw %}
Hello {{ change.user.firstname }},

You've requested a change to your account which requires a confirmation by you:

{% if change.properties.email is defined %}
New email address: {{ change.properties.email }}
{% endif %}

Please enter this token on your profile page to confirm this change.

{{ change.token }}

{% endraw %}
