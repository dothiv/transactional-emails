---
layout: tld-text-en
---

{% raw %}
Hello {{ firstname }},

Thank you for configuring the click-counter!

{% if forward %}
In order for the click-counter to be shown at your domain {{ domainName }} and the visitor is forwarded to {{ forward }} you need to ensure that the click-counter code is served to the visitor. You have two ways of achieving this:

\#\# Configure a webspace

Configure a webspace for the domain and place the attached index.html in the root folder of the webspace.

\#\# -OR- Configure a CNAME

If you can configure CNAME records for your .hiv domain at your registrar, you can use {{ secondLevelDomainName }}.iframe.click4life.hiv as the CNAME for your www subdomain.

As you cannot configure CNAME records for apex domains, you need to configure a redirect for {{ domainName }} to www.{{ domainName }} additionally.

Please keep in mind that if you have visited your .hiv domain before it may take up to 24 hours before you can see the changes.

We are compiling registrar-specific guides on how to configure a CNAME record at this page: https://tld.hiv/en/c/howto/cname 

{% else %}
In order for the click-counter to be shown at your domain {{ domainName }} you need to include the following line of code just before the </body> tag of your site:

&lt;script src="//dothiv-registry.appspot.com/static/clickcounter.min.js" type="text/javascript"&gt;&lt;/script&gt;
{% endif %}

\#\# Need help?

If you need assistance for installing the click-counter do not hesitate to contact us at support@tld.hiv

{% endraw %}
