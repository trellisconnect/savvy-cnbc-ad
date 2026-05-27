# Savvy × CNBC — Ad Embed Guide

Integration instructions for embedding the Savvy insurance ad unit on CNBC properties.

## Overview

The ad is a self-contained, responsive unit served from Savvy's CDN. It shows a short insurance value proposition with a ZIP-code entry; on click it opens the CNBC-branded Savvy quote experience in a new tab.

## Embed

Paste this wherever the ad should appear:

```html
<iframe
  src="https://cdn.savvy.insure/cnbc/v1.0/index.html"
  style="width:100%;max-width:700px;height:460px;border:0;display:block"
></iframe>
```

## Live preview

A rendered reference showing the embed is available at:

**https://cdn.savvy.insure/cnbc/v1.0/iframe-test.html**

## Tracking continuity (optional)

The ad accepts an optional `txn` query parameter, which it forwards to the destination on click. If you pass a transaction or session identifier, append it to the iframe `src`:

```html
<iframe
  src="https://cdn.savvy.insure/cnbc/v1.0/index.html?txn=YOUR_ID"
  ...
></iframe>
```

## Requirements

- A standard `<iframe>`. Nothing else.
- No scripts or external libraries on the host page.
- No cookies are set on the parent page.

## Support

For questions or changes, reach out to your Savvy contact.
