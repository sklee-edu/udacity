# HTTP/1

## Netcat
Netcat command is a utility that's used for sending and receiving messages over a network connection

## Verbs
GET : 데이터 요청
POST : 데이터 추가
HEAD : 데이터가 변경 되었는지 확인
OPTIONS : 어떤 Verbs 들이 허용되는지

## Response Headers
Content-Length : response body에 있는 bytes의 size를 알려줌
Content-Type : image/jpeg, text/html 등 다양한 타입을 알려줌
Last-Modified : 데이터가 수정된 마지막 날짜, 콘텐츠의 일부가 바뀐 뒤에도 수정이 되는 경우를 방지하기 위해 ETag(Entitiy Tah)를 사용하는 것도 방법
Cache-Control : browser에서 cache를 할지 말지를 정함
If-Modified-Since : 변한게 없으면 데이터 전송을 하지 않음

## REST
REpresentational State Transfer

ex. 
GET /persons/Richard
PUT /persons/Richard : update record
POST /persons/ : create new record
DELETE /persons/Surma : delete item in collection

## Performance
head-of-line-breaking : http는 queue처럼 작동해서 다른 connection들이 빨리 끝나는 일이여도 느리게 만드는 bottleneck이다
Connection : keep-alive를 통해 connection의 수를 줄여서 3 way handshaking을 줄이고, bundle.js 등을 만들어서 통신을 적게 하려함