# kembe-theme-shopify

Kembe Theme for Spotify

## Dependencies

- Docker
- bash/zsh

## cli

Theme development is made so much easier with the help of the Shopify Theme cli. I have repackaged Shopify's own Ruby Gem ([`shopify_theme`](https://github.com/Shopify/shopify_theme)) as a [Docker image]() so as to encapsulate the ruby environment and not pollute the host machine. The source for this can be found in [my fork](https://github.com/collingo/shopify_theme).

To set this up...

1. Check this repo out onto your own machine and `cd` in
1. Install cli - `docker run --rm -v $(pwd):/usr/src collingo/shopify_theme`
1. All the `shopify_theme` [commands](https://github.com/collingo/shopify_theme#commands) should work now. Just preped with `make`, e.g. `$ theme download` => `$ make theme download`
1. Setup Shopify config - `make theme configure` passing options as described [here](https://github.com/collingo/shopify_theme#setting-up-shopify-theme)
1. Code!

## Commands

See the [`shopify_theme`](https://github.com/Shopify/shopify_theme) docs for more info. Remember to always prepend commands with `make` when using the cli as described above
