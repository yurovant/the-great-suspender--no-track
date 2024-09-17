<h3>The Great Suspender fork without analytics tracking</h3>
<hr>

Modified version of `The Great Suspender` Chrome extension without analytics tracking and rogue JavaScript files from an anonymous developer who is now in control of the GitHub source and web store versions. I forked it for my personal use.


<h3>Read more</h3>
<hr>

* [New ownership announcement](https://github.com/greatsuspender/thegreatsuspender/issues/1175)
* [New maintainer is probably malicious](https://github.com/greatsuspender/thegreatsuspender/issues/1263)
* [Flagged as malware by Microsoft Edge](https://www.windowscentral.com/great-suspender-extension-now-flagged-malware-edge-has-built-replacement)
* [Reddit forum discussion](https://old.reddit.com/r/HobbyDrama/comments/jouwq7/open_source_development_the_great_suspender_saga/)
* [Medium article](https://medium.com/nerd-for-tech/malware-in-browser-extensions-3805e8763dd5)

This project is a fork from [v7.1.8 of The Great Suspender](https://github.com/greatsuspender/thegreatsuspender) with all tracking code removed, along with some annoying popups/prompts.

<h3>Build from GitHub</h3>
<hr>

You will need these dependencies to be installed first:

* `openssl`
* `Node.js`
* `npm`

Steps to follow:

* clone repository
* switch to folder with repository 
* run `npm install`
* run `npm run generate-key`
* run `npm run build`
* it should say `Done.`
* switch to newly created `build/zip` folder and unzip file that starts with `tgs-`
* open your Chromium-based web browser
* type `chrome://extensions/` in the URL bar
* click on `Load unpacked` button on the top left
* select recently unpacked zip that starts with `tgs-`
* setup your extension


<h3>Shoutouts</h3>
<hr>

* This package uses the [html2canvas](https://github.com/niklasvh/html2canvas) library written by Niklas von Hertzen
* It also uses the IndexedDB wrapper [db.js](https://github.com/aaronpowell/db.js) written by Aaron Powell
* Original source from [The Great Suspender v7.1.8](https://github.com/greatsuspender/thegreatsuspender)


<h3>TODO</h3>
<hr>

* [Migrate from Manifest V2 to Manifest V3](https://developer.chrome.com/docs/extensions/migrating/)
