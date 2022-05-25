# Adform Tracking

This is an unofficial Adform tracking tag for the Google Tag Manager Community Template Gallery. Please raise an issue if you find any bugs or have a question!

## Documentation

### Adform Server Domain

You can change the default domain of the server (usually track.adform.net) to suit your own needs. Do **not** change this if you were not explicitly asked to!

### Adform Tracking ID (pm)

This is the Adform client ID, also referred to as *pm*.

### Tracking Point Name (pagename)

This is the name of the tracking point, also referred to as *pagename*. You can set this to a specific string, but it is recommended to either use URL path or custom *pagenames* when tracking across multiple pages.

`{{Page Path}}` can be used and will generate a tracking point for each page the tag is fired on. You might want to exclude pages which should not be tracked when using the `All Pages` trigger.

### Variables

You can track [custom variables](https://support.adform.com/documentation/implement-tracking-points/standard-javascript/variables/) such as sales, order ids, product names or other custom values in addition to the default values.

#### Variables Object

You can use a variable which returns an `Object` to track custom variables. Any other type than `Object` is discarded.

This is helpful when you need to include product data on certain pages, simply return the values you need on the product pages and `undefined` on the rest.

#### Variables Table

In addition to a variable, you can also use a table to track custom variables.

### Optional Parameters

#### Divider

Tells Adform which character to use to split up the pagename. The default value is the pipe character `|`.
