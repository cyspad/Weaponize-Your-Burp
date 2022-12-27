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

## Methodology

   1) Set Your AutoRepeater Payloads 
   2) Set AutoRepeater Payloads Response Filters in Logger++
   3) Now Check the Logger++ Logs for Hunting ;)

## Example How to Identify SSTI

### AutoRepeater Configuration
   1) Go to AutoRepeater Tab
   2) Add Replacement 
   3) Set Type to:  Request Params Value
   4) Set Match to: .*
   5) Set Replace to: {{ 40*99 }} or any SSTI Detection Payload
   6) Enable Regex Match

 ### Logger++ Configuration 

   1) Go to Logger++ Tab 
   2) Click on Taggs Button in View Logs tab
   3) Now add your response of your SSTI Payload Filter
       ```Response.Body CONTAINS "3600"```

## How To Works This Methodology?
In this methodology, we add our custom payloads in AutoRepeater and create a response of Payload filter in Logger++.
So when we are browsing our target website AutoRepeater is replacing payloads in requests and send to server, Logger++ is logs the all AutoRepeater Requests if detect our filters in Logs you send request to Repeater and try to Exploit

## Sensitive Information Disclosure 

   1) Go Logger++ Tab
   2) Go Grep Value Tab
   3) Paste the Sensitive Data Exposure Regex in filed


# Important Note
In this repository, I can't give you examples of all the vulnerabilities, I explained how to Weaponize Your Burp with an SSTI example in this repository, and I leave the other vulnerabilities to you.


<img src="https://socialify.git.ci/cyspad/Weaponize-Your-Burp/image?font=KoHo&forks=1&owner=1&pattern=Circuit%20Board&stargazers=1&theme=Dark" alt="Weaponize Your Burp" width="640" height="320" />

