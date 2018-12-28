# HTTPS

## HTTPS
HTTPS = HTTP + TLS(SSL)
TLS = Transport Layer Security
Certifiacte를 제공해서 browser에 저장을 해놓음

## Encryption
TLS = Encryption + Hashing
One key for encryption(public key)
One key for decryption(private key)

## Hashing
Hashing의 특징
- Reverse가 힘듬
- Different value가 same value를 가지기 힘듬

## Signature
Document가 보장 되었다는 것을 확인
전체 데이터를 encrypt를 하면 시간이 오래 걸림.
그렇기 때문에 hash를 한 다음에 encrypt를 해서 시간을 단축 시킴.
Asymmetric한 것임.

## TLS hanshake
1. 