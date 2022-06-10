<h1 align="center">WBX3</h1>
<br>

## webRequestBlocking for Manifest V3
Extension Manifest V3 might have made webRequestBlocking a pain in the ass to migrate, but it isn't impossible to use.

## How to use this
1. Fork or clone the repo
2. Go to `/Extension/src/block.json`
3. In line 9, change `example.com` to the domain you want to block.
4. Finally, `npm run build` at `/Extension/`.
5. Done! You now have a blocking extension in .zip, .xpi, and .crx format.
6. Remember, if you're using this as production software, remember to sign the .CRX file (Go to `chrome://extensions`, enable Developer Mode, and use `Pack Extension`).

### How this is done:
Using MV3 declarativeNetRequest rules, we can block requests.

### Google's documentation:
- Manifest: https://developer.chrome.com/docs/extensions/reference/declarativeNetRequest/#manifest
- Rules: https://developer.chrome.com/docs/extensions/reference/declarativeNetRequest/#rules
- Example: https://developer.chrome.com/docs/extensions/reference/declarativeNetRequest/#example