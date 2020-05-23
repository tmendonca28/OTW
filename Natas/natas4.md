# Level 4
The following message shows up:  
Access disallowed. You are visiting from "" while authorized users should come only from "http://natas5.natas.labs.overthewire.org/".  
After clicking the refresh page button the message changes to: Access disallowed. You are visiting from "http://natas4.natas.labs.overthewire.org/index.php" while authorized users should come only from "http://natas5.natas.labs.overthewire.org/".  
Initially it showed You are visiting from "". This implies that certain data is populating the first set of quotations.  
Upon inspecting the page in Firefox, I edited and resent a request adding the HTTP Referer header using the Network tab. The response then bears the message as seen below:

Access granted. The password for natas5 is <ins>iX6IOfmpN7AYOQGPwtn3fXpbaJVJcHfq</ins>