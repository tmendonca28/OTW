# Level 8
Upon viewing the source file, I see a bit of code in PHP that looks interesting:  
<code>$encodedSecret = 
"3d3d516343746d4d6d6c315669563362";

function encodeSecret($secret) {  
     return bin2hex(strrev(base64_encode($secret)));  
    }
</code>

I decided to rewrite the code in an online PHP IDE so as to get encode the secret and got the following: 

Reversing the above looks as below, passing in the encodedSecret to derive the secret:  
<code>
$secret = '3d3d516343746d4d6d6c315669563362';  
$ans = base64_decode(strrev(hex2bin($secret)));  
print($ans)
</code>

This gives the following, oubWYf2kBq  
Access granted. The password for natas9 is <ins>W0mMhUcRRnG8dcghE4qvk3JA9lGt8nDl</ins>