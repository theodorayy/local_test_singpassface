# CDN-free SingPass Face Example

## Instructions

1. Download this repo
2. On macOS, install npm first if it's not installed.
3. Then, run run.sh

## Source Code

### dist folder 

**/dist** contains the build files for a static Vue.js SPA using the Nuxt framework. It also contains the offline build for iProov dependencies.

## How it works

We have a QuickStart backend portal where your frontend (this POC) code can call to retrieve the iProov token and validate results.

The assets source at https://cdn.iproov.app/ – where the typography, verification engine, and other files are stored in a CDN.

To download the assets files, refer here for all the files. You should be able to download the package from there. Here are the next steps on what you need to do:

1. Unzip the package
2. Copy the **iproov-assets** folder into **/dist**

Since this simple POC is using `http-server` to serve the static content, it serves through port `8080`. We've hard-coded `assets_url` to point to `assets_url="/"`.

You could take a look at this implementation in the **/pages** folder.