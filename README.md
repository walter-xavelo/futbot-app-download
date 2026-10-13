# futbot-app-download

Public landing page (GitHub Pages) that links to the latest Futbot Android build on EAS.
It hosts no binaries.

## Releasing a new build

After each EAS build:

1. Edit `index.html`: set the new version in the `.version` paragraph (`<span id="v">`).
2. Replace the button `href` with the new EAS build URL.
3. Commit and push to `main`; Pages redeploys.

Only public information belongs here. Never commit secrets or APK files.
