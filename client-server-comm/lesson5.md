# Security

## Single Origin Policy
javascript는 다른 origin에 있는 것을 허락하지 않음
origin = data scheme(https://) + hostname(www.udacity.com) + port(:443)

## CORS 
JSONP와 같은 방식으로 server에서 해결하는 방식도 있었음
Single Origin Policy의  한계를 극복하기 위한 Cross origin resource
Request의 Referer가 Response의 Access-Control-Allow-Origin에 있으면 가능 
Preflight request로 OPTIONS를 보내서 동작 가능한지 먼저 확인하는 방법도 있음

## CSRF
Cross-site request forgery
Form에서 오는 것은 preflight가 되지 않음.
CSFR token을 통해서 matching이 되는 사람에게만 적당한 응답을 보여줌

## XSS
Cross-site scripting
사용자의 입력 값을 확인하지 않음