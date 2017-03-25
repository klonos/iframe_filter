# Summary

iframe filter embeds content in an iframe, which is useful for embedded external
content or widgets and speeding up ad provider load times.

When used, this will place the entirety of the content into a standalone HTML
page that is included within an `iframe`.

* Project page:
  * http://drupal.org/project/iframe_filter
* Bug reports, feature suggestions and latest developments:
  * http://drupal.org/project/issues/iframe_filter

## Requirements

None.

## Usage

  1. Go to input format page and create or edit an input format.
  2. In the list of filters choose "iframe filter".
  3. Make sure that this filter is the latest one to be executed, for doing
     this click "configure" on the input format and then go to "rearrange".
  4. Move the iframe filter to the latest position and click save.
  5. Create the block or content that you want to be displayed as an iframe
     choosing the input format you defined previously.
  6- Enter the height and width of the iframe in an HTML comment in this way:
    `<!-- =wxh -->` or `<!-- width="w" height="w" -->` replace "h" y "w" with the
	correct width and height.
  7- Save the content.

Example:

```html
<!-- width="728" height="90" --><script src="http://../something.js"></script>
```

## Troubleshooting

* If there isn't a valid width or height, the content won't be placed inside an iframe.

## Credits

* The Drupal version of this project is maintained by Javier Reartes (javierreartes)
* Originally created by Nathan Haug (quicksketch)
* Ported to Backdrop by Jon Peck (fluxsauce).
