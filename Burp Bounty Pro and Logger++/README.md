## Burp Bounty Pro and Logger++ Methodology 
#### <em>Extentions: Burp Bounty Pro and Logger++ </em>

## Methodology

Burp Bounty Pro and Logger++ can be said to be the most popular Burp Suite extensions.

Logger++ is a extension with advanced filtering capability for HTTP history requests and responses

Burp Bounty Pro is also a extension that has the ability to write active and passive profiles, and it also has complete profiles for each vulnerability.

As a result, the combination of these two extensionsin the hunting methodology using Burp Suite has become very powerful and if the hunter implements this methodology correctly, he will find much more power in hunting vulnerabilities.

The whole trick of the methodology is as follows:
Using your mindset to discover vulnerabilities, write a filter for requests. For example, for the SSRF vulnerability, write a filter that identifies parameters that have the URL like pattern (go to the SSRF section in this repository)

When the filter is applied, select the requests and give Burp Bounty Pro to scan all SSRF tags :)

<h4><em>Happy Hunting ;) </em><h4>
