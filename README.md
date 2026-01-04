# Bike Bus Network

This repository contains the source for website at http://www.bikebus.net.au


## Development

### Prerequisites

Same as `jekyll`. See https://jekyllrb.com/docs/

### Build

Clone or copy this repository, then from the root directory execute:

```
bundle install
```

### Test

From the root directory, execute:

```
bundle exec jekyll serve
```

and then browse to http://localhost:4000

## Deploy

Build the site with:

```
JEKYLL_ENV=production bundle exec jekyll build
```

and then copy the `_site` folder to the web server with something like:

```
rsync -avz --delete _site/ www-data@my.web.server:/var/www/bike_bus_network
```

Note the trailing slash on `_site/` to copy the contents, rather than the folder itself.

This assumes there is a web server engine (eg. nginx or apache) set up to serve from `/var/www/bike_bus_network`. Being a static site, there is little else to do.

The build and copy steps are what happens in CI, using Github Actions, on every commit to the `main` branch.
