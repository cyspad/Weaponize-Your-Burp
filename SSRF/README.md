## Server Side Request Forgery Automation in Burp Suite
#### <em>Extentions: AutoRepeater</em>


## AutoRepeater Replacement Configuration 
1) Replace any URL Patterns in Request (Headers and Body) with your Out Of Band Server:

    ```
    Type: Request String
    Match: (https?:\/\/(?:www\.|(?!www))[a-zA-Z0-9][a-zA-Z0-9-]+[a-zA-Z0-9]\.[^\s]{2,}|www\.[a-zA-Z0-9][a-zA-Z0-9-]+[a-zA-Z0-9]\.[^\s]{2,}|https?:\/\/(?:www\.|(?!www))[a-zA-Z0-9]+\.[^\s]{2,}|www\.[a-zA-Z0-9]+\.[^\s]{2,})
    Replace: https://<Your-OoB-Server>
    Which: Replace All
    Regex Match: Enabled
    ```
    
<h4><em>Happy Hunting ;) </em><h4>
