
# aiot (AiStore)



<!--- If we have only one group/collection, then no need for the "ungrouped" heading -->
1. [buy_product](#1-buy_product)
   1. [success](#i-example-request-success)
1. [get_products_list](#2-get_products_list)
   1. [success](#i-example-request-success-1)
1. [get_menu](#3-get_menu)
   1. [success](#i-example-request-success-2)
1. [manage_store](#4-manage_store)
   1. [success](#i-example-request-success-3)
1. [show_stores](#5-show_stores)
   1. [success](#i-example-request-success-4)
1. [show_store](#6-show_store)
   1. [success](#i-example-request-success-5)
1. [register_store](#7-register_store)
   1. [success](#i-example-request-success-6)
   1. [fail](#ii-example-request-fail)


## Variables

| Key | Value | Type |
| --- | ------|-------------|
| BASE_URL | http://127.0.0.1:9999/api | string |



## Endpoints


--------



### 1. buy_product



***Endpoint:***

```bash
Method: POST
Type: FORMDATA
URL: {{BASE_URL}}/buy
```



***Body:***

| Key | Value | Description |
| --- | ------|-------------|
| s_id | s1 |  |
| p_id | p1 |  |
| count | 2 |  |



***More example Requests/Responses:***


#### I. Example Request: success



***Body:***

| Key | Value | Description |
| --- | ------|-------------|
| s_id | s1 |  |
| p_id | p1 |  |
| count | 2 |  |



#### I. Example Response: success
```js
{
    "result": true
}
```


***Status Code:*** 200

<br>



### 2. get_products_list



***Endpoint:***

```bash
Method: GET
Type: 
URL: {{BASE_URL}}/products
```



***More example Requests/Responses:***


#### I. Example Request: success



***Body: None***



#### I. Example Response: success
```js
{
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
    ],
    "result": true
}
```


***Status Code:*** 200

<br>



### 3. get_menu



***Endpoint:***

```bash
Method: GET
Type: FORMDATA
URL: {{BASE_URL}}/menu
```



***Body:***

| Key | Value | Description |
| --- | ------|-------------|
| s_id | s1 |  |



***More example Requests/Responses:***


#### I. Example Request: success



***Body:***

| Key | Value | Description |
| --- | ------|-------------|
| s_id | s1 |  |



#### I. Example Response: success
```js
{
    "data": [
        {
            "p_name": "커피",
            "price": 2000,
            "count": 46,
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
    ],
    "result": true
}
```


***Status Code:*** 200

<br>



### 4. manage_store



***Endpoint:***

```bash
Method: POST
Type: FORMDATA
URL: {{BASE_URL}}/manage/:id
```



***URL variables:***

| Key | Value | Description |
| --- | ------|-------------|
| id | s1 |  |



***Body:***

| Key | Value | Description |
| --- | ------|-------------|
| p_id | p8 |  |
| price | 1500 |  |
| count | 5 |  |



***More example Requests/Responses:***


#### I. Example Request: success



***Query:***

| Key | Value | Description |
| --- | ------|-------------|
| id | s1 |  |



***Body:***

| Key | Value | Description |
| --- | ------|-------------|
| p_id | p1 |  |
| price | 1800 |  |
| count | 5 |  |



#### I. Example Response: success
```js
{
    "result": true
}
```


***Status Code:*** 200

<br>



### 5. show_stores



***Endpoint:***

```bash
Method: GET
Type: 
URL: {{BASE_URL}}/stores
```



***More example Requests/Responses:***


#### I. Example Request: success



***Body: None***



#### I. Example Response: success
```js
{
    "data": [
        {
            "s_id": "s1",
            "name": "용산점",
            "locate": "용산",
            "products_num": 6
        },
        {
            "s_id": "s2",
            "name": "강남점",
            "locate": "강남",
            "products_num": 3
        },
        {
            "s_id": "s3",
            "name": "강북점",
            "locate": "강북",
            "products_num": 4
        }
    ],
    "result": true
}
```


***Status Code:*** 200

<br>



### 6. show_store



***Endpoint:***

```bash
Method: GET
Type: 
URL: {{BASE_URL}}/store/:id
```



***URL variables:***

| Key | Value | Description |
| --- | ------|-------------|
| id | s1 |  |



***More example Requests/Responses:***


#### I. Example Request: success



***Query:***

| Key | Value | Description |
| --- | ------|-------------|
| id | s1 |  |



***Body: None***



#### I. Example Response: success
```js
{
    "data": [
        {
            "s_id": "s1",
            "name": "용산점",
            "locate": "용산",
            "products_num": 6
        }
    ],
    "result": true
}
```


***Status Code:*** 200

<br>



### 7. register_store



***Endpoint:***

```bash
Method: POST
Type: FORMDATA
URL: {{BASE_URL}}/register
```



***Body:***

| Key | Value | Description |
| --- | ------|-------------|
| s_id | s4 |  |
| name | cu |  |
| locate | seoul |  |



***More example Requests/Responses:***


#### I. Example Request: success



***Body:***

| Key | Value | Description |
| --- | ------|-------------|
| s_id | s4 |  |
| name | cu |  |
| locate | seoul |  |



#### I. Example Response: success
```js
{
    "result": true
}
```


***Status Code:*** 200

<br>



#### II. Example Request: fail



***Body:***

| Key | Value | Description |
| --- | ------|-------------|
| s_id | s4 |  |
| name | cu |  |
| locate | seoul |  |



#### II. Example Response: fail
```js
{
    "data": "already exist",
    "result": false
}
```


***Status Code:*** 400

<br>



---
[Back to top](#aiot-aistore)

>Generated at 2022-11-24 17:03:44 by [docgen](https://github.com/thedevsaddam/docgen)
