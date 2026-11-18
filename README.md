# Cisco Webex Contact Center LiveChat – GitHub Pages Demo

A simple static HTML page that loads the Cisco Webex Contact Center LiveChat widget.

## Files

- `index.html` – LiveChat widget integration and browser-load fallback message.

## Publish with GitHub Pages

1. Create a GitHub repository (for example, `cisco-webex-livechat-demo`).
2. Add `index.html` to the repository's root folder.
3. Commit and push the file to the default branch.
4. In GitHub, open **Settings → Pages**.
5. Under **Build and deployment**, select **Deploy from a branch**.
6. Select your default branch and the `/ (root)` folder, then save.
7. Wait for GitHub Pages to publish the site. Open the URL shown in the Pages settings.

## Before testing

- Confirm that the Cisco Webex Contact Center tenant/widget configuration allows the published GitHub Pages domain.
- Confirm any required domain allowlisting, CSP, and security settings with your Cisco administrator.
- The page loads the Cisco-hosted script from `chat-widget.produs1.ciscoccservice.com`; the widget will not work if that service is unreachable or the tenant configuration is invalid.
- Test in a supported, up-to-date browser and check the browser developer console if the widget does not appear.

## Important

The fallback message is displayed when the external Cisco script fails to load. A script-load failure does not, by itself, prove that the browser is unsupported; network restrictions, domain configuration, or service availability can also cause it.

The widget IDs and script URL in this demo are preserved from the supplied snippet. Treat tenant-specific identifiers as configuration data and avoid publishing them publicly unless your organization permits it.
