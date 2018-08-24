- `spider.py` to create a database. Fill in where html is Null, 

  |pages|  | | | | |
  |-----|-----|-----|-----|-----|-----|
  | id | url | html | error | old_rank | new_rank |
  | | | | | | |

  |links| a many to many table|
  |---|---|
  |from_id|to_id|
  | | | 
  
  >smart usage:
  - starturl = starturl[:-1] start to end-1
  - pos = starturl.rfind('/') find from the right side
