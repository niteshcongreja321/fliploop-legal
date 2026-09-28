# Fliploop legal and support site

This folder is the small static website for Fliploop, the iOS app for resellers published by NK Genesis. It holds the home page, Privacy Policy, Terms of Use and Support page as plain HTML with one shared stylesheet (no JavaScript, no external fonts, no trackers), and it is served as-is by GitHub Pages; the empty `.nojekyll` file tells Pages to skip Jekyll processing, and all links are relative so the site works at a project path such as `https://<user>.github.io/fliploop-legal/`.

## Supabase keep-alive

`.github/workflows/supabase-keepalive.yml` pings the Fliploop backend
(Supabase project `fkzpuhbhjvgqssqsnyik`) once a day at 07:23 UTC, so the free
project doesn't pause. It lives here because Actions is free for public repos.
It uses only the app's public key. A failed run means the project may be
paused: restore it in the Supabase dashboard.
