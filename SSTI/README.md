## Server Side Template Injection Automation in Burp Suite
#### <em>Extentions: AutoRepeater and Logger++ </em>


## AutoRepeater Replacement Configuration 
1) Replace any Parameters Value with others CSTI Payload:

    ```
    Type: Request Param Value
    Match: .*
    Replace: [2548*70]
    Which: Replace All
    Regex Match: Enabled
    ```
    
    And Your Custom Payloads
2) Logger++ Filter For AutoRepeater Response of SSTI Payload

    ``` Response.Body CONTAINS "178360" ```
    And Repsonse of Your Custom others Patloads Filters
<h4><em>Happy Hunting ;) </em><h4>
