## Web Cache Deception Automation in Burp Suite 
#### <em>Extentions: AutoRepeater and Logger++</em>


## AutoRepeater Replacement Configuration
 
1) Replace nonexistent with valid static files:

    ```
    Type: Reqeust Frist Line
    Match: ([^/\s]+\.(?:jpg|png|gif|css|js))
    Replace: nonexistent.js
    Witch: Replace Frist
    Regex Match: Enabled
    ```
    
## Logger++ Filter For AutoRepeater Local File Inclusion

    Request.Path CONTAINS "nonexistent.js" AND !(Response.Status == 404) AND Response.Headers CONTAINS "Age: "
    

<h4><em>Happy Hunting ;) </em><h4>
