# sukajee-legal

Public pages for Sukajee apps: privacy policies, terms of use and account deletion
instructions. Served with GitHub Pages at <https://sooshil.github.io/sukajee-legal/>.

## Layout

```
index.html                 list of apps
assets/style.css           shared style (light and dark)
<app>/index.html           the app's page, linking to the rest
<app>/privacy/index.html   privacy policy
<app>/terms/index.html     terms of use
<app>/delete-account/      how to delete an account and its data (Google Play asks for this URL)
```

The apps link to these URLs, so keep each path stable. To add an app, copy `cognikids/`,
rewrite it for that app, and add it to `index.html`.

## Changing a policy

Edit the page, update its "Last updated" date, and commit. Pages deploys on every push to
`main` in about a minute. For a material change to a privacy policy, also tell users in the
app's release notes.

Plain HTML, no build step. `.nojekyll` tells Pages to serve the files as they are.
