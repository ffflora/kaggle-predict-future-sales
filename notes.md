## Observations based on the Profiling Reports 

#### `train`

6 numeric, 1 categorical,

`date_block_num` has 3.9% zeros; has a lot common values, need to <u>remove duplicates</u> 

`item_cnt_day` is highly skewed : 272, might need to <u>take log</u>; has a lot common value

`item_id` common value; extreme value;

`item_price`  it has <u>negative value</u>, doesn't make sense; lots common value;

`shop_id` has a lot common value;

**correlation**

`date_block_num`  - `item_price` 

#### `test`

2 numeric, no warnings no zeros no missing

`item_id` why every value has exactly 42 count?

`shop_id` 42 variables. this might answer the last question.

#### `item_catg` 

2 numeric 

`item_categories` has only 1 zero

#### `items`

2 numeric,1 text

`item_cat_id` has some duplicates.

#### `shops`

---

## Some notes:

Not much need to do data cleaning.

since the submission is to predict in terms of month, we need to turn the date in days into months.



## Submissions:

- v1, baseline
  - score: 1.02317,  rank: 1817 