# Thornbury Swing Band – Static Site

Plain static HTML site, ready to serve via GitHub Pages.

## Structure

```
index.html              – Home
the-band/               – About the band
your-event/             – Booking info
events-coming-up/       – Upcoming events
media/                  – Audio & video
gigs/                   – Past events
contact/                – Contact & privacy policy
assets/
  style.css             – Shared stylesheet
  uploads/              – All images from original WordPress site
```

## GitHub Pages setup

1. Push this folder to a GitHub repository
2. Go to **Settings → Pages**
3. Set source to **main branch / root folder**
4. Your site will be live at `https://<username>.github.io/<repo>/` i.e. in this case at https://owen-kellie-smith.github.io/tsb-static/

## Notes

- `.nojekyll` is present so GitHub Pages won't try to process as Jekyll
- All image paths are relative — no changes needed for subdirectory hosting
- Contact form uses a `mailto:` link (WordPress form not available in static)
- Media page has placeholder text — embed audio/video URLs when available
