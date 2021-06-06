## Design a URL shorterning service like tinyurl
### Scope
1. 100 million URLs generate per day
2. Alpha numeric character allowed (a-zA-Z0-9)
3. Delete update not allowed
4. Highly avaiable, scalable and fault tolerance

### API end points
1. POST api/v1/url/tiny
> - request {long url : String}
> - response {tiny url : String}
2. GET api/v1/tinyurl
> response 301 redirect to original url

### Estimation
1. Write 100 million / 24 hr = 1157 per second
2. Read 10:1 1157 * 10 = 11570 per second
3. Number of records 100 million * 365 = 36.5 billion records per year
4. Data size 36.5 billion * 150 bytes = 5475 billion bytes = 5475 GB


### Fetch original URL
![Image fetch original URL](https://github.com/impradeeparya/system-design/blob/main/url-shortener/get-tiny-url.png)

### Create tiny URL
![Image create tiny URL](https://github.com/impradeeparya/system-design/blob/main/url-shortener/post-tiny-url.png)

