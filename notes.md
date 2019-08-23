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

