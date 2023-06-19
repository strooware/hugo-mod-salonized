# Salonized for Hugo

This mod for hugo makes it really easy to add [salonized](https://salonized.com) to your theme or website.

## Usage

There are shortcodes for the following widgets:
- [layouts/shortcodes/salonized/bookings](https://github.com/strooware/hugo-mod-salonized/blob/master/layouts/shortcodes/salonized/bookings.html) ([partial](https://github.com/strooware/hugo-mod-salonized/blob/master/layouts/partials/salonized/bookings.html))
- [layouts/shortcodes/salonized/reviews](https://github.com/strooware/hugo-mod-salonized/blob/master/layouts/shortcodes/salonized/reviews.html) ([partial](https://github.com/strooware/hugo-mod-salonized/blob/master/layouts/partials/salonized/reviews.html))


## Installation

Run this to install mod
```bash
$ hugo mod get -u git.strooweb.nl/strooware/hugo-mod-salonized
```

Add this to your html
```html
<html>
   <head>
      <!-- ... -->
      {{- partial "header/scripts/salonized" . -}}
   </head>

   <body>
      <!-- ... -->
      {{- partial "footer/scripts/salonized" . -}}
   </body>
</html>
```

Add this to your config
```toml
[params.mods.salonized]
color = "#ff50b3"
company_id = "xxx"
company_url = "xxx"
```