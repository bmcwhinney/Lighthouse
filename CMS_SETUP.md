# Decap CMS Setup (Free, Netlify + GitHub)

This project now includes a client-friendly editor at `/admin`.

## One-time Netlify dashboard setup

1. Open your site in Netlify.
2. Go to `Site configuration` -> `Identity` and click `Enable Identity`.
3. Under Identity settings:
   - Set `Registration preferences` to **Invite only** (recommended).
   - Enable **Git Gateway**.
4. Invite your client by email from the Identity tab.

### Note about invitation links

Sometimes the invite email lands users on the **homepage** first (instead of `/admin/`). That is OK: Identity invite tokens arrive in the URL hash, and this site loads the Netlify Identity widget on both `/` and `/admin/` so the invite completion flow can finish and then redirect to `/admin/`.

## How your client edits content

1. Visit `https://your-site-domain/admin/`.
2. Log in from the Netlify Identity prompt.
3. Edit fields in **Homepage Content**.
4. Click **Publish**.

Changes are committed to GitHub and deployed automatically by Netlify.
