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
{
    "result": true
}
```


⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃

## End-point: show_store
### Method: GET
>```
>{{BASE_URL}}/store/:id
>```
### Response: 200
```json
{
    "result": true,
    "data": [
        {
            "s_id": "s1",
            "name": "용산점",
            "locate": "용산",
            "products_num": 6
        }
    ]
}
```


⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃

## End-point: show_stores
### Method: GET
>```
>{{BASE_URL}}/stores
>```
### Response: 200
```json
{"result": true, "data": [{"s_id": "s1", "name": "\uc6a9\uc0b0\uc810", "locate": "\uc6a9\uc0b0", "products_num": 6}, {"s_id": "s2", "name": "\uac15\ub0a8\uc810", "locate": "\uac15\ub0a8", "products_num": 3}, {"s_id": "s3", "name": "\uac15\ubd81\uc810", "locate": "\uac15\ubd81", "products_num": 4}, {"s_id": "s4", "name": "cu", "locate": "seoul", "products_num": 0}]}
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
{
    "result": true
}
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
{
    "result": true,
    "data": [
        {
            "p_name": "커피",
            "price": 2000,
            "count": 50,
            "p_id": "p1"
        },
        {
            "p_name": "쿠키",
            "price": 1000,
            "count": 30,
            "p_id": "p2"
        },
        {
            "p_name": "아이스크림",
            "price": 1500,
            "count": 30,
            "p_id": "p3"
        },
        {
            "p_name": "에이드",
            "price": 3000,
            "count": 20,
            "p_id": "p4"
        },
        {
            "p_name": "와플",
            "price": 4000,
            "count": 10,
            "p_id": "p5"
        },
        {
            "p_name": "과일주스",
            "price": 3000,
            "count": 10,
            "p_id": "p6"
        }
    ]
}
```


⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃

## End-point: get_products_list
### Method: GET
>```
>{{BASE_URL}}/products
>```
### Response: 200
```json
{
    "result": true,
    "data": [
        {
            "p_id": "p1",
            "product": "커피",
            "reco_price": 1500
        },
        {
            "p_id": "p2",
            "product": "쿠키",
            "reco_price": 2000
        },
        {
            "p_id": "p3",
            "product": "아이스크림",
            "reco_price": 1500
        },
        {
            "p_id": "p4",
            "product": "에이드",
            "reco_price": 3000
        },
        {
            "p_id": "p5",
            "product": "와플",
            "reco_price": 4000
        },
        {
            "p_id": "p6",
            "product": "과일주스",
            "reco_price": 4000
        },
        {
            "p_id": "p7",
            "product": "초콜릿",
            "reco_price": 1500
        }
    ]
}
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
{
    "result": true
}
```


⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃
_________________________________________________
Powered By: [postman-to-markdown](https://github.com/bautistaj/postman-to-markdown/)
