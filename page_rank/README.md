- [`spider.py`](https://github.com/ZimingY/hello-world/blob/master/page_rank/spider.py)

  create a database. put inside the links in a web. have a web to initialize, initial rank is 1,  __database__, open __url__, __html__, __html.parser__,       __BeautifulSoup__, __anchor tags__, find url in a webpage.

  |pages|  | | | | |
  |-----|-----|-----|-----|-----|-----|
  | id | url | html | error | old_rank | new_rank |
  | | | | | | |

  |links| a many to many table|
  |---|---|
  |from_id|to_id|
  | | | 
  
  |webs|
  |----|
  |url|
  
  >smart usage:
  - `starturl = starturl[:-1]` start to end-1
  - `pos = starturl.rfind('/')` find from the right side
  - select from a sql, get a tuple, if only one, need a ',' behind.
  -  `tags = soup('a')`, Retrieve all of the anchor tags
   
   
- [`sprank.py`](https://github.com/ZimingY/hello-world/blob/master/page_rank/sprank.py)
  Save a previos rank using current rank. 

  >smart usage:
  - `conn = sqlite3.connect('spider.sqlite'). cur = conn.cursor()` read a database
  - `for (node, old_rank) in list(prev_ranks.items()):`, fetch a pair in the __dictionary__
