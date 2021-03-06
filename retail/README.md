# Usage 

```
usage: retail_data_gen.py [-h] [--no-file NO_FILE] [--no-line NO_LINE]
                          [--no-date NO_DATE] [--no-product NO_PRODUCT]
                          [--no-product-category NO_PRODUCT_CATEGORY]
                          [--no-store NO_STORE] [--no-city NO_CITY]
                          [--no-sales_quantity NO_SALES_QUANTITY]
                          [--no-unit_price NO_UNIT_PRICE]
                          [--always-same-result]

retail data generator

optional arguments:
  -h, --help            show this help message and exit
  --no-file NO_FILE     number of files. default is 1.
  --no-line NO_LINE     number of lines. default is 10000.
  --no-date NO_DATE     number of dates start from 2015-01-01 in YYYY-MM-DD
                        format. default is 365.
  --no-product NO_PRODUCT
                        no-product: number of products. default is 100.
  --no-product-category NO_PRODUCT_CATEGORY
                        number of product categories. default is 3.
  --no-store NO_STORE   number of stores. default is 10.
  --no-city NO_CITY     number of cities of stores. default is 3.
  --no-sales_quantity NO_SALES_QUANTITY
                        number of sales quantities. default is 107.
  --no-unit_price NO_UNIT_PRICE
                        number of unit prices. default is (no_product) * 2.
  --always-same-result  if you need always same result, please set this
                        option. random data is generated by default.
  ```

# Schema
  
## sales

- date_id
- product_id
- store_id
- sales_quantity
- unit_price
- sales_amount
  
## date_dim

- id
- date
  
## product_dim

- id
- name
- category
  
## store_dim

- id
- name
- city
  
