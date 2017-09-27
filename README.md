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
