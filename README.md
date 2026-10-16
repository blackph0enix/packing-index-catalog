# Packing Index catalog feed

The live gear catalog that the Packing Index app downloads in the background, so a new
product reaches a phone without a new app build.

`catalog.json` is generated and published automatically from the
[Packing Index](https://github.com/blackph0enix/packing-index) repository whenever its
bundled catalog changes. Do not edit it by hand: the next publish overwrites it.

Contents are facts only: brand, product name, category, weight in grams and an estimated
street price in US dollars. There are no images, and nothing bladed (the importer and the
app both filter that).

Format: `{ "schema": 1, "generatedAt": "<ISO 8601>", "count": N, "items": [ ... ] }`
