---
layout: tld-text-en
---

{% raw %}
Hello {{ firstname }},

Thank you for configuring the click-counter! You are only a tiny little step away from joining the .hiv micro-donation.

{% if forward %}
There are two different ways to make sure that the click-counter works at your domain <strong>{{ domainName }}</strong> and your visitor is forwarded to {{ forward }}:

\#\# 1) A new webspace for {{ domainName }}

Configure a webspace for the domain and place the attached index.html in the root folder of the webspace.

 -OR-

\#\# 2) Configure a CNAME {{ domainName }}

At most registrars, you can configure CNAME records for your .hiv domain. Just use {{ secondLevelDomainName }}.iframe.click4life.hiv as the CNAME for your www subdomain.

As you cannot configure CNAME records for apex domains, you need to configure a redirect for {{ domainName }} to www.{{ domainName }} additionally.

Please keep in mind that if you have visited your .hiv domain before it may take up to 24 hours before you can see the changes.

We are compiling registrar-specific guides on how to configure a CNAME record at this page: https://tld.hiv/en/c/howto/cname 

{% else %}
It's just a small excursion into the code of your homepage: In order for the click-counter to be shown at your domain {{ domainName }} you need to include the following line of code just before the </body> tag of your site:

&lt;script src="//dothiv-registry.appspot.com/static/clickcounter.min.js" type="text/javascript"&gt;&lt;/script&gt;
{% endif %}

\#\# Done?

Wonderful! Now every visit on your .hiv domain counts to help end AIDS.

\#\# Need help?

If you need assistance for installing the click-counter do not hesitate to contact us at support@tld.hiv

{% endraw %}
