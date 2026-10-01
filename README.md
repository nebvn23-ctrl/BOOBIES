# BOO-BIES · The Haunted Hallway

A one-page 3D site for **$BOO-BIES**, the ghost who put on a sheet to scare people and accidentally made them stare.

Everything (images, videos, font, code) is packed into `index.html`. Only three.js and Google Fonts load from a CDN.

## Set the contract and links

Open `config.js` (it is a small file, so you can edit it right on GitHub with the pencil icon):

```js
window.BOO_CONFIG = {
  ca:  "",                // contract address
  x:   "https://x.com/",  // X (Twitter) link
  buy: ""                 // optional buy link (DEX); leave empty to hide the button
};
```

While `ca` is empty, the site shows "Drops soon. The sheet is still on." instead of a copy button.

## Publish with GitHub Pages

1. Create a new **public** repository.
2. Upload every file from this folder to the root of the repository.
3. Go to **Settings → Pages**. Set **Source** to *Deploy from a branch*, branch `main`, folder `/ (root)`, then click **Save**.
4. After a minute or two, the site is live at `https://YOUR-USERNAME.github.io/REPO-NAME/`.

## Link preview on X

X needs a full URL for the preview image. In `index.html`, replace `preview.jpg` in the `og:image` and `twitter:image` tags with the full address, for example:

```
https://YOUR-USERNAME.github.io/REPO-NAME/preview.jpg
```

## Custom domain (optional)

1. In **Settings → Pages → Custom domain**, enter your domain.
2. At your domain provider, add a `CNAME` record pointing to `YOUR-USERNAME.github.io`.

## Files

| File | Purpose |
|---|---|
| `index.html` | The whole site |
| `config.js` | Contract address, X link, buy link |
| `preview.jpg` | 1200×630 image for link previews |
| `favicon.ico`, `apple-touch-icon.png` | Tab and home-screen icons |
