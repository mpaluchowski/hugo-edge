# Triathlete Hugo Theme

Triathlete is a Hugo theme for personal triathlete websites. Originally built for my own site at https://triathlete.paluchowski.com

## Installation

Clone the repository to your `/themes` directory, ie.

```shell
$ cd /your/hugo/site
$ git clone https://github.com/mpaluchowski/hugo-triathlete themes/triathlete
```

Build the [SASS](http://sass-lang.com/) files from `/assets/css` into `/static/css`:

```shell
$ cd themes/triathlete
$ sass -E UTF-8 --sourcemap=none --style compressed --update assets:static
```

Then tell Hugo to render your site with the theme:

```shell
$ hugo --theme=triathlete
```

## Customization

The theme is built primarily for my own use, so while it does offer some configuration and customization options, it will often impose a certain structure on you.

## Shortcodes

### `strava-activity`

Renders a single [Strava](https://www.strava.com) activity:

```go
{{< strava-activity id="840057488" hash="6a93a704064cb3cf22b266a1698cf9870fd1765a" >}}
```

Where `id` and `hash` are values you'll get when you open an activity, open the "Embed on Blog" dialog, which'll offer you an `IFRAME` code:

```html
<iframe height='405' width='590' frameborder='0' allowtransparency='true' scrolling='no' src='https://www.strava.com/activities/<id>/embed/<hash>'></iframe>
```
