## CORS Misconfiguration Automation in Burp Suite 
#### <em>Extentions: AutoRepeater and Logger++</em>


## AutoRepeater Replacement Configuration
1) Add Origin Header:

    ```
    Type: Add Header
    Match: 
    Replace: Origin: https://cyspad.info
    Which: Replace Frist
    Regex Match: Disabled
    ```
    
2) Replace Origin Header:

    ```
    Type: Request Header
    Match: Origin:
    Replace: Origin: https://cyspad.info
    Witch: Replace Frist
    Regex Match: Disabled
    ```
    
## Logger++ Filter For AutoRepeater CORS Misconfiguration

    Response.Headers CONTAINS "Access-Control-Allow-Origin: https://cyspad.info" AND Response.Headers CONTAINS "Access-Control-Allow-Credentials: true"
    

<h4><em>Happy Huntnting ;) </em><h4>
