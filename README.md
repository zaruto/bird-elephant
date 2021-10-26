# Elephant Bird

### Connect to Twitter API v2 Early Access endpoints in PHP.

---

**Note**: This package now caters for both bearer token based app access as well as OAuth 1.0 user access**.

Use cases as I see them:
1. App read-only access - pull stats and data from the API - use bearer tokens
2. User Authenticated access - allow your apps users to authenticate and perform read/write actions ,will require you to use a workflow for storing/retrieving auth tokens
3. App read/write - ideal for bots/managed accounts where you need to write exclusively to one account

you can look at index.php and authenticate.php for examples.

These endpoints are early access so subject to change. This package does not support v1 endpoints.

To use the Twitter API v2, and consequently this package, you must have an approved developer account and have activated the new developer portal.

Learn more about getting access to the Twitter API v2 endpoints:

[Twitter Getting Started Docs](https://developer.twitter.com/en/docs/twitter-api/getting-started/guide)


Note that operator support is quite sparse at the moment which makes the use of tweets and media more than a little risky in some contexts - for example filtering NSFW content is not yet possible. I don't know if this is in Twitter's plans or not.

## Install:

Install via composer.

```bash
$ composer require coderjerk/elephant-bird
```

## Auth

Bearer token support only for now. Copy the contents of .env.example to .env in your project and populate with your own credentials that you have set up for your project in the Twitter dev portal. If you aren't using .env in your project, you will need to set it up, [details here](https://github.com/vlucas/phpdotenv)

## Reference &amp; Examples:

- [Users](/docs/Users.md)
- [Tweets](/docs/Tweets.md)
- [Compliance](/docs/Compliance.md)
- [Lists](/docs/Lists.md)
- [Spaces](/docs/Spaces.md)


## Contributing

Fork/download the code and run
`composer install`

This package is in the early stages of development. Issues, pull requests and other contributions most welcome.

You can [look at the project board here for upcoming features:](https://github.com/danieldevine/elephant-bird/projects/1)
