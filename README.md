> Any-Proxy can help you browse any website with a perfect reverse proxy  
> No need for complicated procedures, less than 10KB file, excellent compatibility
  
> Added easy password access, default password web  
> The latest version changes the exit command to ~q, which will be more convenient when typing.  
> Pseudo-static needs to be configured. The nginx pseudo-static rules are as follows:  
> if ( !-e $request_filename) {  
> rewrite ^/(.*)$ /index.php?$1 last;  
> break;  
> }
  
> index.php external links, external link pictures, external link static files and other requests do not go through Any-Proxy, and the target domain name will not be displayed in the address bar.  
> index_all.php is different from the traditional version. The address bar will display the target domain name, and its performance is not as good as the former.  
> index_all.php All requests for external links, external link pictures, external link static files, etc. go through Any-Proxy
  
> Support POST, Cookie, https/http can be used  
> Supports forged IP. If the $anyip value is 1, the server IP header will be sent. If the value is 2, a random IP will be sent. If the value is 3, the client IP will be sent.  
> The problem of Chinese garbled characters has been solved and automatic conversion
  
> Enter ~q at the end of the current link to exit the current page and return to the home page.  
> Add the link address after the domain name to access:  
> https://www.com/http://+the link to be accessed (the target link must add http(s)://)
  
> Such as: https://www.com/http://ip38.com/
  
![Image](https://p.pstatp.com/origin/fe81000376fc445be379)  
![Image](https://p.pstatp.com/origin/137b90001905c99862df3)  

> Based on: https://github.com/koala0529/reverse-proxy-php modified  
> Please do not use it for illegal purposes, otherwise you will be responsible for the consequences.
