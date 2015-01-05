---
layout: click4life-en
---

{% raw %}
<tr width="100%" itemscope itemtype="http://schema.org/EmailMessage">
    <td valign="top" align="left" style="background:#fff; padding: 40px;" itemprop="action" itemscope itemtype="http://schema.org/ViewAction">
        <h1 style="font-size: 20px; margin: 0; color: #333;">
            Hello {{ firstname }}, </h1>
            
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            Thank you for configuring the click-counter! You are only a tiny little step away from joining the .hiv micro-donation program.
        </p>
        
        {% if forward %}
        
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            There are two different ways to make sure that the click-counter works at your domain <strong>{{ domainName }}</strong> and your visitors are forwarded to <em>{{ forward }}</em>:
        </p>
        
        <h2 style="font-size: 16px; margin: 0; color: #333;">1) A new webspace for {{ domainName }}</h2>
        
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            Configure a webspace for the domain and place the attached <code style="padding: 0px 4px; color: #d14; background-color: #f7f7f9; border: 1px solid #e1e1e8;">index.html</code> in the root folder of the webspace.
        </p>
        
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            <strong>-OR-</strong>
        </p>
        
        <h2 style="font-size: 16px; margin: 0; color: #333;">2) Configure a CNAME for {{ domainName }}</h2>
        
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            At most registrars, you can configure CNAME records for your .hiv domain. Just use <code style="padding: 0px 4px; color: #d14; background-color: #f7f7f9; border: 1px solid #e1e1e8;">iframe.clickcounter.hiv</code> as the CNAME for your <code style="padding: 0px 4px; color: #d14; background-color: #f7f7f9; border: 1px solid #e1e1e8;">www</code> subdomain.</p>

        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            As you cannot configure CNAME records for apex domains, you need to configure a redirect for <code style="padding: 0px 4px; color: #d14; background-color: #f7f7f9; border: 1px solid #e1e1e8;">{{ domainName }}</code> to <code style="padding: 0px 4px; color: #d14; background-color: #f7f7f9; border: 1px solid #e1e1e8;">www.{{ domainName }}</code> additionally.
        </p>
        
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            <em>Please keep in mind that if you have visited your .hiv domain before it may take up to 24 hours before you can see the changes.</em>
        </p>
        
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            We are compiling registrar-specific guides on how to configure a CNAME record <a href="https://tld.hiv/en/c/howto/cname" style="color: #3d90b5;">at this page</a>. 
        </p>
                
        {% else %}
        
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            It's just a small excursion into the code of your homepage: In order for the click-counter to be shown at your domain <strong>{{ domainName }}</strong> you need to include the following line of code just before the <code style="padding: 0px 4px; color: #d14; background-color: #f7f7f9; border: 1px solid #e1e1e8;">&lt;/body&gt;</code> tag of your site:
        </p>
        
        <pre style="padding: 2px 4px; color: #d14; background-color: #f7f7f9; border: 1px solid #e1e1e8;">&lt;script<br/>    src=&quot;//dothiv-registry.appspot.com/static/clickcounter.min.js&quot;<br/>    type=&quot;text/javascript&quot;&gt;<br/>&lt;/script&gt;</pre>
        
        {% endif %}
        
        <h2 style="font-size: 16px; margin: 0; color: #333;">Done?</h2>
        
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">
            Wonderful! Now every visit on your .hiv domain counts to help end AIDS.
        </p>
        
        <h2 style="font-size: 16px; margin: 0; color: #333;">Need help?</h2>
        
        <p style="font: 15px/1.25em 'Helvetica Neue', Arial, Helvetica; color: #333;">If you need assistance for installing the click-counter do not hesitate to contact us at <a href="mailto:support@tld.hiv" style="color: #3d90b5;">support@tld.hiv</a>
        </p>

    </td>
</tr>
{% endraw %}
