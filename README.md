# futbot-app-download

Public landing page (GitHub Pages) that links to the latest Futbot Android build on EAS.
It hosts no binaries.

The site's own SemVer is in `package.json` and the `futbot-site-version` meta tag in
`index.html`. Bump it once for every site change and run `npm run check`. This is
separate from the Android app version shown on the page.

## Releasing a new build

After each EAS build:

1. Edit `index.html`: set the new version in the `.version` paragraph (`<span id="v">`).
2. Replace the button `href` with the new EAS build URL.
3. Bump the site's own SemVer and run `npm run check`.
4. Merge the reviewed change through a PR after authorization; Pages redeploys from `main`.

Only public information belongs here. Never commit secrets or APK files.
