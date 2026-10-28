# Website Stylekit

Website Stylekit is a free color palette and typography generator. This repository contains the final static website build (v2.7) and the WordPress plugin (v2.6).

The website is still available at [websitestylekit.com](https://websitestylekit.com/). New features are no longer being developed. You are welcome to download and self-host this build for your own use.

## Host the website

The ready-to-host files are in [`site/`](site/). There is no build step or Node.js dependency.

- **Netlify Drop:** Upload the `site` folder.
- **Other static host:** Publish the contents of `site` as the site root. The host needs to serve `index.html` for unknown page paths; Netlify uses the included `_redirects` file.
- **Local preview:** Run `cd site && python3 -m http.server 8000`, then open `http://localhost:8000`.

If you connect this repository to Netlify, [`netlify.toml`](netlify.toml) sets `site` as the publish directory.

This is the deployed, compiled website bundle, not the original editable Bolt project. The site build matches the live v2.7 app, apart from removing Website Stylekit's analytics scripts and correcting asset filename case for case-sensitive hosts.

## WordPress plugin

The installable [v2.6 ZIP](site/downloads/websitestylekit-2.6.zip) is the same package offered on the website. Its source files are in [`wordpress-plugin/websitestylekit/`](wordpress-plugin/websitestylekit/). In WordPress, go to **Plugins → Add New → Upload Plugin** and select the ZIP.

Version 2.6 imports Website Stylekit CSS variables and global classes into Elementor V4 or Bricks, with an import preview and backups. It is no longer actively developed, so compatibility with future builder versions is not guaranteed.

The [Figma plugin](https://www.figma.com/community/plugin/1540582911151196326/website-stylekit) remains available separately in Figma Community.
