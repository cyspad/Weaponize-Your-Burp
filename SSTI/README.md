## Server Side Template Injection Automation in Burp Suite
#### <em>Extentions: AutoRepeater and Logger++ </em>


## AutoRepeater Replacement Configuration 
1) Replace any Parameters Value with SSTI Payload:

    ```
    Type: Request Param Value
    Match: .*
    Replace: {{2548*80}}
    Which: Replace All
    Regex Match: Enabled
    ```
    
2) Logger++ Filter For AutoRepeater Response of SSTI Payload

    ``` Response.Body CONTAINS "203840" ```

<h4><em>Happy Hunting ;) </em><h4>
