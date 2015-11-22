prayforparis
===========

Real time mapping of tweets tagged with #prayforparis. Forked from [worldtweets](https://github.com/abailin/worldtweets).

# Running Locally
Copy `config/config-sample.js` to `config/config.js`. Add in your Twitter API keys (which can be generated [here](https://dev.twitter.com/apps/new)).

Then run:
``` bash
npm install
foreman start # (or node server.js)
```


# Running on Heroku

``` bash
heroku create
```

You will need to set the twitter config vars that are normally specified in config.js. To do so run:

``` bash
heroku config:set consumer_key=XXX consumer_secret=XXX access_token_key=XXX access_token_secret=XXX
```

Finally, deploy it:

``` bash
git push heroku master
heroku open
```

