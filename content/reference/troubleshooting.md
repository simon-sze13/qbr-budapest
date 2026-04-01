# Troubleshooting

## Cannot sign in

- Confirm **SSO / VPN** steps from your facilitator.
- Try a **private browser window** to rule out stale cookies.
- Check **clock skew** on your laptop if certificate errors appear.

## Missing project or cluster

- Verify you are using the **workshop organization** and **project name** from the invite.
- Ask facilitators to confirm your user was added to the correct **RBAC** group.

## Deploy fails or stays pending

- Note the **exact error message** or event (screenshot for internal channels only).
- Confirm **quota** and **namespace** limits in the workshop tenant.
- Retry once; if it persists, escalate on the facilitator **Slack/email**—do not post secrets publicly.

## This site looks broken after fork

- Run `mkdocs serve` from `instructor/mkdocs` after installing `requirements.txt`.
- Set **`site_url`** in `mkdocs.yml` to match your **GitHub Pages** URL (with trailing slash). For this repo: `https://simon-sze13.github.io/qbr-budapest/`.
- Ensure **GitHub Actions** completed successfully (**Settings → Pages**).
