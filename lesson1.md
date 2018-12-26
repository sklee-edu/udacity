# HTTP's Request/Recycle cycle

## HTTP Request
HTTP : HTML을 전송하기 위한 프로토콜
Request와 Response로 이루어져 있음

Request = First Line + Header
First line = method + request + version
Header section = host + (options)

## HTTP Response
Response = First Line + Header
First Line = version + status code + word
Header Section = content-length + (options)

## Getting multiple requests
index.html을 받아온 뒤에 additional resources(css, js, images)들을 받아옴

## DevTools
Browser에 있는 DevTools의 network 탭을

## Get
get data

## Post
Request에 payload를 담을 수 있음 
Post request에 redirect를 주는 이유

## Ajax (XHR -> Fetch)
XHR = XMLHttpRequest : outdated, callback을 사용
Fetch : promise를 사용해서 XHR을 사용할 필요 없음, Promises 사용
전체 웹페이지를 새로고침 할 필요 없이 데이터를 불러옴 