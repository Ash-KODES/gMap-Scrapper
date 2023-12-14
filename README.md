# Google maps scraper
For scrapping mail and phone number
## Extracted Data Points

```
link
title
category
address
open_hours
popular_times
website
phone
plus_code
review_count
review_rating
reviews_per_rating
latitude
longitude
cid
status
descriptions
reviews_link
thumbnail
timezone
price_range
data_id
images
reservations
order_online
menu
owner
complete_address
about
user_reviews
emails
```

### On your host

(tested only on Ubuntu 22.04)


```
cd google-maps-scraper
go mod download
go build
./google-maps-scraper -input example-queries.txt -results restaurants-in-cyprus.csv -exit-on-inactivity 3m
```

Be a little bit patient. In the first run it downloads required libraries.

The results are written when they arrive in the `results` file you specified

**If you want emails use additionally the `-email` parameter**
