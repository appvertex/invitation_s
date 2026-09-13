# Offline invitation preview

This repository is a static, offline-friendly mirror of the **Minimalism Dark
Red** invitation demo. It does not require Node.js, a database, or any build
tool. The deployed home page opens `offline-preview.html` automatically.

## Deploy to Cloudflare Pages

1. In Cloudflare, open **Workers & Pages** and select **Create application** →
   **Pages** → **Connect to Git**.
2. Select the GitHub repository `appvertex/invitation_s` and choose the `main`
   branch.
3. Use these build settings:

   | Setting | Value |
   | --- | --- |
   | Framework preset | `None` |
   | Build command | `exit 0` |
   | Build output directory | `.` |
   | Root directory | Leave blank |

4. Select **Save and Deploy**. Cloudflare will publish the site on a
   `*.pages.dev` address and redeploy future pushes to `main` automatically.

## Offline limitations

The invitation visuals and saved gallery are local. Live functions from the
original service, such as RSVP submission, guestbook storage, and the embedded
Google Map, need their original backend/API and are not included.
