# lepto-webp

```console
$ npm i -D lepto-webp
```

See [lepto documentation](https://github.com/dimitrinicolas/lepto) for usage.

This plugin has no options, just add it to your plugins list.

Default options:
```js
"use": [
  {
    "name": "lepto-webp",
    "quality": 80,
    "alphaQuality": 100,
    "lossless": false,
    "replaceFile": false
  }
]
```

## How to use .webp format

Since `.webp` files are not supported on all browser, you have to give them multiples ressources (like a `.jpg` and a `.webp`).

The simplest solution is to use the `<pictures>` tag:

```html
<picture>
  <source srcset="assets/output/image.webp" type="image/webp">
  <img src="assets/output/image.jpg" alt="">
</picture>
```

Browsers that supports webp format will only load the webp file, the others will only load the jpg one.

You can learn even more with the [images.guide](https://images.guide/) by Addy Osmani.

## License

This project is licensed under the [MIT license](LICENSE).
