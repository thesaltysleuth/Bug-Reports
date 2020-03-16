## Bug Report #1

Vulnerability: Reflected Cross Site Scripting(XSS) 
Affected domain: http://pngimg.com/search

Steps to reproduce:
1.	Open http://pngimg.com/search in browser
2.	In the search tab paste the following code:

       <script>alert(1)</script>

3.	A popup with the text 1 appears.

**Note: Screenshots attached as POC(Proof of Concept)**


Impact:
With the help of xss a hacker or attacker can perform social engineering on users by redirecting them from real website to fake one. hacker can steal their cookies and download a malware on their system, and there are many more attacking scenarios a skilled attacker can perform with xss.
For example, instead of donating to your site, an attacker can redirect a victim to pay the attacker, as demonstrated through the screenshots.

![POC1](https://github.com/thesaltysleuth/Bug-Reports/blob/master/POC%20Screenshots/Screenshot%202020-03-16%2019_37_09.png)
![POC2](https://github.com/thesaltysleuth/Bug-Reports/blob/master/POC%20Screenshots/Screenshot%202020-03-16%2019_37_39.png)

