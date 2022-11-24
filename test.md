
# aiot (AiStore)



<!--- If we have only one group/collection, then no need for the "ungrouped" heading -->
1. [buy_product](#1-buy_product)
   1. [buy_product](#i-example-request-buy_product)
1. [get_products_list](#2-get_products_list)
   1. [get_products_list](#i-example-request-get_products_list)
1. [get_menu](#3-get_menu)
   1. [get_menu](#i-example-request-get_menu)
1. [manage_store](#4-manage_store)
   1. [manage_store](#i-example-request-manage_store)
1. [show_stores](#5-show_stores)
   1. [show_stores](#i-example-request-show_stores)
1. [show_store](#6-show_store)
   1. [show_store](#i-example-request-show_store)
1. [register_store](#7-register_store)
   1. [register_store](#i-example-request-register_store)
   1. [register_store](#ii-example-request-register_store)


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


#### I. Example Request: buy_product



***Body:***

| Key | Value | Description |
| --- | ------|-------------|
| s_id | s1 |  |
| p_id | p1 |  |
| count | 2 |  |



#### I. Example Response: buy_product
```js
{"result": true}
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


#### I. Example Request: get_products_list



***Body: None***



#### I. Example Response: get_products_list
```js
{"data": [{"p_id": "p1", "product": "\ucee4\ud53c", "reco_price": 1500}, {"p_id": "p2", "product": "\ucfe0\ud0a4", "reco_price": 2000}, {"p_id": "p3", "product": "\uc544\uc774\uc2a4\ud06c\ub9bc", "reco_price": 1500}, {"p_id": "p4", "product": "\uc5d0\uc774\ub4dc", "reco_price": 3000}, {"p_id": "p5", "product": "\uc640\ud50c", "reco_price": 4000}, {"p_id": "p6", "product": "\uacfc\uc77c\uc8fc\uc2a4", "reco_price": 4000}, {"p_id": "p7", "product": "\ucd08\ucf5c\ub9bf", "reco_price": 1500}], "result": true}
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


#### I. Example Request: get_menu



***Body:***

| Key | Value | Description |
| --- | ------|-------------|
| s_id | s1 |  |



#### I. Example Response: get_menu
```js
{"data": [{"p_name": "\ucee4\ud53c", "price": 2000, "count": 46, "p_id": "p1"}, {"p_name": "\ucfe0\ud0a4", "price": 1000, "count": 30, "p_id": "p2"}, {"p_name": "\uc544\uc774\uc2a4\ud06c\ub9bc", "price": 1500, "count": 30, "p_id": "p3"}, {"p_name": "\uc5d0\uc774\ub4dc", "price": 3000, "count": 20, "p_id": "p4"}, {"p_name": "\uc640\ud50c", "price": 4000, "count": 10, "p_id": "p5"}, {"p_name": "\uacfc\uc77c\uc8fc\uc2a4", "price": 3000, "count": 10, "p_id": "p6"}], "result": true}
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


#### I. Example Request: manage_store



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



#### I. Example Response: manage_store
```js
{"result": true}
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


#### I. Example Request: show_stores



***Body: None***



#### I. Example Response: show_stores
```js
{"data": [{"s_id": "s1", "name": "\uc6a9\uc0b0\uc810", "locate": "\uc6a9\uc0b0", "products_num": 6}, {"s_id": "s2", "name": "\uac15\ub0a8\uc810", "locate": "\uac15\ub0a8", "products_num": 3}, {"s_id": "s3", "name": "\uac15\ubd81\uc810", "locate": "\uac15\ubd81", "products_num": 4}], "result": true}
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


#### I. Example Request: show_store



***Query:***

| Key | Value | Description |
| --- | ------|-------------|
| id | s1 |  |



***Body: None***



#### I. Example Response: show_store
```js
{"data": [{"s_id": "s1", "name": "\uc6a9\uc0b0\uc810", "locate": "\uc6a9\uc0b0", "products_num": 6}], "result": true}
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


#### I. Example Request: register_store



***Body:***

| Key | Value | Description |
| --- | ------|-------------|
| s_id | s4 |  |
| name | cu |  |
| locate | seoul |  |



#### I. Example Response: register_store
```js
{"result": true}
```


***Status Code:*** 200

<br>



#### II. Example Request: register_store



***Body:***

| Key | Value | Description |
| --- | ------|-------------|
| s_id | s4 |  |
| name | cu |  |
| locate | seoul |  |



#### II. Example Response: register_store
```js
{"data": "already exist", "result": false}
```


***Status Code:*** 400

<br>



---
[Back to top](#aiot-aistore)

>Generated at 2022-11-24 16:26:24 by [docgen](https://github.com/thedevsaddam/docgen)
