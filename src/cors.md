#Same Origin Policy
https://en.wikipedia.org/wiki/Same-origin_policy



#CORS (Cross-Origin Resource Sharing)
同源: 协议，域名，端口相同
同源策略: 由Netscape提出的一个著名的安全策略，现在所有支持JavaScript的浏览器都会使用这个策略。
https://www.w3.org/TR/cors/




#nginx configuration
```
if ($http_origin ~ haiziwang\.com(:\d+)?$) {
  add_header 'Access-Control-Allow-Origin' "$http_origin";
  add_header 'Access-Control-Allow-Credentials' "true";
  add_header 'Access-Control-Allow-Headers' 'DNT,X-Mx-ReqToken,Keep-Alive,User-Agent,X-Requested-With,If-Modified-Since,Cache-Control,Content-Type,Authorization,token';
}
add_header 'Access-Control-Allow-Origin' "*";

```
