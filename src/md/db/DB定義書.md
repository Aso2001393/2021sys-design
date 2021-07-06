# DB定義書
## ER図
[ER図]( https://github.com/Aso2001393/2021sys-design/blob/main/test.md )

# DBテーブルカラム詳細一覧

# データベース詳細


### 購入テーブル（d_purchase）
|和名|属性名（カラム名）|型|PK|NN|FK|
|:---|:---|:---|:---|:---:|:----:|
|オーダーID|order_id|bigint(20)|〇|〇||
|顧客コード|customer_code|varchar(50)||〇||
|購入日|purchase_date|date||〇||
|総額|total_price|int(11)||〇||

### d_purchase_detail
|属性値|型|PK|NN|FK|
|:---|:---|:---|:---:|:----:|
|detail_id|bigint(20)|〇|〇||
|order_id|bigint(20)|〇|〇|〇|
|item_code|int(11)||〇||
|price|int(11)||〇||
|num|int(11)||〇||
