## Sensitive Data Exposure Automation in Burp Suite 
#### <em>Extentions: Logger++</em>

    
## Logger++ Filter For Sensitive Data Exposure

    Response.Body == /(?i)([a-z0-9]+){0,}((_|-){0,}(\\s){0,})(APIkey|secret|accesstoken|apiToken|localhost)(\\s){0,}(=|:|is|>){1,}/ AND Response.Headers CONTAINS "application/javascript"
    

<h4><em>Happy Hunting ;) </em><h4>
