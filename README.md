# Find My Home

A private, mobile-friendly dashboard for a 2 BHK rental search in Bengaluru. It is hosted on GitHub Pages.

- **Listings** (`data/listings.json`, `data/meta.json`) are refreshed once a day by a scheduled cloud search. The data comes from public owner listings and always links to the original listing.
- **Sign-in and collaboration** (shortlist, comments, votes, private notes) use Supabase, with email sign-in links and Row Level Security. Anyone with the link can view listings and the daily report without signing in. Signing in is optional and only needed to shortlist, comment, vote, keep notes or edit preferences; only invited emails can do that.
- `config.js` contains only the Supabase project URL and the *publishable* key, both of which are designed to be public. No secret keys are stored in this repository.
