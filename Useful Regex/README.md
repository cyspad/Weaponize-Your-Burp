## Useful Regular Expression


   1) URL Patterns

      ```(?:http|ftp|https):\/\/(?:[\w_-]+(?:(?:\.[\w_-]+)+))(?:[\w.,@?^=%&:\/~+#-]*[\w@?^=%&\/~+#-])```
   2) Sensetive Data Exposure Keywords

      ```(?i)([a-z0-9]+){0,}((_|-){0,}(\\s){0,})(APIkey|authtoken|creds|secret|secretKey|password|accessToken|token|api|apiToken)(\\s){0,}(=|:|is|>){1,} ```
   3) JSON Values
      ```:"([^"]+)"```
