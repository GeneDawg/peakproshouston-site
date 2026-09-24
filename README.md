# Peak Pros Houston

Contractor platform for roof rejuvenation, maintenance, and repair opportunities across the Houston, Texas market. Houston counterpart to [peakprosga-site](https://github.com/GeneDawg/peakprosga-site).

## Files

- `index.html` — Public landing page (hero, how it works, earnings)
- `login.html` — Contractor access-code login (sessionStorage-gated)
- `portal.html` — Authenticated job-assignment submission form

## Authentication

Simple sessionStorage gate (not security — restricts the form, not the URL):

- Access code: `PEAKTX2026`
- Session key: `pptx_auth`

## Form routing

The job-assignment form (`portal.html`) uses Netlify Forms (`data-netlify="true"`) and routes to `assignment@peakprosusa.com`. The notification email must be configured in the Netlify dashboard under Forms → Form notifications. There is no Stripe or payment integration in this site.

## Deploy

Designed for Netlify (Drop or GitHub integration), same workflow as `peakprosga.com`. No build step — pure static HTML.
