
quaint-google-analytics
=======================

Generate Google Analytics' boilerplate for your Quaint site.

Once the plugin is loaded, you can use the `analytics ::` macro
anywhere in order to load the tracking code.

## Install

    quaint --setup google-analytics

Follow the instructions.


## Sample configuration

This configuration entry must be added in the `plugins` section of
`quaint.json`:

```json
"google-analytics": {
  "trackingId": "UA-12345678-9",
  "auto": true
}
```

If the `auto` option is true (it is false by default), then it is
unnecessary to call `analytics ::`.


## Options

### trackingId

**REQUIRED**. The tracking ID that google analytics gives you for your
domain. It should start with "UA" and then a numeric code.


### auto

(boolean) (default: false)

If `auto` is true, the tracking code will be added to each page
automatically. If `auto` is false, then you need to call the
`analytics ::` macro explicitly.

