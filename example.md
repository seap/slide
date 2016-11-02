#Same Origin Policy
https://en.wikipedia.org/wiki/Same-origin_policy



#CORS (Cross-Origin Resource Sharing)
https://www.w3.org/TR/cors/




#nginx配置
```
if ($http_origin ~ haiziwang\.com(:\d+)?$) {
  add_header 'Access-Control-Allow-Origin' "$http_origin";
  add_header 'Access-Control-Allow-Credentials' "true";
  add_header 'Access-Control-Allow-Headers' 'DNT,X-Mx-ReqToken,Keep-Alive,User-Agent,X-Requested-With,If-Modified-Since,Cache-Control,Content-Type,Authorization,token';
}
add_header 'Access-Control-Allow-Origin' "*";

```
