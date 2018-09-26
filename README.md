
<p align="center">
	<a href="https://projects.abranhe.com/popular-repos"><img src="https://cdn.abranhe.com/projects/popular-repos/logo.png" width="30%"></a>
	<br>
	<br>
	<br>
	<a href="https://projects.abranhe.com/popular-repos"><b>popular-repos</b></a>: Get the most popular public repositories from a user.
</p>

<p align="center">
	<a href="https://travis-ci.org/abranhe/popular-repos"><img src="https://img.shields.io/travis/abranhe/popular-repos.svg?logo=travis" /></a>
	<a href="https://github.com/abranhe/popular-repos/blob/master/LICENSE"><img src="https://img.shields.io/github/license/abranhe/popular-repos.svg" /></a>
	<a href="https://github.com/abranhe"><img src="https://abranhe.com/badge.svg"></a>
	<a href="https://cash.me/$abranhe"><img src="https://cdn.abraham.gq/badges/cash-me.svg"></a>
	<a href="https://www.patreon.com/abranhe"><img src="https://cdn.abraham.gq/badges/patreon.svg" /></a>
	<a href="https://paypal.me/abranhe/10"><img src="https://cdn.abraham.gq/badges/paypal.svg" /></a>
</p>

# Overview

It returns the most popular repositories (sorted by startgazers) of a user along with some metadata. The result is cached for a day.

# Usage

[![Deploy to now](https://deploy.now.sh/static/button.svg)](https://deploy.now.sh/?repo=https://github.com/abranhe/popular-repos&env=GITHUB_TOKEN&env=GITHUB_USERNAME&env=ACCESS_ALLOW_ORIGIN&env=MAX_REPOS&env=CACHE_MAX_AGE)

or

```
$ now abranhe/popular-repos -e NODE_ENV=production -e GITHUB_TOKEN=xxx -e GITHUB_USERNAME=xxx -e ACCESS_ALLOW_ORIGIN=xxx -e MAX_REPOS=xxx -e CACHE_MAX_AGE=xxx
```

Deploy to your hosting provider, set the below environment variables, and start it with `npm start`.


## Environment variables

Define the following environment variables:

- `GITHUB_TOKEN` - [Personal access token.](https://github.com/settings/tokens/new?description=popular-repos)
- `GITHUB_USERNAME` - The username you like to get repos from.
- `ACCESS_ALLOW_ORIGIN` - The URL of your website or `*` if you want to allow any origin (not recommended), for the `Access-Control-Allow-Origin` header.
- `MAX_REPOS` - The number of repos returned. Optional. Defaults to 6.
- `CACHE_MAX_AGE` - The maximum age for client cache-control in seconds. Optional. Defaults to 300 (5 minutes).


# Related

> it wouldn't be possible without [gh-latest-repos](https://github.com/sindresorhus/gh-latest-repos)👏

- [gh-latest-repos](https://github.com/sindresorhus/gh-latest-repos): Microservice to get the latest public GitHub repos from a user.

# Team

|[![Carlos Abraham Logo](https://avatars3.githubusercontent.com/u/21347264?s=50&v=4)](https://19cah.com)|
| :-: |
| [Carlos Abraham](https://github.com/abranhe) |


# License

[MIT](https://github.com/abranhe/popular-repos/blob/master/LICENSE) License © [Carlos Abraham](https://github.com/abranhe)
