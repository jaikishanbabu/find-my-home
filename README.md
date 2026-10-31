# Find My Home

A private, mobile-friendly dashboard for a 2 BHK rental search in Bengaluru. It is hosted on GitHub Pages.

- **Listings** (`data/listings.json`, `data/meta.json`) are refreshed once a day by a scheduled cloud search. The data comes from public owner listings and always links to the original listing.
- **Collaboration** (shortlist, comments, votes, private notes) use Supabase, with email sign-in links and Row Level Security. There is no email sign-in. The dashboard asks for a passcode once per device; the database checks it (only a salted hash is stored, never in this repo) before allowing shortlist, comment, vote, note or preference changes.
- `config.js` contains only the Supabase project URL and the *publishable* key, both of which are designed to be public. No secret keys are stored in this repository.
