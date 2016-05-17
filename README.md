## Dependencies
**Install:**
`npm install`
`bower install`

**Notes:**
Ensure that your $PATH contains the following in this order:
```
node_modules\.bin;
bower_components\.bin;
%USERPROFILE%\AppData\Roaming\npm;
C:\Program Files\nodejs;
```
When using a dependency within mtz-seed-element all imports should be treated as though they have the same root, import
Polymer by using:
`../polymer/polymer.html`

## Linting
**Run:**
`npm run lint`

**Notes:**
It's recommended to use linters directly in your code editor and support can be added through plugins for polylint and
eslint.

## Testing
**Run:**
`wct` - Runs all of your tests
`wct -l chrome` - Will only run tests in chrome.
`wct -p` - Will keep the browsers alive after test runs (refresh to re-run).
`wct test/some-file.html` - Will test only the files you specify.

**Notes:**
If your tests are running extremely slow for some reason, odds are that Launchpad is having trouble locating your
browser binaries, to resolve this set LAUNCHPAD_BROWSERS=chrome and LAUNCHPAD_CHROME in your environment variables.
This holds for all supported browsers: chrome, canary, firefox, aurora, ie, safari, phantom

## Serving
**Run:**
`polyserve`

**Notes:**
You can run tests in your browser using: `http://localhost:8080/components/mtz-seed-element/test/`.
Demo pages are available at `http://localhost:8080/components/mtz-seed-element/demo/`.
