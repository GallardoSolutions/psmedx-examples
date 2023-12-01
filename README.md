# PSMEDx Examples

Examples of how to use PSMEDx API

This pages will be published at [PSMEDx Examples](https://s3.amazonaws.com/www.gallardo.solutions/psmedx-examples/index.html)

## Resources:
- [PSMEDx](https://psmedx.com)
- [PSMEDx docs](https://psmedx.com/docs)


# Easy of use

We are focussing here in how to use a `Public Key` that can be obtained from PSMEDx website once you have an account.
With this `Public Key` you will be able to use the API without the need of a `Secret Key` that is used for authentication.
Meaning you can access to `GET` requests that provide images based on query parameters.

In order for this public key to be secure, you need to add the allowed origin to your account. This is done in the `Account` section of the website.

## Example 1: Get an image without the background

This example shows how to get an image with the background.

Basic example is this one:

```html
<img src="https://api.psmedx.com//remove-background/?image_url=YOUR_IMAGE_URL&pub_api_key=YOUR_PUBLIC_KEY" />
```

But We provide a more complete example using [htmx](https://htmx.org/) and [Alpine.js](https://alpinejs.dev/)

