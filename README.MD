# Weaponize Your Burp

## Description 
This is a repository about how to Weaponize Burp Suite with extensions for Bug Bounty Hunting.
Burp Suite is an amazing tool for Bug Hunting, Penetration Testing Web Applications.

If a bug hunter or penetration tester can implement his own bug hunting mindset in BurpSuite, he can hunt bugs much more powerfully and faster than before.

According to a tweet I published on Twitter, it has been decided to release the methodology for Weaponize Burp Suite This is the repository for this methodology :)

## Useful Extensions 

   1) Burp Bounty Pro
   2) Logger++ 
   3) AutoRepeater

## Useful Regex

   1) URL Patterns

      ```(?:http|ftp|https):\/\/(?:[\w_-]+(?:(?:\.[\w_-]+)+))(?:[\w.,@?^=%&:\/~+#-]*[\w@?^=%&\/~+#-])```
   2) Sensetive Data Exposure Keywords

      ```(?i)([a-z0-9]+){0,}((_|-){0,}(\\s){0,})(APIkey|authtoken|creds|secret|secretKey|password|accessToken|token|api|apiToken)(\\s){0,}(=|:|is|>){1,} ```
   3) JSON Values
      ```"([^"]+)"```

   4) And ....


# Methodology
## How To Works This Methodology?
In this methodology, we add our custom payloads in AutoRepeater and create a response of Payload filter in Logger++.
So when we are browsing our target website AutoRepeater is replacing payloads in requests and send to server, Logger++ is logs the all AutoRepeater Requests if detect our filters in Logs you send request to Repeater and try to Exploit

## Important Note

I have added examples of each vulnerability in this repository, but you should add more payloads. In the vulnerability examples, I'll show you how to configure and add your own custom payloads to make your burp powerful.

<br>
<img src="https://socialify.git.ci/cyspad/Weaponize-Your-Burp/image?font=KoHo&forks=1&owner=1&pattern=Circuit%20Board&stargazers=1&theme=Dark" alt="Weaponize Your Burp" width="640" height="320" />

