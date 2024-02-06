# CreditCard

```
Comment on page

# Credit Card

How to use CreditCard to submit a payin in Brazil.

post

https://gateway-test.pagsmile.com

/trade/pay

Payin by CreditCard

##

Example

curl --location --request POST 'https://gateway-test.pagsmile.com/trade/pay' \

\--header 'Authorization: Basic
MTYyNTgyOTIxNDUzMTY2Mzg6UGFnc21pbGVfc2tfZDUwMWQ1ZGNkNTI5OGQ5N2MwNmUzYjI4YjA2OWZjZmY3NDU5ZjY2NzNiMjFjMTFlYTY3NDM5MDgzOTZkOTYxNQ=='
\

\--header 'Content-Type: application/json' \

\--data-raw '{

* "app_id": "162************38",

* "out_trade_no": "202201010354003",

* "method": "CreditCard",

* "order_amount": "12.01",

* "order_currency": "BRL",

* "subject": "trade pay test",

* "content": "trade pay test conent",

* "notify_url": "http://merchant/callback/success",

"return_url": "https://www.merchant.com",

* "buyer_id": "buyer_0101_0001",

* "user_ip":"127.0.0.1",

* "token":"${token}",

* "fingerprint":"${fingerprint}",

* "issuer":"visa",

"installments":"1",

* "timestamp": "2022-01-01 03:54:01",

"timeout_express":"1c",

* "customer" : {

* "identify": {

* "type": "CPF",

* "number": "11032341882"

},

* "name": "Test User Name",

* "email": "[[email protected]](/cdn-cgi/l/email-protection)",

* "phone": "75991435892"

},

* "address" : {

* "zip_code": "38082365"

},

* "threeds": {

* "sli": "",

* "version": "",

* "cavv": "",

* "eci": "",

* "server_trans_id": "",

* "xid": "",

"cvv": "",

"avs": "",

"status": "",

* "status_code": "",

"status_reason_code": "",

"liability_shift": true

}

}'

Note: **162************38** is pagsmile's test app id for sandbox, and
**MTYyNTgyOTIxNDUzMTY2Mzg6UGFnc21pbGVfc2tfZDUwMWQ1ZGNkNTI5OGQ5N2MwNmUzYjI4YjA2OWZjZmY3NDU5ZjY2NzNiMjFjMTFlYTY3NDM5MDgzOTZkOTYxNQ==**
is authorization token associated with the test app id.

Please use your own **app_id** and generate your own **authorization token**
when testing.

[PreviousBrazil](/payin/submit-a-payin/brazil)[NextPix](/payin/submit-a-
payin/brazil/pix)

Last modified 2mo ago

```
