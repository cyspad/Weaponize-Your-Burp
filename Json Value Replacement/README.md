## Json Values Replacement Automation in Burp Suite
#### <em>Extentions: AutoRepeater</em>


## AutoRepeater Replacement Configuration 
1) Replace any payload in json values canary:

    ```
    Type: Request String or Request Body
    Match: :"([^"]+)"
    Replace: "<canary>"
    Which: Replace All
    Regex Match: Enabled
    ```
You can replace any payload in Replace filed for json values.

<h4><em>Happy Hunting ;) </em><h4>
