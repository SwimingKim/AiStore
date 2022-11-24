# Project: aiot (AiStore)

## End-point: register_store
### Method: POST
>```
>{{BASE_URL}}/register
>```
### Body formdata

|Param|value|Type|
|---|---|---|
|s_id|s4|text|
|name|cu|text|
|locate|seoul|text|


### Response: 200
```json
{"result": true}
```


⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃

## End-point: show_store
### Method: GET
>```
>{{BASE_URL}}/store/:id
>```
### Response: 200
```json
{"data": [{"s_id": "s1", "name": "\uc6a9\uc0b0\uc810", "locate": "\uc6a9\uc0b0", "products_num": 6}], "result": true}
```


⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃

## End-point: show_stores
### Method: GET
>```
>{{BASE_URL}}/stores
>```
### Response: 200
```json
{"data": [{"s_id": "s1", "name": "\uc6a9\uc0b0\uc810", "locate": "\uc6a9\uc0b0", "products_num": 6}, {"s_id": "s2", "name": "\uac15\ub0a8\uc810", "locate": "\uac15\ub0a8", "products_num": 3}, {"s_id": "s3", "name": "\uac15\ubd81\uc810", "locate": "\uac15\ubd81", "products_num": 4}], "result": true}
```


⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃

## End-point: manage_store
### Method: POST
>```
>{{BASE_URL}}/manage/:id
>```
### Body formdata

|Param|value|Type|
|---|---|---|
|p_id|p8|text|
|price|1500|text|
|count|5|text|


### Response: 200
```json
{"result": true}
```


⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃

## End-point: get_menu
### Method: GET
>```
>{{BASE_URL}}/menu
>```
### Body formdata

|Param|value|Type|
|---|---|---|
|s_id|s1|text|


### Response: 200
```json
{"data": [{"p_name": "\ucee4\ud53c", "price": 2000, "count": 46, "p_id": "p1"}, {"p_name": "\ucfe0\ud0a4", "price": 1000, "count": 30, "p_id": "p2"}, {"p_name": "\uc544\uc774\uc2a4\ud06c\ub9bc", "price": 1500, "count": 30, "p_id": "p3"}, {"p_name": "\uc5d0\uc774\ub4dc", "price": 3000, "count": 20, "p_id": "p4"}, {"p_name": "\uc640\ud50c", "price": 4000, "count": 10, "p_id": "p5"}, {"p_name": "\uacfc\uc77c\uc8fc\uc2a4", "price": 3000, "count": 10, "p_id": "p6"}], "result": true}
```


⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃

## End-point: get_products_list
### Method: GET
>```
>{{BASE_URL}}/products
>```
### Response: 200
```json
{"data": [{"p_id": "p1", "product": "\ucee4\ud53c", "reco_price": 1500}, {"p_id": "p2", "product": "\ucfe0\ud0a4", "reco_price": 2000}, {"p_id": "p3", "product": "\uc544\uc774\uc2a4\ud06c\ub9bc", "reco_price": 1500}, {"p_id": "p4", "product": "\uc5d0\uc774\ub4dc", "reco_price": 3000}, {"p_id": "p5", "product": "\uc640\ud50c", "reco_price": 4000}, {"p_id": "p6", "product": "\uacfc\uc77c\uc8fc\uc2a4", "reco_price": 4000}, {"p_id": "p7", "product": "\ucd08\ucf5c\ub9bf", "reco_price": 1500}], "result": true}
```


⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃

## End-point: buy_product
### Method: POST
>```
>{{BASE_URL}}/buy
>```
### Body formdata

|Param|value|Type|
|---|---|---|
|s_id|s1|text|
|p_id|p1|text|
|count|2|text|


### Response: 200
```json
{"result": true}
```


⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃
_________________________________________________
Powered By: [postman-to-markdown](https://github.com/bautistaj/postman-to-markdown/)
