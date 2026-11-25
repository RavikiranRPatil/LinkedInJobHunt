# Data roles, found

A lightweight job feed for Data Engineer and related openings in the Netherlands.

## Run locally

This is a static web app with no build step or dependencies. From the project folder, start a local web server:

```powershell
python -m http.server 8000
```

Then open <http://localhost:8000>.

## Listings and updates

The app reads the public [Arbeitnow Job Board API](https://www.arbeitnow.com/blog/job-board-api), filters its latest listings for data-engineering roles and Netherlands locations, and checks for new data every minute. The source feed itself refreshes about once an hour, so new listings may take up to an hour to appear. Openings link to their original postings. An internet connection is required.