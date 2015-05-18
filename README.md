This PHP library implements a subscriber for PubSubHubbub.

It was written by Josh Fraser (joshfraser.com) and is released under the Apache 2.0 License

# Usage

```php
include("subscriber.php");

$hub_url = "http://pubsubhubbub.appspot.com";
$callback_url = "put your own endpoint here";

$feed = "http://feeds.feedburner.com/onlineaspect";

// create a new subscriber
$s = new Subscriber($hub_url, $callback_url);

// subscribe to a feed
$s->subscribe($feed);

// unsubscribe from a feed
$s->unsubscribe($feed);
```
