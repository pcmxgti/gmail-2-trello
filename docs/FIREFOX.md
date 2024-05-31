## Building for Firefox
As of Firefox 126, go in the *chrome_manifest_v2* directory, and execute the command below. Firefox does not currently
support all the manifest v3 features.

```sh
zip -r -FS ../g2t-ff-mv2-$(jq -r '.version' manifest.json).zip * --exclude '*.git*'
```

And submit to the [Mozilla Developer Hub](https://addons.mozilla.org/en-US/developers/) as a private XPI.

